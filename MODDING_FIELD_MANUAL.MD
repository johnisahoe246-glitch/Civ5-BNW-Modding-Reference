# Civ 5 Modding Field Manual: Workflow & Translation Layer

This document bridges the gap between a "Gameplay Idea" and the specific files required to execute it in this repository. 

## 1. TASK-TO-FILES MATRIX
When starting a new feature, only look at the files listed for that specific task. Ignore the rest of the repository.

### ⚔️ Creating a Custom Civilization
* **The Rules (XML):** `/XML-Schema/CIV5Civilizations.md`, `/XML-Schema/CIV5Traits.md`, `/XML-Schema/CIV5Leaders.md`
* **The Assets (XML):** `/XML-Schema/CIV5Units.md` (Unique Unit), `/XML-Schema/CIV5Buildings.md` (Unique Building)
* **The Colors (XML/UI):** `/XML-Schema/CIV5PlayerColors.md`, `/UI-and-Graphics/Color.md`

### 🏗️ Adding a New Building or Wonder
* **The Rules (XML):** `/XML-Schema/CIV5Buildings.md`, `/XML-Schema/CIV5BuildingClasses.md`
* **The Yields (XML):** `/XML-Schema/CIV5Yields.md`
* **Custom Effects (Lua):** Check `/API-Reference/` for `CityConstructed` hooks.

### 🧠 Modifying AI Behavior
* **Personality (XML):** `/AI-Logic/CIV5Flavors.md`, `/AI-Logic/CIV5LeaderTables.md`
* **Decision Making (XML):** `/AI-Logic/CIV5AIGrandStrategies.md`, `/AI-Logic/CIV5AICityStrategies.md`
* **Diplomacy (XML/Lua):** `/AI-Logic/CIV5MinorCivApproachTypes.md`, `/API-Reference/` for `Team` and `Contact` hooks.

---

## 2. THE "GOLDEN HOOKS" (Known Useful Lua Events)
Out of thousands of API references, these are the most reliable Lua hooks for injecting custom gameplay logic. Search the `/API-Reference/` folder for these specific terms.

### Turn & Time Hooks
* `GameEvents.PlayerDoTurn(playerID)`: **The most used hook.** Fires at the start of every player's turn. Perfect for recurring effects (e.g., giving a Civ +5 gold per turn).
* `Events.ActivePlayerTurnStart()`: UI-focused. Use this to update custom UI panels when the human player's turn begins.

### Combat & Conquest Hooks
* `GameEvents.UnitKilledInCombat(winningPlayerID, losingPlayerID, unitType)`: Triggers exactly when a unit dies. Best for "gain culture on kill" or spawning temporary units.
* `GameEvents.CityCaptureComplete(oldPlayerID, capital, x, y, newPlayerID)`: Best for triggering massive empire-wide effects or narrative pop-ups when a city falls.

### Construction & Tech Hooks
* `GameEvents.CityConstructed(playerID, cityID, buildingID, bGold, bFaithOrCulture)`: Fires when a building finishes. Use to trigger one-time Lua bonuses that XML can't handle.
* `GameEvents.TeamSetHasTech(teamID, techID, bFirst)`: Fires when a technology is researched. Good for unlocking custom Lua-driven abilities or eras.

---

## 3. ENGINE RULES & DANGER ZONES
* **State Preservation:** Civ 5 does not automatically save custom Lua variables when the player saves the game. You MUST use a saving utility (like `TableSaverLoader` or `ScriptData`) to persist data, or your mod will break on reload.
* **UI Reloads:** Changing Lua UI files requires the user to fully reload the game or mod. It cannot be hot-swapped easily.
* **The VFS Rule:** All custom Lua scripts, DDS textures, and MP3 files must have `Import into VFS = True` in ModBuddy, or the game engine will ignore them completely.