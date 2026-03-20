This is actually pretty simple (on a PC).  Here are the steps:
* Open CvDefines.h
* Find "#define MAX_CIV_PLAYERS" and look over to the right.  That number is the number of players allowed not including barbarians, 18 by default.
* Change the number to the maximum number of players you want.
* Save the file and do a clean build of the DLL.

That's it!