-- retrieved from http://www.dunnington.info/public/startrek/ 08/18/2022

Star Trek

Star Trek was a very popular game on early microcomputers and minis, and lots of 
versions existed at one time. The "standard" was originally written in BASIC for 
a Sigma 7, then rewritten in Hewlett Packard BASIC, by Mike Mayfield in 1972. It 
was included in the HP library early in 1973. Most versions are BASIC or FORTRAN 
adaptations of this, which was based on an 8 x 8 galactic grid.

David Ahl translated Mike Mayfield's code to DEC BASIC and then with Mary Cole, 
to BASIC-PLUS for RSTS-11 in 1973. The program was published in the first 
edition of 101 BASIC Computer Games under the name SPACWR (Space War) and 
various people translated that, in turn, to other versions for other DEC 
machines and operating systems. Bob Leedom upgraded this version, adding things 
like the damage and status reports, galactic quadrant names, and a more powerful 
library computer, while he was porting it to Data General's NOVA. Ahl called 
this extended version "Super Star Trek", and published it in the "Microcomputer 
Edition" of BASIC Computer Games, published by Creative Computing in 1978. It 
was converted to MicroSoft 8K BASIC (notice the capital 'S' in MicroSoft in 
those days) by John Borders; the version below under the name "startrek.txt" 
is almost identical.

Recently I had some email from Aron Insinga, who'd found this page, and he was 
able to give me some interesting information about his version. Although it's 
contemporary with David Ahl's, it's derived directly from the HP version, and 
he didn't see Ahl's version until later:

Back in the 1970s there was a computer center in Delaware that was used by the 
high schools in the state and was staffed by students. We had the 2nd RSTS-11 
system that DEC sold. Kids were using the Project DELTA Teletype and DataPhone 
at their school to make long distance calls to a time-sharing system at the HP 
facility in Avondale, PA. They were using the system for hours to play this 
Star Trek game and the phone bill was a big problem. I was told that it would 
help a lot if I could get it to run on our RSTS-11 (PDP-11/20) system at Project 
DELTA.

Aron described how he modified the program to fit in 8K (it would normally need 
about 24K), and some of the other things he worked on as a high-school student. 
His version of Star Trek was RSTS-11-20, only the 20th program published by DEC 
for the RSTS operating system. Later he went to work for DEC.

There's a good writeup of the early history of this line of Star Treks and how 
the "Super" came to be added to "Star Trek" at Maury Markowitz's webpage.

Lynn Cochran adapted a member of this family in February 1976. It was published 
in SCCS INTERFACE in June '76, and was the version most MITS Altair 8800 users 
knew. It had fewer commands - lacking a damage report and shield control - but 
with MITS 8K BASIC, it would run in 12K bytes of memory. This SCCS INTERFACE 
listing was in turn slightly modified by Dr. Li Chen Wang to create a slightly 
smaller version (published in the Peoples Computer Company journal, July 1976) 
for his Palo Alto TINY BASIC (published in Dr Dobbs Journal, May 1976). This 
used words (well, letters) instead of numbers for commands, and achieves the 
impressive feat of fitting both the interpreter (1.77K bytes) and the program 
(just over 6K) into a machine with only 8K memory! A different, even smaller, 
version for use with Bruce Sherry's version of TINY BASIC manages the same feat.

Another adaptation of Mike Mayfield's program appeared as STTR2 on the Univac 
1100, and was then ported by Ralph Hopkins to Processor Technology's Sol-20 
microcomputer using BASIC/5,. In 1978, this evolved into GALAXY with more ships, 
more enemies, and a 10 x 10 grid, and then around 1982 into COMBAT with still 
more sophistication (no more grids), both for Sol-20 Extended Cassette BASIC.

Processor Technology's own TREK80, dated 1977, was coded in 8080 assembly 
language. It's particularly notable because it includes sound effects, obtained 
by placing an AM radio near the computer, to pick up the electronic "noise" 
from the machine.

Meanwhile, of course, other people had made other modifications, or started 
with different sources - Mike Mayfield wasn't the only or even the first person 
to write a Star Trek program. Bob Bishop, who later wrote APPLEVISION, the 
first ever Apple HiRes graphic game (Rocket Pilot), and several others, had 
heard of Star Trek games but never played any when he wrote APPLE STAR TREK for 
the original Apple computer (which we now often call the "Apple-1") in late 
1976. It was published in Interface Age (commercial successor to SCCS 
INTERFACE) in May 1977, just a couple of months before the Apple II became 
available.

