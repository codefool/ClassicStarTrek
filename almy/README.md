-- retrieved from https://almy.us/sst.html 18/08/2022

The Classic Super Star Trek Game

Super Star Trek is quite possibly the best of the "Star Trek" games from the 
1970's. Of course, it does not make use of graphics, or even assume a video 
display, but it still an interesting game to play, particularly for those of 
us who don't have the reflexes we used to and prefer a more cerebral computer 
game.

Of course, Star Trek and it's characters are trademarks of Paramount Studios, 
Inc. And just like the original game, written by Star Trek fans who were also 
the, back then, rare breed of computer geek, isn't used with permission but with 
admiration of the show.

This game was written by David Matuszek and Paul Reynolds, with modifications 
by Don Smith. I've received further information that the black holes, Tholian 
web, Super Commander, and Emeritus mode were added by Marc Newman. I resurrected 
the game, rewrote it in C, and fixed many bugs.

In June 2002, I fixed two known bugs and a documentation typo, and created a 
new Linux version. In June 2004 I fixed a number of bugs involving: 

1) parsing invalid numbers, 
2) manual phasers when SR scan is damaged and commander is present, 
3) time warping into the future, 
4) hang when moving klingons in crowded quadrants.

In December 2010, I fixed bugs involving attempting to fire more than 3 
torpedoes at once, a typo ("READ ALERT"), and a couple of buffer overflow issues.

In October 2013 I fixed a bug that caused the number of remaining Klingons to be 
negative when the remaining Klingons and the Enterprise are destroyed in a Super 
Nova. Typos pointed out by users have been corrected. I added the ability to get 
the current score (why was that never possible?), and have an optional fix that 
rotates the scan displays so that the X axis is horizontal. Yes, for some reason 
the authors of SST had the displays rotated 90 degrees clockwise. Just add -f as 
the first command line argument. Fixed instance where total casualties would 
decrease when casualties occur.

In December 2013 I added three new commands -- CLOAK to cloak the Enterprise, 
CAPTURE to allow Klingons to surrender, and SCORE to show the score in the game. 
I also fixed many typos in the program dialog and in the documentation.

In June 2015 I fixed some bugs that kept certain counts from being reset when 
starting a new game. In August I fixed a bug that was reporting a violation of 
the Treaty of Algeron that did not occur, and the lack of the Score command in 
the Windows version. In December an extraneous control-S character was deleted 
from sst.c source file.

In January 2019 I did the following: Numerous reported typos, spelling, and 
grammar errors corrected. References to "Romulan ship captured" changed to 
"Romulan ship surrendered" since that is what happens at the end of a won game. 
"Klingons per stardate" changed to "Klingon ships per stardate".

Death Ray can no longer be repaired with a 0.1 stardate rest at a base.

Damage Report no longer states the Death Ray can be repaired away from a base.

Capturing prisoners while docked will have them immediately transferred to the 
base rather than going into the ship?s brig.

If the Cloaking Device is damaged in the same turn it is activated, it gets 
deactivated.

Destroying the remaining enemy ships with the Death Ray should no longer give a 
negative number of Klingons left.

If the game is compiled without the CLOAK, CAPTURE, and/or SCORE commands, 
issuing those commands now gives an invalid command message rather than just 
being silent. These commands are enabled by default.

In February 2019 I corrected a compilation error (I compiled it for "Debug") 
in the Windows Console version.

Super Star Trek For LINUX (77k) -- built for 32-bit Linux. If you have a 64-bit 
distribution you will need to add 32-bit support or recompile from source.
[https://almy.us/files/sstlinux.zip]

Super Star Trek for Windows Console (98k) [https://almy.us/files/sstnt.zip]

Super Star Trek for Mac OS X (85k) -- 64-bit Intel only. 
[https://almy.us/files/sstosx.zip]

Source code (Generic ANSI C, 90k) As is will build on Linux or Mac OS X. Has 
instructions to build with VisualStudio for Windows. 
[https://almy.us/files/sstsrc.zip]

These do not have the the bug fixes:

Super Star Trek For DOS (83k) [https://almy.us/files/sstdos.zip]
Super Star Trek For OS2 (95k) [https://almy.us/files/sstos2.zip]

The DOS version requires a 80386 or better. Since source code is available, 
Super Star Trek can be compiled for virtually any system having a C compiler 
and sufficient memory for execution (which isn't much by today's standards!)

All versions have an executable program as well as a documentation file, SST.DOC.
The SST.DOC file must be in the same directory/folder as the program is run from 
in order to view the documentation from within the game with the HELP command.

-------------------------------------------------------------------------------
History of This Version

I first played Super Star Trek in the mid 1970's. It was a game on the Control 
Data mainframe computer, and was a big hit at work during evening hours.

About 1977 I got a copy the source code of the game. Someone had converted it 
to PDP-11 Fortran but couldn't get it to run because of its size. I modified 
the program to use overlays and managed to shoehorn it in on the 56k byte machine.

I liked the game so much I put some time into fixing bugs, mainly what could be 
called continuity errors and loopholes in the game's logic. We even played a 
couple tournaments.

In 1979, I lost access to that PDP-11. I did save the source code listing. In 
1995, missing that old friend, I started converting the program into portable 
ANSI C. It's been slow, tedious work that took over a year to accomplish.

In early 1997, I got the bright idea to look for references to "Super Star Trek" 
on the World Wide Web. There weren't many hits, but there was one that came up 
with 1979 Fortran sources! This version had a few additional features that mine 
didn't have, however mine had some feature it didn't have. So I merged its 
features that I liked. I also took a peek at the DECUS version (a port, less 
sources, to the PDP-10), and some other variations.

-------------------------------------------------------------------------------
Modifications I Made

Compared to original version, I've changed the "help" command to "call" and the 
"terminate" command to "quit" to better match user expectations. The DECUS 
version apparently made those changes as well as changing "freeze" to "save". 
However I like "freeze".

I added EMEXIT from the 1979 version.

That later version also mentions srscan and lrscan working when docked (using 
the starbase's scanners), so I made some changes here to do this (and 
indicating that fact to the player), and then realized the base would have a 
subspace radio as well -- doing a Chart when docked updates the star chart, and 
all radio reports will be heard. The Dock command will also give a report if a 
base is under attack.

It also had some added logic to spread the initial positioning of bases. That 
made sense to add because most people abort games with bad base placement.

The experimental deathray originally had only a 5% chance of success, but could 
be used repeatedly. I guess after a couple years of use, it was less 
"experimental" because the 1979 version had a 70% success rate. However it was 
prone to breaking after use. I upgraded the deathray, but kept the original set 
of failure modes (great humor!).

I put in the Tholian Web code from the 1979 version.

I added code so that Romulans and regular Klingons could move in advanced games. 
I re-enabled the code which allows enemy ships to ram the Enterprise; it had 
never worked right. The 1979 version seems to have it all fixed up, but I'm 
still not overly happy with the algorithm.

The DECUS version had a Deep Space Probe. Looked like a good idea so I 
implemented it based on its description.

In 2013 I added the CLOAK and CAPTURE commands and also fixed lots of bugs. The 
CAPTURE command is based on the one in BSDTrek. When making this change I also 
changed text so that killing Klingons became destroying Klingon ships reflecting 
that a Klingon ship does have more than one Klingon aboard! The CLOAK command 
and some other bug fixes and correction of typos are thanks to Erik Olofsen.

I revised the documentation to match the version.
---------------------------------
Tom Almy [https://almy.us/almy.html]
webmaster9@almy.us
Last modified Feb 2019