One notable lineage originated with William Char and friends at City College of 
San Francisco and passed into circulation as TREK73 from Lawrence Hall of 
Science, UC Berkeley. You can find later versions of this around the 'net, 
written in C, but the original was in BASIC; in fact, the same HP 2000C BASIC 
used by Mike Mayfield. 30 years later, almost to the day, I've re-typed TREK73 
from a 45-page listing, kindly donated by Kermit Murray.

TREK73 begat a C version (for UNIX), which begat an MS-DOS port around 1985. 
Those, and other programs, almost certainly influenced the development of the 
multi-user TREK83; somewhere along the line we got Xtrek and Netrek, but I was 
never so interested in those.

Star Trek games appeared in many languages, and have remained popular to this 
day. For example, John Thingstad faithfully copied David Ahl's version from 
BASIC Computer Games, but in LISP. Other modern versions exist in the form of 
Java applets, Z-code, programs for the Cybiko, Palm Pilot, Sharp Zaurus, and 
many others.

Here are listings of two dozen versions, written in BASIC:

STTR1	        Mike Mayfield's original HP BASIC (extracted from HP tape image), 1972 
    [http://www.dunnington.info/public/startrek/STTR1]
    
spacwr.bas	converted to DEC BASIC (with MAT statements) by David Ahl, 1973
                [http://www.dunnington.info/public/startrek/spacwr.bas]
                
strtr1.bas	DEC BASIC-PLUS, probably from David Ahl, Part 1 (instructions)
                [http://www.dunnington.info/public/startrek/strtr1.bas]
                
strtrk.bas	DEC BASIC-PLUS, probably from David Ahl, Part 2 (the game)
                [http://www.dunnington.info/public/startrek/strtrk.bas]
                
spacwr.ba	OS-8 BASIC conversion for PDP-8, by Kay Fisher, about 1973/4
                [http://www.dunnington.info/public/startrek/spacwr.ba]
                
spacwr.in	text file: instructions for spacwr.ba
                [http://www.dunnington.info/public/startrek/spacwr.in]
                
TREK.BAS	adapted for RSTS-11 BASIC, by Aron Insinga, Project Delta, 20-JUL-73
                [http://www.dunnington.info/public/startrek/TREK.BAS]
                
TREK.DOC	text file: Instructions for TREK.BAS
                [http://www.dunnington.info/public/startrek/TREK.DOC]
                
UT-trek.basic	Hicks & Korp extended version for TAURUS, from UTexas, 5 April 1973
                [http://www.dunnington.info/public/startrek/UT-Trek.basic]
                
BIGMES.orig	HP 2000 version (paper tape punched by Doug Quebbeman, 1976)
                [http://www.dunnington.info/public/startrek/BIGMES.orig]
                
startrek.bas  	Lynn Cochran's version, common on Altairs, 1976
                [http://www.dunnington.info/public/startrek/startrek.bas]
                
instr	text file: instructions for Lynn Cochran's version above
                [http://www.dunnington.info/public/startrek/instr]
                
STARTREK.BAS  	A particularly small version (6K) for Palo Alto TINY BASIC, 1976
                [http://www.dunnington.info/public/startrek/STARTREK.BAS]
                
STARTREK.DOC	text file: instructions for the TINY BASIC version above
                [http://www.dunnington.info/public/startrek/STARTREK.DOC]
                
startrek.asc  	An even smaller version (under 6K) for PATB 3.1, 1976
                [http://www.dunnington.info/public/startrek/startrek.asc]
                
tiny.doc	text file: Information to go with TINY BASIC 3.1
                [http://www.dunnington.info/public/startrek/tiny.doc]
                
trek15	        One of the "Super Star Trek"s, this one for Intellec MDS, 1976
                [http://www.dunnington.info/public/startrek/trek15]
                
newgame4.bas	3-dimensional version for a CDC 6000, V.1.1 April 06 1976
                [http://www.dunnington.info/public/startrek/newgame4.bas]
                
newgame4.basic	As above but translated to PR1ME BASIC/VM
                [http://www.dunnington.info/public/startrek/newgame4.basic]
                
startrek.txt	BASIC-80 for CP/M (Microsoft BASIC), from Creative Computing, 1978
                [http://www.dunnington.info/public/startrek/startrek.txt]
                
sttr.bs5	Ralph Hopkin's Sol-20 BASIC/5 version, late 1970s
                [http://www.dunnington.info/public/startrek/sttr.bs5]
                
COMBT.ECB	Ralph Hopkin's COMBAT for Sol-20 Extended Cassette BASIC, February 1982
                [http://www.dunnington.info/public/startrek/COMBT.ECB]
                
CMDS.ECB	Instructions for COMBAT
                [http://www.dunnington.info/public/startrek/CMDS.ECB]
                
AppleStarTrek	Bob Bishop's Apple Star-Trek for Apple INTEGER BASIC, 1976
                [http://www.dunnington.info/public/startrek/AppleStarTrek]
                
AppleStarTrek.txt	text file: rules for Apple Star-Trek; retyped from a scanned copy
                [http://www.dunnington.info/public/startrek/AppleStarTrek.txt]
                
APPLETREK	INTEGER BASIC version for Apple II, by W SANDER 1/11/78
                (Has some machine code on the end)
                [http://www.dunnington.info/public/startrek/APPLETREK]
                
Star Trek 3.3	APPLESOFT version for Apple II, author/date unknown
                [http://www.dunnington.info/public/startrek/StarTrek3.3]
                
trek.bas	From Ensign Software, possibly for a Tandy Color Computer, 1982
                [http://www.dunnington.info/public/startrek/trek.bas]
                
strek	        BBC BASIC, an enhanced version for the BBC Microcomputer, about 1983
                [http://www.dunnington.info/public/startrek/strek]
                
GALAXY	        A thinly-disguised AcornSoft version of Star Trek for the BBC Micro, 1982
                [http://www.dunnington.info/public/startrek/GALAXY]
                
STREK	        Exidy Sorcerer version, adapted from Practical Computing around 1980
                [http://www.dunnington.info/public/startrek/STREK]
                
TREK73	        William K. Char's original HP 2000 BASIC version, 26-NOV-1973
                [http://www.dunnington.info/public/startrek/TREK73]
                

Here are a few in other languages:

startrek.c	Chris Nystrom's 'C' port of Mayfield-style StarTrek, 1995
                [http://www.dunnington.info/public/startrek/startrek.c]
                
startrek.doc	text file: Instructions for Chris Nystrom's version
                [http://www.dunnington.info/public/startrek/startrek.doc]
                
trek.tar.gz	gzipped tar file: Eric Allman's C version for Unix, 1993 (originally 1976)
                [http://www.dunnington.info/public/startrek/trek.tar.gz]
                
trekdocs.tar.gz gzipped tar file: documentation to Eric Allman's C version, as nroff source
                [http://www.dunnington.info/public/startrek/trekdocs.tar.gz]
                
spacwr.for	Mike Mayfield's version, DEC FORTRAN-IV, by Kay Fisher, 1974
                [http://www.dunnington.info/public/startrek/spacwr.for]
                
sttr.ftn	Mike Mayfield's version, CDC FORTRAN (author/date unknown)
                [http://www.dunnington.info/public/startrek/sttr.ftn]
                
startrek.exe	MS-DOS TREKWAR ver. 5.7, compiled Microsoft BASIC, by Stan Warman
                [http://www.dunnington.info/public/startrek/startrek.exe]
                
TREK.PAS	VAX/VMS Pascal, from Don Kooker, 1988
                [http://www.dunnington.info/public/startrek/TREK.PAS]
                
ctrek.cob	wow, a COBOL version!  By Kurt Wilhelm, 1979
                [http://www.dunnington.info/public/startrek/ctrek.cob]
                
trk80	        Processor Technology's TREK80. A binary file, but the Intel HEX is here.
                [http://www.dunnington.info/public/startrek/trk80]
                
trk80.pdf	PDF file: instructions for Processor Technology's TREK80
                [http://www.dunnington.info/public/startrek/trk80.pdf]
                
startrek.lisp	John Thingstad's LISP version of David Ahl's Super Star Trek
                [http://www.dunnington.info/public/startrek/startrek.lisp]
                
startrek.files	Help, map, and pic(ture) files which accompany startrek.lisp
                [http://www.dunnington.info/public/startrek/startrek.files]
                
startrek	is like a simplified TREK73, written in IMP, an Algol-like language used 
                at The University of Edinburgh (and elsewhere). Probably written by Dave 
                Briggs circa 1974; rescued from oblivion by Graham Toal.
                [http://www.dunnington.info/public/startrek/gamespd_briggs.txt]
                
Palm Trek	for the Palm Pilot (with CBASPAD 0.84 or higher) by Michael Baker
                [http://www.dunnington.info/public/startrek/palmtrek11.zip]
                
ztrek.z5	ZTrek, a Super Star Trek executable written in Z-code by John Menichelli
                [http://www.dunnington.info/public/startrek/ztrek.z5]
                
ztrek.inf	the ZTrek Inform source, ported from Chris Nystrom's C version
                [http://www.dunnington.info/public/startrek/ztrek.inf]
                
st.html	        Super Star Trek as a Java applet, by Jim Bat, December 2003
                Similar to TREK15, based on Star Trek 77 in FORTRAN
                [http://www.dunnington.info/public/startrek/st.html]
                
st.jar	        Java Archive for Jim Bat's applet
                [http://www.dunnington.info/public/startrek/st.jar]
                
StarTrek.doc.html HTML document: instructions to go with Jim Bat's Java applet
                [http://www.dunnington.info/public/startrek/StarTrek.doc.html]
                
sst	        a Super Star Trek executable for the Sharp Zaurus, by Mark Hart
                [http://www.dunnington.info/public/startrek/sst.zaurus]
                
sst.doc	        text file: instructions for Zaurus Super Star Trek
                [http://www.dunnington.info/public/startrek/sst.doc]

(actually Tom Almy's instructions for his Super Star Trek)
Since I would hate to be accused of interstellar racism, I'm pleased to be able 
to provide at least one view from the other side of the Neutral Zone:

romulan.bas    	Command the RSS VINDICTAE. Author/date unknown.
                [http://www.dunnington.info/public/startrek/romulan.bas]

I have several other versions "somewhere":

* STARTREK, a Sharp MZ80K cassette tape version (also about 1980, I think)
* StarTrek for Polymorphic Systems A00 11K BASIC, for a Poly-88 micro, published 
  in Practical Computing, April 1979
* TREK73, a version in C from about 1986

and probably some on RT-11 and UCSD p-systems as well.

It's amazing how many people wrote their own versions of Star Trek. To get an 
idea, take a look at the People's Computer Company Alumni Site 
[http://sumeru.stanford.edu/pcc/], especially the page for the Games Archive
[http://sumeru.stanford.edu/pcc/archive.html#GamesArchive].

Other places to find Star Trek listings and information include 

* Maury Markowitz's Star Trek page [http://www3.sympatico.ca/maury/games/space/star_trek.html], 

* Chris Nystrom's Classic Computer Game: Star Trek page [http://www.cactus.org/~nystrom/startrek.html] 

* the AI Attic [ftp://ftp.cc.utexas.edu/pub/AI_ATTIC/Programs/Classic/], 

* Kermit Murray's page [http://ch309c.chem.lsu.edu/~kmurray/other/trek73/] which has links to other 
versions, and any number of sites you'll find if you search for "classic basic 
games", or any of the authors' names you see above.

Of course, there are loads of other games in BASIC for microcomputers, 
especially from the late 1970s and early 1980s, because that's when home micros 
were really taking off. I keep a small number online, not really a 
representative sample, but a somewhat random collection of games that I've been 
asked for, or which have interested me for one reason or another.

Last updated: Sat Mar 26 23:28:05 2005

If anyone has other interesting StarTrek versions, I'd be glad to hear from you. 
I'm particularly interested in versions in other languages such as FORTH, LISP, 
or APL. You can contact me (pete) by email -- remove the "www" from the address 
of this web page, strip off the directory names, and put my name @ the front.

Star Trek® is a registered trademark of Paramount Pictures registered in the 
United States Patent and Trademark Office. The computer programs listed here 
are not affiliated to Paramount Pictures.
