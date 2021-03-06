```ASCIIDOC







                     WWIV Network Docs
                            v2.37
                                                            
                                                            
                                                            
                                                            
                                                            
    Copyright (c) 1998-2000, WWIV Software Services, LLC
               Copyright (c) 1995, Wayne Bell


                          Contents
  1 HISTORY ...........................................     
  2 INTRODUCTION ......................................     
  3 REGISTRATION ......................................     
  4 ORGANIZATION ......................................     
  5 WWIV SOFTWARE .....................................     
  6 INSTALLATION ......................................     
  7 USING THE NETWORK .................................     
  8 NETWORK FILES .....................................     
  9 STARTING YOUR OWN NETWORK .........................     
 10 TROUBLE-SHOOTING NETWORK CONNECTIONS ..............     
 11 FUTURE DIRECTIONS .................................
 Appendix A - Macro Language ..........................
 Appendix B - Macro Examples ..........................
 Appendix C - Network message types ...................
 Appendix D - Identifiers Used in BBSLIST .............
 Appendix E - Private Networks ........................
 Appendix F - Automated subboard requests .............
 Appendix G - Multi-Networking ........................
 Appendix H - USING HS/LINK ...........................
 Appendix I - Symbols in SUBS.XTR .....................
 Appendix J - External Message Interface ..............
 Appendix K - WSS Operational Policy ..................
                                                            

======================================================
1.  HISTORY
======================================================
                                                            
    The first version of WWIVnet Docs was written by Will   
Daystrom, also known as The Captain (1 @2370), who ran the  
White Star Line and who copyrighted the Documentation for   
WWIV v4.10 and WWIVnet Docs under White Star Line Software. 
His documentation was excellent and would not have needed   
to be rewritten if the WWIV BBS software and the networks   
associated with it were not growing and dynamic.  However,  
v4.21a of WWIV introduced the ability for a BBS to be on    
more than one network, and with that ability many new       
networks were started.  This documentation has been         
rewritten with those changes in mind, so that the current   
documentation will be useful regardless of which WWIV-based 
networks a board happens to belong to.  The part of the     
documentation detailing the policies and procedures of      
WWIVnet has been moved to a separate document.              
                                                            
    The second version of the WWIVnet Docs was written by
Filo in 1995, and was copyrighted by Wayne Bell and WWIV
Software Services (WSS) in order that future versions
could be built upon it without anyone's having to worry
about copyright infringements.

    This version incorporates all changes up to an including
Net37 and is maintained and distributed by WSS.
                                                            
======================================================
2. INTRODUCTION
======================================================
                                                            
    A network is a voluntary association of bulletin boards 
using WWIV software and participating in a network by
calling one another to facilitate the transfer of elec-     
tronic mail (email) and message bases (subs).
                                                            
    Through this network, a user of any of the bulletin     
boards that are members may send email to a user of any     
other board.  A user may also post on a message base which  
may be read by the users of systems which subscribe to that 
message base; thus, many of the networked subs have         
international distribution.  Because this system of communi-
cation is read by others and because it has an effect on    
systems other than the one on which it originates, a spirit 
of cooperation must prevail.                                
                                                            
    Out of this spirit grows systems of organization and    
regulation which are known as networks and which are        
discussed in separate documents distributed by those        
networks.  This document covers some of the aspects of the  
software which should be of interest to users and/or sysops 
regardless of the particular WWIV-based network(s) with     
which they are affiliated.                                  
                                                            
    WARNING: When you unzip the network software, you       
should see "- AV" on the line next to every filename.       
Furthermore, after the files have been extracted, you       
should see the message:                                     
                                                            
Authentic files Verified!  # XLD658  WWIV Software Services 
                                                            
  If you do not see the "-AV" and the above message (be     
sure the number is "XLD658"), then the files you have have  
been tampered with, and you should not use them.  Since     
this software is used by several WWIV-based networks, the   
files herein should not be extracted and included in        
another network package.  If you desire to distribute       
NETxx with another network software, you should include the 
NETxx.ZIP file in its entirety within the other network     
archive in order to preserve the AV codes.                  
                                                            
======================================================
3. REGISTRATION
======================================================
                                                            
    The WWIV network software is distributed as shareware,
which means (in this case) that you can use the WWIV and
WWIV network software for up to two months before
deciding whether or not to register WWIV.  If, at the end   
of the two month period, you decide to register WWIV,       
please see the 'read.me' file in the WWIV*.ZIP file for     
information on how to register.   If at the end of two      
months you decide NOT to register WWIV (and hence not use   
WWIV software for your BBS), you must stop using the WWIV   
and the network software.                                   
                                                            
    If/when you register WWIV (and receive a WWIV           
registration number), you have also registered the network  
software, and may use the bbs and network software on your  
system as you wish -- as a standalone BBS, or in a network. 
                                                            
   If you are running a BBS that is in no way based on WWIV 
software, but that uses the WWIV network software, then a   
similar registration procedure applies.  You can use the    
network software for a two month trial period.   If you     
decide to continue using the network software after the two 
month trial period, then you must register the network      
software at a cost of $25.  If you do not register the
network software at the end of the two month trial
period, you must stop using it.  Registration of the
network software for those systems not running a BBS
based on WWIV is done by following the instructions in the
NETREG.FRM included with each NETxx.ZIP packet.

    Note that registration of the BBS or the network software
does not include LNET II packaged with the Net37 software.
LNET II is a separately licensed product of CMI Software
bundled with Net37 for your convenience.
                                                            

4.  ORGANIZATION
======================================================
                                                            
    WWIVnet originally began in 1988 with 25 charter        
members who helped Wayne Bell develop the network software  
and debug it.  Since that time it has spread from a small   
Los Angeles-based system of local boards to several inter-  
national networks.

    When WSS was purchased in 1998, the WWIVnet and the
software itself were separated from each other to allow
for a more flexible operation and administration of the
network independant of any ties to the software business
and vice versa.
                                                            
     WWIVnet policies are explained in separate document
provided by Snorkel 1@2100, the current Network Coordinator.

    You may also want to refer to the WSS Operational Policies
included in Appendix K of this document.


5. WWIV SOFTWARE
======================================================
                                                            
   WWIV v4.20e and up support the automatic request for a
sub and the automatic removal provided that each board has  
the network software to support the feature and provided    
that the sysop has configured his board to allow auto-      
requests.  Beginning with NET32, the automatic request      
feature and an option for the description of the sub in the 
SUBS.LST is included in BOARDEDIT.  This feature should     
facilitate a board's adding or dropping subs that are       
subscribed to.                                              
                                                            
    The network software includes the creation of informa-  
tional files on each network system which reflects subs or  
messages received that have 'no place to go.'  In effect    
that would mean that the receiving sysop has not created a  
message base for that sub or has deleted it but is still    
receiving mail for it.  The sysop should check this file    
regularly and if he is receiving subs that he has not       
ordered or does not want, he should notify the sending      
host to please remove his system from the distribution      
list.  This information and other information on network    
connections may be found in your GFILES directory in files  
named NETDAT0.LOG, NETDAT1.LOG and NETDAT2.LOG.  The        
NETDAT0 is the newest log and NETDAT2 is the oldest log.    
These logs are only kept for a three day period unless you  
make other provisions to have them saved.  They may         
provide useful information to you in terms of what you      
are/are not receiving and in terms of problems that may     
occur in your network connection.  Under v4.22 of the BBS   
software the sysop can access these logs from the bulletin  
board by typing a comma at the main menu.                   
                                                            
    The sysop should also occasionally review his DEAD.NET  
file which will be in DATA.  Messages in this file are      
those which were bound for another system but which cannot  
be delivered after having arrived on your system.  Often    
these are due to one of two factors.  The first case might  
be due to a board's having subscribed to a sub and having   
been put on the distribution list for it before that board  
has been added to the bbslist.  Thus the system does not    
know where to deliver it.  If that is the case, the         
DEAD.NET should be left alone because once the system is    
added, the network software will deliver that mail to the   
new system.    The second case would occur when a board has 
left the network or has been temporarily disconnected from  
the network.  It may still be receiving mail because either 
the sysop failed to notify the host, mail was already in    
the system, or because the host sysop has failed to remove  
the board from the distribution list.  In that case, the    
mail may be safely deleted.  Before deleting the mail,      
you should check with the board's AC to be sure that the    
board is out of the network.                                
                                                            
    In addition, the sysop should write the host of the sub 
whose mail is going to DEAD.NET and inform the host of      
which board is no longer on the network and request that    
host delete the board from the distribution list. NET32     
and up also has a feature to report on undeliverable e-mail 
to another system in the form of a System Short Message     
(SSM).                                                      
                                                            
    Sysops who receive subs from other systems have the     
responsibility to restrict access to the sub according to   
the rules of the host.  For example, some subs may limit    
access to User Number 1, to users with 255 access, or some  
other requirements such as all posts must not have tag      
lines.  The receiving sysop must also take steps to inform  
users of the rules applying to a particular sub.  GFILES    
are often a good way of doing this.                         
                                                            
    These guidelines for sysops are nothing more than       
common sense and normal courtesy which reflect the desire   
on the part of all to cooperate in order to make the        
network work properly and efficiently.  One of the          
interesting features of the network is that it is a great   
leveler.  No one (except possibly a few sysops) knows the   
age of the person making the post; therefore, people's      
impressions of the person who posts is made entirely based  
upon the language used and the thought expressed.  As a     
consequence many a young user can convey the impression     
that he is much older and more mature, and some older users 
may convey the impression that they are irresponsible,      
illiterate users.  One hopes that users will opt to convey  
the impression that they are mature, responsible human      
beings.                                                     
                                                            
    Sysops may choose to promote responsible use of the     
network by asking users to make their network posts conform 
to certain suggested guidelines.  For example, the Sysop    
may request that users:                                     
                                                            
   o    Not Use Foul language on the network                
   o    Not make personal attacks against others            
   o    Not post a lot of one-line messages on the network  
   o    Learn the differences between using A, W, or P to   
        respond to network messages.                        
                                                            
    These are merely suggestions for responsible use of the 
network and are not requirements; however, some of those    
suggestions are also found in the rules of the hosts of many
network subs.  Where they reflect the host rules, they are  
generally considered network rules for that sub.            
                                                            
     The following information lets you see at a glance the 
type of message (ie where it originated) when reading       
message bases:                                              
                                                            
   [1] = messages posted by you                             
   <2> = messages posted by someone else remotely           
   (3) = messages posted by someone else locally            
                                                            
     //BOARDEDIT now manages additional information for     
you, such as the host system #, whether a sub you host is   
auto-requestable, and whether the sub is automatically      
reported for SUBS.LST updates.  This additional info is     
stored in the "SUBS.XTR" file in your data directory, but   
DO NOT MODIFY THAT FILE DIRECTLY.  Use //BOARDEDIT all the  
time.  If you're using net31 or earlier, you'll notice that 
your nnall.net, allow.net, and subs.pub files will auto-    
matically be updated for you.  With net32 or later, the     
files will be deleted, as all the info is now in the        
SUBS.XTR FILE.                                              
                                                            
    You can now gate subboards among networks your system   
is a member of.  This is done in //BOARDEDIT, simply by     
entering net info for multiple networks.  In order to       
support sub gating, you need to be using net32 or later.    
Do not try listing different sub types in the same network, 
as it probably won't work. Gating DOES work with            
net-validation.  You can gate subs as either the host or    
as a subscriber system, but please do not gate subs unless  
you really have a good reason, and know what you're doing.  
Additionally, you need the permission of the original sub   
host in order to gate messages.                             
                                                            
   You can now net subboards by sub name (instead of just   
sub type).  A sub name is 1-7 chars of upper-case letters   
and numbers, and doesn't start with a number.  Note that in 
order to use sub-by-name, the host AND all subscribers      
need to be using v4.22 (or later) AND net32 (or later).     
Other than that, subs-by-name works the same as subs-by-    
number.  Because of changes being made by the telephone     
companies (see Section 10 - Future Directions), it may soon 
be necessary to run v4.22 or better in order to be able to  
use the sub-by-name feature in almost all networks.  There  
may even be a MANDATORY UPGRADE of both WWIV software and   
NET VERSION in the near future as a result of these changes.
                                                            
If you connect to the same system number in multiple        
networks, you can now force a callout to either one (you    
are prompted to select which one).  Future versions of the  
network software will allow you to pick up all network      
messages for your system on one call to the same connecting 
system.                                                     
                                                            
    You can now (correctly) forward mail between networks.  
If you're using net32 or later, if the person you forward   
the email to auto-replies, the reply will correctly go back 
to the original person who sent the email.  System Operators
also have the ability to Mail a received e-mail to someone  
else and add a message of their own.  In this case, a reply 
is sent to the sytem operator rather than to the original   
author of the mail.  This feature is available in WWIV v4.24
and higher.                                                 
                                                            
6.  INSTALLATION
======================================================
                                                            
    This section takes you step-by-step through the
installation process involved in setting up the network
executbles and other files necessary to the operation of
a WWIV-based network.
                                                            
ÚÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄ¿                           
³ Apply for Network Node Number ³                           
ÀÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÙ                           
                                                            
    The first step is to obtain a node number.  The         
appropriate method for doing this varies from network to    
network and is covered in the documentation specific to the 
network that you are interested in.  You may consult the    
NETWORKS.LST file included with this documentation to       
determine if a "contact person" has been designated for the 
network you are interested in.

    The node number should be entered in wwivconfig under Option  
N.  You may wish to enter information in wwivconfig for a "Net
low time" and "Net high time".  If you do this, it means    
that beginning at the low time and ending with the high     
time, a user who attempts to log in will receive a message  
indicating that your board is only accepting network calls  
during that time period.  For example,                      
                                                            
                 Net low time     : 03:00                   
                 Net high time    : 05:00                   
                                                            
would indicate that the network time period is from 3am to  
5am.  Military times are used to indicate time periods in   
the network.                                                
    Also, in wwivconfig option 1, you should insure that your     
board name and telephone number are entered exactly as they 
are shown in the BBSLIST.### or the BBSLIST.NET file which  
are also discussed later.                                   
                                                            
ÚÄÄÄÄÄÄÄÄÄÄÄ¿                                               
³CALLOUT.NET³                                               
ÀÄÄÄÄÄÄÄÄÄÄÄÙ                                               
                                                            
    You will have a CALLOUT.NET file which should be placed 
in your DATA directory, or in the case of multiple-networks-
 -in the date directory for each network, and which will    
 show the systems that you connect with. This file is in    
the following format:                                       
                                                            
  @node [macro options] [transmit options] [callout         
         options] [password]                                
                                                            
   Each of these options is discussed in turn.  The node is 
the node number of the board you are connecting with.       
ÚÄÄÄÄÄÄ¿                                                    
³Macros³                                                    
ÀÄÄÄÄÄÄÙ                                                    
    Macros are often used to achieve special purposes.      
These purposes include (a) connecting with another board    
in your area code where it is necessary to dial 1 before    
dialing the board number, (b) using a telephone service     
such as PcPursuit where special numbers, passwords, etc.,   
must be sent, (c) connecting with another board that is     
running WWIV as some form of door (i.e., WWIV is not        
answering the phone--instead some other software answers).  
                                                            
   The macro to use is designated in the CALLOUT.NET by %x  
where x is an integer number.  The macro should then be     
provided in the DATA directory under the name Mx.NET where  
x is the same number.                                       
                                                            
ÚÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄ¿                                          
³Transmit Options³                                          
ÀÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÙ                                          
   Transmit options are basically two.  You may use the &&  
parameter which means that files will be transferred each   
direction when a connection takes place.  If the && is      
omitted then the transfer will be uni-directional; from you 
to the other board.  In such a situation, you pay to send   
your files to the other board, and presumably, it will pay  
to send its files to you.  This is not a very efficient     
arrangement and is basically discouraged.                   
                                                            
    The other transmit option is for network compression.   
If you  specify the ; parameter, then network traffic to be 
transmitted to that node will be compressed, using pkzip's  
compression techniques. PKzip or other compression programs 
are not needed, as the compression/decompression code is    
built into the network software (using the PkZip data       
compression library).  You must ensure, however, that the   
system for which you specify compression is using net24 or  
higher; if they are using net23 or lower, all compressed    
data sent to that node will be lost.                        
                                                            
    Please do not assume that compression should be used    
for all your net connections.  Local connections and high   
speed connections that also use V.42bis are probably not    
good choices for using compression.  Also, try to avoid     
using MNP5 on connections for which compressed data is      
sent.  The packets that are created begin with z.   For     
example,                                                    
                                                            
        Z5252.NET                                           
                                                            
would indicate a compressed net packet bound for node 5252. 
You should check with the Sysop of the other node before    
enabling compression between your system and the other.     
Some experimentation may be necessary to determine which    
connections benefit from compression.                       
                                                            
                                                            
ÚÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄ¿                                           
³Callout options³                                           
ÀÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÙ                                           
   These options affect when your board will call the other 
board.                                                      
                                                            
      /x   Where x is an integer between one and 9.         
                                                            
This means that the network will force a callout to that    
board every x hours, even if there is no mail waiting to be
sent to that system.  This parameter is often set where     
one board does not often call the other.                    
    =   This means to call during the hours of 6 pm to 6 am 
Monday thru Friday and anytime on weekends).  These para-   
meters are handy for those long distance connections        
utilizing certain LD calling plans.                         
                                                            
   -    The minus parameter means to call during times when 
rates are  cheapest (11 pm to 7 am and anytime on           
weekends).  This parameter is recommended for long distance 
connections in order to minimize your phone bill.           
                                                            
   !    This limits the number of calls per day to 1.  The  
board will attempt to call out starting 20 hours after the  
last successful connect.  This feature only works with WWIV 
v4.12 or higher.                                            
                                                            
   !x   Where x is an integer.  This limits the number of   
calls per day to 20 divided by x.  The board will attempt   
to call out every 20/x hours after the last connect.  This  
feature only works with WWIV v4.12 or higher.               
                                                            
  +    The plus parameter indicates that your board does    
not call the indicated node; instead, that node should be   
calling you. If both of you have the + parameter in         
CALLOUT.NET then no transfers will take place between you.  
                                                            
  ~    The tilde (~) means that your system will never call 
out to the other system, and that the other system will     
never call yours to pick up mail.  The other system will    
only call yours to send data to you.                        
                                                            
  ^    The caret (^) is used to enable the HSLINK  protocol 
between your system and another.  If present on both        
systems (and the HSLINK executable is found on both         
systems), the network will attempt to use HSLINK as the     
protocol instead of Zmodem (or ymodem).  CAUTION: Be sure   
you do NOT have the -! modifier in your HSLINK.CFG file.    
NET32 now appends that modifier to the command line for     
outgoing Net calls.  If the -! is present in the HSLINK.CFG 
file, it may cause conflicts that could prevent optimium    
performance when recieving Net calls.  See Appendix for     
details on setting up HS/Link for WWIV.

  *    The asterisk (*) is used to force 10 digit dialing
required by many telephone systems due to the increasing
number of telephones and area codes.
                                                            
    Another set of parameters may be used to designate that 
the board should call between certain hours.  These         
parameters are illustrated below:                           
                                                            
  (3 )5     would mean that the board should call between 3 
am and 5 am.  Times are specified in 24 hour time.  Mid-    
night is specified as 0.

                                    
                                                            
     These parameters are useful if you are having a        
connection with a board that runs a NET TIME PERIOD or to   
insure that local connections take place during non-busy    
hours.  If none of these time delimiting parameters are     
used, your board will make the connection with the other    
anytime that there is mail to go out and the board is not   
busy.  This is NOT recommended for long distance            
connections unless you are using a WATTS line or other      
system that makes long distance a fixed cost.  It may be    
used for local connections if desired.                      
ÚÄÄÄÄÄÄÄÄÄ¿                                                 
³Passwords³                                                 
ÀÄÄÄÄÄÄÄÄÄÙ                                                 
   You should not enter a password in your CALLOUT.NET.     
The network software will generate a password between the   
two systems once there is a successful connection.  This    
is one way that you can tell whether or not your system     
has connected with the other. If there is a password        
present, there has been a connection. For more              
information on passwords, see the section on Trouble        
Shooting NetWork Connections.  Also note that the password  
will be in quotation marks as the last item on each line    
of CALLOUT.NET.  If you lose your password for some reason  
such as corrupt files or hard disk failure, you will need   
to contact the other sysop to have the password removed     
from his CALLOUT.NET file so that a new one may be          
established.                                                
ÚÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄ¿                                          
³Network Software³                                          
ÀÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÙ                                          
    You should obtain the latest version of the Network     
software and place the files in the main directory of your  
BBS.  That will be the directory where the BBS.EXE file     
resides.  You may determine the latest version of the       
software, by asking your network contact person or other    
network official to supply you with a copy of it. You       
should remain alert for changes in the network version.     
Currently, it is NET37; however, future versions will be
released as needed.  It is your responsibility to obtain    
these versions once you are on a network.                   
                                                            
   You may obtain them from The Mountain Empire BBS
(423) 477-4015, the WSS website http://wss.wwiv.com, or from
one of the WWIV Support Boards (you will get a list of these
with the WWIV software, and the list is updated from time to
time), or from one of your networks' officials.

   If you are running WWIV v4.30 or later and/or have a
FOSSIL driver insalled, you will want to delete NETWORK.EXE
and rename NETWORKF.EXE to NETWORK.EXE to take advantage of
the FOSSIL based communication routines.
                                                            
ÚÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄ¿                                       
³BBSLIST and CONNECT³                                       
ÀÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÙ                                       
   There are basically two ways of using the network        
software.  One of these ways is best suited for small       
networks and the other lends itself to larger networks.     
While both methods will work for small networks, the large  
method must be used when a network approaches 500 systems   
due to the way that some of the software functions.  A      
small network will only need two of the files mentioned     
below (BBSLIST.NET and CONNECT.NET) and all nodes will      
have a listing in each.  Large networks will use several    
BBSLIST and CONNECT files.  All of these files should be    
placed in the DATA directory if your board is only on one   
network.  If you are on more than one network, then the     
files for a particular network should be in its separate    
directory as you defined it in wwivconfig option N.               
                                                            
   BBSLIST.NET -  For a small network, this file can list   
all nodes participating in the network.  The general format 
of this file is discussed in the appendices.  A small       
network does not need any of the remaining BBSLIST.x files. 
In a large network, this file functions as a time/date      
stamp and will normally be two bytes long.  If you did      
not get a file like this with your network data files and   
if things are not functioning properly, you may need to     
create this file.  All that is necessary is to create a     
file name of BBSLIST.NET and put a single space inside of   
it and save it.                                             
                                                            
   BBSLIST.0 - This contains the numbers of valid groups in 
the network.  It will look like an N*.NET file, sort of.    
All systems in the network will have a copy of this file.   
Let us say that a particular network has groups 1,2,3,      
and 60.  In that event, the BBSLIST.0 file would appear     
as follows:                                                 
                                                            
  ~754648789   A number such as the one given would appear  
               on the first line following a tilde.  This   
               number is a time/date stamp and will change  
               from time to time.                           
  :A           This lets the software know that the infor-  
               mation for each group will be found in       
               separate files rather than in the            
               BBSLIST.NET and CONNECT.NET.                 
  1                                                         
  2                                                         
  3                                                         
  60           Observe that the group numbers are shown one 
               per line.                                    
                                                            
  BBSLIST.xxx - This file will have a number in the place of
                xxx.  The number will be the group number   
                and the file will have all of the           
                BBSLIST.NET entries for that group.  All    
                systems will have a BBSLIST.1-255 for all   
                groups listed in BBSLIST.0.  However, the   
                information in the file will pertain only   
                to that group.  You may note, at times,     
                information in your network logs regarding  
                bbslists ending in 5xx.  Depending upon the 
                type of software being used by your network 
                for updates, these probably indicate that a 
                "partial" update was received and           
                processed.  Normally after processing these 
                files (the BBSLIST.5xx and CONNECT.5xx) are 
                removed from the hard disk.                 
                                                            
  CONNECT.NET -- For small networks, this file will reflect 
                 the connections of all nodes in the        
                 network.  For a large network, this will   
                 be a time/date stamp type file similar to  
                 that discussed for the BBSLIST.NET.  If    
                 things do not work right and the           
                 CONNECT.NET file is missing, try creating  
                 it with a space inside.                    
                                                            
  CONNECT.0 - This file will exist on all systems for a     
              large network and will show  connections      
              between systems in different groups.  For     
              example, if area codes 512 and 502 are part   
              of the same group (group 4), a connection     
              between boards in those groups is not between 
              groups, even though it is long distance, and  
              the connection would not be shown in the      
              connect.0 file (it would be shown in the      
              connect.4 file).  However, a connection       
              between 512 and 213 which are in different    
              groups would be shown in the connect.0 file.  
              Note that systems with connections listed     
              in the connect.0 file will almost certainly   
              also have connections listed in their local   
              (group) connection file also.  Some networks  
              refer to groups as zones or regions so be     
              alert for this difference in terminology      
              in the respective network policy documents.   
                                                            
                                                            
   CONNECT.xxx - This file will exist on all systems and    
                 will show connections between systems in   
                 that group.  This will not show connec-    
                 tions to systems in other groups.          
                                                            
     If your connection within the group will be calling    
you, then you need only wait until you receive the files.   
Thus, once this update arrives at the board which will be   
calling you, that board will callout to you and you will    
receive the necessary files.  One exception to this is that 
some smaller networks use a different method of sending     
network updates.  If you are on a small, private network,   
then you should check with your network administrator       
regarding what you should do (if anything) in order to      
receive updates.                                            
                                                            
  If you are to call the other board (and it does not call  
you), then you will need to keep in touch with that sysop   
so that you have an idea of when the network update comes   
in.  If you obtain new network files via a download or some 
process other than receiving them through the network as an 
update, then you may need to force the network software to  
do an analysis.  This may be done by using the following    
command at the DOS level.  (Note: if you are on more than   
one network, you may need to use "dot commands" as          
discussed in the appendix.                                  
                                                            
      NETWORK3                                              
                                                            
That will run NETWORK3.EXE which analyzes your BBSLIST,     
CONNECT, and CALLOUT.NET files.  If you add a Y after the   
command (ie space Y) then the network will send you a form  
letter as feedback letting you know the results of the      
analysis and sometimes identifying problems with your       
setup.                                                      
                                                            
     Although it is natural for you to want to begin to     
subscribe to subs and so forth, you should exercise         
patience until you are 'officially' in the network.  If     
you order subs before your board is official, then your     
system will show up as "unknown" and the mail will not      
reach you.  Since many hosts of subs like to send new       
subscribers the rules regarding posting on that sub, the    
fact that you are an unknown system may result in a delay   
in your receiving the sub.  If you wait until you are       
officially in the network, then these problems are          
avoided.                                                    
                                                            
   If you are joining more than one network, it is          
important that you establish these connections ONE AT A     
TIME.  The reason for this is simply that if you have       
several CALLOUT.NET files that have not established         
passwords and so forth for your connections, it is          
possible to have the passwords get confused (ie an          
incorrect association between network and password          
established).  This may be avoided if you proceed in        
an orderly fashion and add one network at a time.           
                                                            
ÚÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄ¿                   
³Information Needed for BBSLIST listings³                   
ÀÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÙ                   
  Your Board Name -- exactly as you want it to appear in    
the Network.  You may wish to peruse a current listing of   
boards on the network in order to select a name that is     
unique.                                                     
                                                            
  Your telephone  -- this should include both area code and 
complete number.                                            
                                                            
  Maximum Baud -- this should be the maximum baud rate that 
you can support.  If you are using a high speed modem       
capable of more than 2400 bps then you should indicate the  
maximum throughput for your modem in modem-to-modem         
exchanges.                                                  
                                                            
                                                            
  Some networks will also want either your registration     
number (if you are registered).  That information may (or   
may not) be reported in brackets in the BBSLIST             
information.                                                
                                                            
  The information above will be included in the BBSLIST.XXX 
for your group along with a group identification number.    
In that listing, some networks identify area coordinators   
(AC's) by a ^ next to the telephone number.  Group or Zone  
Coordinators are often identified with a %.                 
                                                            
FIDONET INSTALLATION                                        
                                                            
     Beginning with Net34 and v4.24 of the WWIV BBS         
software, sysops may be FidoNet compatible if they chose to 
do be.  Thirdparty add-ons are required to interface with
FidoNet networks.  Installation instructions are included
with those non WSS products

PPP PROJECT INSTALLATION

  In 1997, a group of sysops headed by Frank Reid developed
a freeware, open source add-on to allow for the transmission
of network packets via the Internet.  While WSS had some
input and influence in the development of this product, it
is not a WSS product nor is the software itself supported by
WSS.  There have been many hooks placed in both the network
software and the BBS to allow this add-on to be used to its
fullest capacity.  See the PPP Project documentation for
installation and operational instructions.
                                                            

7.  USING THE NETWORK
======================================================
                                                            
   Using the network is relatively simple.  Sending         
netmail, subscribing to network subs and hosting network    
subs are discussed in this section.                         

ÚÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄ¿                                           
³Sending Netmail³                                           
ÀÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÙ                                           
   Netmail is like email on your local system.  That is,    
users on your board may send email to one another by enter- 
ing either the name or user number of the person that the   
mail is to be sent to.  In netmail, you must also use the   
node number as part of the addressing scheme.  Suppose that 
user number 5 on your system wishes to send netmail to      
user 4 (Dr. Seuss) at 4000.  In that case, the netmail could
be addressed as follows:                                    
                                                            
       4 @4000                                              
        -or-                                                
       Dr Seuss @4000                                       
                                                            
Please note that this is merely an example; there is no     
user named DR SEUSS @4000.  If the BBS is using NET32 or    
later and v4.22 or later, and that board is on multiple     
networks, the software will provide a listing of choices if 
the node number given is not unique (ie exists on more than 
one network to which the board is a member.)                
                                                            
     Such mail may be sent by the user in one of several    
ways. The user could simply use the E option to send email  
and then address it properly.  The user might use the A     
response to send a private message to someone who has       
posted on a national message base, or the user might use    
either the A or S to respond to a message received          
privately from another system.  Any of these methods will   
result in netmail being sent to another system.             
                                                            
   Mail may also be sent from one WWIV-based NetWork to     
another by using the following type of addressing:          
                                                            
NETWORK NAME #UserNumber AT NodeNumber @XXXX where XXXX     
is the gateway node number.  For example to send mail from  
WWIVLink to user #1 at node number 1 on WWIVnet, the mail   
would be addressed as follows:                              
                                                            
WWIVNET #1 AT 1 @4000                                       
                                                            
That is just an example.  Any node that is running the      
NET32 software can function as a gateway node provided that 
it has connections in both networks.  Addressing gateway    
mail by name is also permissable.  For example, to address  
Wayne Bell by name in the previous example, you would use:  
                                                            
WWIVNET RANDOM AT 1 @4000                                   
For those who care, Random is Wayne Bell's handle.          
                                                            
ÚÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄ¿                               
³Subscribing to a Netted Sub³                               
ÀÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÙ                               
   The method of subscribing to a networked message base    
depends upon the version of NETxx that you are using.  To   
subscribe to a message base hosted by another system (i.e., 
a netted sub) while using NET30 or earlier, there are 3     
things which you must do.  First, you should send netmail   
to the host of the sub requesting that she place you on     
the distribution list for that sub.  It is a good idea to   
name the sub and sub-type in that letter as many people     
host more than one netted sub and it will prevent them from 
getting confused.  Second (for versions prior to NET32),    
you should enter your DATA directory and create a file.     
The name of the file should be NNsub-type.NET and it        
                                                            
should have the host's node number in it.  Although you     
can do this with an ascii text editor, it may be easiest    
to do this from the DOS level with the copy con command.    
To accomplish this, type in the following (note information 
beginning with -- is commentary and should not be typed)    
assuming that you are subscribing to  the WWIV New Sysop's  
sub (sub-type 22050; hosted by 2050):                       
                                                            
                                                            
  copy con NN22050.NET   --followed by an ENTER or          
                           RETURN                           
  2050 F6                --the F6 means press Function key  
                         6 or you can hold control down     
                         and press Z.                       
                                                            
    A successful result will result in the message "One     
file copied" being seen on your screen.  Please be sure to  
put two N's in the NNxxxx.net file.  One N is used for a    
host system, so if you put a file  with one N into your     
data directory, it will result in messages being doubled,   
most disconcerting to the host and other systems which      
subscribe to that sub.                                      
                                                            
    Starting with NET29, it was possible to auto-request a  
sub.  This meant that if the sysop had listed the sub in a  
file called ALLOW.NET in DATA, then the subscriber/sysop    
could automatically request the sub.                        
                                                            
    This method has been further refined under NET32        
and v4.22 of WWIV so that the ALLOW.NET is not used and the 
NNALL.NET is not used either.  SUBS.XTR contains all of the 
pertinent information regarding the sub and the networks    
that it is on.                                              
                                                            
   The third step is to either use B (for boardedit) when   
you are at  W-F-C or type //boardedit when you are logged   
onto your BBS and then set up the message base.  Be sure    
to indicate the sub-type number in the option for that:     
Completed result for the New Sysop's Sub might look like    
the following under v4.22 :                                 
                                                            
                                                            
  A. Name       : WWIV New Sysop's Forum                    
  B. Filename   : NEWSYS                                    
  C. Key        : None                                      
  D. Read SL    : 60                                        
  E. Post SL    : 60                                        
  F. Anony      : No.                                       
  G. Min. Age   : 0                                         
  H. Max Msgs   : 50                                        
  I. AR         : C                                         
  J. Net Info   :                                           
         Network     Type   Host    Flags                   
      a) WWIVnet     22050  4000                            
  K. Storage typ: 2                                         
  L. NetValidate:  No                                       
  M. Require Ansi:  No                                      
  N. Disable Tag:  No                                       
  O. Description:  WWIV New Sysop's Forum for Help & Advice 
                                                            
    Since the host of New Sysop's Forum permits visiting    
sysops to read and post and since the sysop of this board   
assigns an SL of 60 and an AR of C to visiting WWIV sysops, 
he can be sure that the host's requirements are met.        
                                                            
    Although you are not required to do so, it is a good    
idea to send a short thank you or other acknowledgement to  
the host to let him know when you begin to successfully     
receive messages on the sub.  If the host has special rules 
and regulations that you need to inform your users of, you  
may do this in several ways.  You could include such        
information in a form message (i.e., a message named        
FORMxx.MSG where the xx may be either integers or letters)  
which you send to all users.  You also might make the first 
message on the message base contain the rules and then make 
it a permanent message.  If you choose this form, be sure   
to make such a message before you get hooked up to receive  
the messages, else your message will go out on the network. 
Finally, you could put a synopsis of special rules in the   
GFILES area and direct your users to read that.             
ÚÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄ¿                                      
³Hosting a Netted Sub³                                      
ÀÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÙ                                      
     As part of some networks, you will receive SUBS.LST, a 
listing to be found in your network DATA directory regarding
the various networked subs that are available for you to    
subscribe to.  At some point, you may wish to host a netted 
sub yourself.  If you do, you should first make sure that   
there is not another sub already out there serving the same 
need.  If there is, then you should only host a sub on the  
same topic because you think that you can do it better or   
because yours will have a special slant. On the other hand, 
you may have expertise in an area or information on a       
subject which is not being currently addressed on your      
network and for which you think that there might be a       
demand.  In that case, you could decide to host such a sub. 
                                                            
   To host a sub, you must create an Nsub-type.NET file in  
DATA and in it, you should keep a list of the systems which 
subscribe.  The list may be vertical or horizontal as long  
as there is a space between numbers when they are placed    
horizontally.  Personally, I recommend a vertical listing   
from lowest to highest; that way you can easily tell when a 
sub has already subscribed.                                 
                                                            
    Because telephone companies are changing the tradition  
method of numbering areas codes in 1995, the use of numeric 
sub-types will certainly decrease.  Each network will have  
its own policy with respect to whether or not numeric       
subtypes can be used and if so under what circumstances.    
The documentation here, will illustrate sub-by-name rather  
than a numeric subtype.                                     
                                                            
    Net32 and V4.22 of WWIV support a Sub-by-Name concept   
which means that you may use any legal 6 letters or         
characters as a SubType.  This numbering convention will    
enable boards to handle more subs than was possible before  
under the sub-as-integer concept.  NOTE that future changes 
(see Section 10 Future Directions) may effectively          
necesitate your being able to use the sub-by-name approach. 
Thus if you have not upgraded your WWIV version, you should 
give some thought to doing so soon.                         
                                                            
    You may want to develop a form message to send to those 
sysops who subscribe to your sub.  Such a message should    
remind them of the name, sub-type, and host and it should   
provide any rules that you may have regarding who may       
access the sub or who may read/post there.  Also you        
should get in the habit of reading your mail regularly and  
responding quickly to requests for the sub.  If you have    
indicated (under NET32 and version 4.22) that the sub may   
be auto-requested, then if you have a file called           
SA......NET in GFILES, and if the dots are replaced with    
either the subtype number of the first 6 letters of the     
sub-by-name, then that letter will automatically be sent    
to those who subscribe to the sub with the autorequest      
function.                                                   
                                                            
    You may wish to advertise your sub.  There are some     
National netted subs which have been developed just for     
that purpose and you should use them if you can.            
                                                            
    The host has the right to run his sub as he sees fit    
and may establish any rules he wishes.  The only            
restriction on sub topics is that they be legal.  If a host 
chooses to 'throw' someone off of a sub,   the individual   
has no recourse.  Of course someone may start her own sub   
if she wishes.  These rules are followed on most networks,  
however, you should refer to the documentation for the      
particular networks you are a member of to see if that net- 
work has different rules for sub hosts.                     
                                                            
   WWIV v4.12 and following introduced a feature known as   
Net Validation.  This feature may be toggled on or off in   
BOARDEDIT.  When it is toggled on, messages will not leave  
your system until they have been validated.  A host, when   
reading new messages on a sub, may press X to prevent a     
message from being sent out.  After reading the messages,   
she will be asked, "Net Validate these Messages?"  A Y      
response will result in all messages being sent out except  
those where an X was pressed.  After all messages have been 
read, pressing X will cause them to be sent again.          
NOTE: This should not be done for it may result in sending  
out duplicate messages across the network.                  
                                                            
8.  NETWORK FILES
======================================================

     The files discussed below are the Network executable
files which should be placed in the same directory as your  
BBS.EXE file.  The files which belong in your DATA          
directory are discussed in the next section.                
                                                            
  1)   NETWORK.EXE - This file is run when a BBS is calling 
another board through the network.  This program handles the
modem and the network security.                             

  2)   NETWORKF.EXE -  This is a FOSSIL based version of
NETWORK.EXE.  If you are running WWIV v4.30 or later or have
a FOSSIL driver installed, delete NETWORK.EXE and rename this
file to NETWORK.EXE
                                                            
  3)   NETWORK1.EXE - This program analyzes P*.NET files to
determine which are for local distribution and which are to 
be sent to boards that you connect with.  The latter files  
will be stored in DATA in Sxxxx.NET files where xxxx is the 
node number of the receiving board, or in Zxxxx.NET files   
if the packet is compressed.                                
                                                            
  4)   NETWORK2.EXE - This program analyzes local mail and
distributes it to the proper message sub or to email.       
                                                            
  5)   NETWORK3.EXE - This program analyzes CONNECT.NET and
BBSLIST.NET. The analysis may cause the network software to 
leave you messages.  The sysop should read these messages   
and respond to them ASAP.  These messages are discussed in  
the Appendix.

                                                            
  6)   LNET.EXE - This program allows the deletion of
corrupted messages prior to their being sent over the net-  
work.  It can also be used to delete a message which the    
Sysop does not want to go out over the network....such as   
one which violates the spirit or rules of a Sub.  As a      
general rule, a Sysop should not use LNET to read outgoing  
messages.  One exception to this is to use LNET to read     
the messages in DEAD.NET.  LNET cannot read mail in packets 
which have been compressed.                                 
                                                            
   DEAD.NET is a file to be found in DATA for messages      
that could not be delivered because the system and/or       
routing was in error.  The header for these messages in     
DEAD.NET indicates the systems which it is for and the      
number of days since it was written.  Sometimes messages    
go there because a new board has not gotten set up yet; but 
often they go there because one or more of the destination  
boards have gone down.  If these messages are several weeks 
old, there is probably no harm in deleting the DEAD.NET.    
                                                            
  7)   DExxx.EXE - These programs authenticate updates
received from the network or group coordinator.  These files
are not used by all networks and are network specific.  If
you are on several networks, put these files in the network 
data directory for each separate network or consult your network
documentation for installation instructions.
                                                            
  8)   NETINIT.C - This file needs to be used only if you   
have registered WWIV and have modified the structure or     
size of the userrec structure.  If you have modified it,    
compile and run NETINIT and it will store information       
necessary for the network in the CONFIG.DAT file.           
                                                            
  9)   REQ.EXE - This file is provided to allow those       
systems that do not run WWIV BBS software a means of auto-  
requesting subs.                                            
                                                            
  Additional files may be added to the network as the       
development progresses or some of the existing files may be 
changed and/or eliminated.                                  
                                                            
ÚÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄ¿                      
³Files in your Network Data Directory³                      
ÀÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÙ                      
    The files that belong in your network data directory    
will vary somewhat from network to network depending upon   
whether the "large" or "small" form or file organization is 
being used and upon whether or not the network employs      
group or zone coordinators who send out updates.  As        
mentioned earlier, those executables (like DEx.EXE type     
files) belong in the network data directory.                
                                                            
   In addition, the BBSLIST.NET and possibly BBSLIST.1,     
BBSLIST.2, etc., the CONNECT.NET and possibly CONNECT.1,    
CONNECT.2, etc. and the CALLOUT.NET files must be present   
in order for the network to function properly.  When the    
network analysis is performed by NETWORK3.EXE, additional   
binary data files will be created such as CONTACT.NET,      
BBSDATA.*, etc.                                             
   You may also find FBACKHDR.NET (an information file      
distributed by the net coordinator for the network),        
SUBS.LST and perhaps SUBS.1, SUBS.2, etc which provide      
information on the subs available in the network.           
CATEG.NET, an information file that permits sub hosts to    
categorize their subs so that they automatically show up    
in SUBS.LST according to the proper category.               
NETWORKS.LST, a file showing the various WWIV networks and  
whom to contact for additional information on that network  
as well as information on the coordinator of that list so   
that persons creating a network will know whom to contact   
to get their network on the listing.                        
                                                            
                                                            
"Dot Commands"                                              
                                                            
    Beginning with NET32, it is possible to use "dot        
commands" when it is desireable to force a network          
executable to work with a specific network.  If no "dot     
command" is used, the program defaults to using the network 
executable with data in the DATA directory.  On the         
other hand, if you are on more than one network, Option N   
in wwivconfig will create a file called NETWORKS.DAT in the DATA  
directory.  Dot commands work by using data from the        
networks in the order listed in the NETWORKS.DAT file which 
is the same order that you see when you use option N in     
wwivconfig.  The first network listed is associated with .0; the  
second with .1, etc.                                        
                                                            
   For example, to force LNET to run on the DEAD.NET file   
in the second network listed, you would use LNET .1.  To    
force a network analysis on the third network listed, you   
would use NETWORK3 Y .2.  Under NET31, it was necessary to  
set environmental variables to make these commands work.    
These environmental variables are no longer needed under    
NET32 and should NOT be used.
                               
9. STARTING YOUR OWN NETWORK by Jim Nunn, Former NC of IceNET
======================================================

ÚÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄ¿
³A BASIC COST-FACTOR WWIV NETWORK ³                         
ÀÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÄÙ                         
                                                            
The following will describe a basic two node WWIV network.  
The steps involved are recruiting another node, creating    
the nodelist files which are common to all systems in your  
network, creating unique callout.net files for each node    
in your network (usually done by each sysop), adding the    
network information in section N of wwivconfig, adding the        
networking software to both boards, analyzing the network   
(automatically done by WWIV or can be manually done), and   
making a network connection via modem to the other node.    
                                                            
First of all, you need to find ONE other system willing to  
join your network. Once this recruitment task is complete,  
you need to create two network files:                       
                                                            
   CONNECT.NET                                              
   ~~~~~~~~~~~                                              
     @1  2=0.00                                             
     @2  1=0.00                                             
                                                            
     BBSLIST.NET                                            
     ~~~~~~~~~~~                                            
     @1   &  *111-111-1111 #2400  "@1's BBS"                
     @2      *222-222-2222 #2400  "@2's BBS"                
                                                            
Each node has both these files in their network data        
directories.  To establish the network data directory, go   
into wwivconfig, section N, and add in the information as         
requested in the menu there (Network Name, node number,     
data directory).                                            
                                                            
Each node creates their own CALLOUT.NET file, which goes    
in the network data directory, thusly:                      
                                                            
     For @1:                                                
     CALLOUT.NET                                            
     ~~~~~~~~~~~                                            
     @2                                                     
                                                            
     For @2                                                 
     CALLOUT.NET                                            
     ~~~~~~~~~~~                                            
     @1                                                     
                                                            
                                                            
You'll both need to unzip NET33 into your main BBS          
directory.  The files required are the 4 basic networking   
files, NETWORK.EXE, NETWORK1.EXE, NETWORK2.EXE, and         
NETWORK3.EXE.                                               
                                                            
When you start the bbs with all these files properly        
installed, WWIV will automatically perform a network        
analysis.  If you have done everything right, you'll        
receive feedback email from your network, and at the        
bottom, you'll see the message "Everything is fine".        
                                                            
With these basic steps done, email the other node in the    
network, then sit back and watch as WWIV will automatically 
callout to the other system within two minutes or so.  Upon 
making the first connect, a password will be added to your  
callout.net file.   You now have a completely functional    
network of two systems.                                     
                                                            
     OTHER CONSIDERATIONS                                   
     ~~~~~~~~~~~~~~~~~~~~                                   
The basic network above is called a 'cost factored'         
network.  You'll notice network cost factors after each     
node number in a connect line in the CONNECT.NET file       
(e.g. 1=0.00).  These cost factors are taken into account   
by the networking software to determine routing of email.   
It really won't matter in a two node network just how the   
costs are set since regardless of cost, you can only send   
mail to one other node. However, by setting a cost factor   
on one node higher than another, mail will be routed via    
the node with the lower cost factor where that node has     
multiple network connects.                                  
                                                            
By now, you may be wondering why there's no mention of the  
more familiar bbslist.0, bbslist.1, bbslist.2, etc type     
files you have seen in WWIVnet, WWIVlink, IceNET, etc.      
These networks have enough systems in them that the         
networking administration task has been split up into       
groups, so that several network administrators are          
responsible for updating the files, rather than having      
one person do it all.                                       
                                                            
However, it's awkward to use the multiple bbslist/          
onnect files for a small network.  WWIVnet started using    
them when the network grew to around 575 nodes or so,       
IceNET at about 400, and WWIVlink at about 550.  Up til     
your network is in that range, you'll find it much easier   
to edit only two files instead of the larger number in the  
group based network.  Once your bbslist gets to around      
20-25k or so, you need to begin thinking about switching to 
the group approach.                                         
                                                            
     STARTING YOUR OWN WWIV NETWORK                         
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~                          
I am frequently asked questions about how to start and run  
a network. With the multi-networking capabilities of        
WWIV421a+, many of you have thought about how much fun it   
would be to have that '1@1' designation by your name.  Let  
me assure you, it is INDEED fun. However, when I started    
IceNET, along with a few of my friends, there really were   
no other major networks besides WWIVnet and WWIVlink, and   
IceNET found it's niche because it is something new and     
different, with a personality of it's own.                  
                                                            
So, how DO you start a network today? It's simple. Get one  
other board to join with you, and you have a two system     
network, as described above. But if your serious about it,  
then I think you should consider several things:            
                                                            
     1 - What is the PURPOSE of the network I'm going       
         to start?                                          
                                                            
         Your network should have a THEME and a PURPOSE.    
                                                            
     2 - Your network should have a POLICY and GUIDELINES   
         for operation.                                     
                                                            
         A policy is a way of acting, or proceding; a       
         course.                                            
                                                            
     3 - How do I send out network updates?                 
                                                            
         To keep your network running smoothly, each system 
         must be using the same nodelists. As the network   
         grows, you will need to distribute the new files   
         to each system in a timely and efficient manner.   
                                                            
     YOUR NETWORK THEME                                     
     ~~~~~~~~~~~~~~~~~~                                     
Think of this just like you would think of hosting a        
message base, but in this case, you are 'hosting' and       
entire network of systems. Everything that goes on in your  
network doesn't necessarily have to involve the theme; but  
your theme and purpose is the foundation. The theme         
provides a special focus for your network, and new systems  
interested in your theme will be attracted.                 
                                                            
     YOUR NETWORK POLICY                                    
     ~~~~~~~~~~~~~~~~~~~                                    
The policy you establish will be the reference source for   
dealing with problems and issues as they arise in your      
network. When something is wrong, you should be able to     
look in the policy to get some answers about how to         
proceed to resolve the problem. You don't have to re-invent 
the wheel to write a good policy.  Look for the basics in   
the WWIVNET guidelines, which contain sound practices which 
have been demonstrated to work quite well. I believe that a 
short, elegant, well thought out policy can put your        
network on a firm footing right from the beginning.         
Involve others in the preparation of your policy, then      
establish, maintain, and enforce your policy.               
                                                            
                                                            
     A TECHNICAL MATTER - UPDATING THE NETWORK              
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~              
As your network grows, you will need to edit the            
connect.net and bbslist.net files for new systems, remove   
systems that drop out, connection changes, and numerous     
other things that systems within your network will want     
changed.                                                    
                                                            
One big question then, is how to get these edited files     
distributed to all systems in the network. There are at     
least three methods to do this:                             
                                                            
     1 - The email method.                                  
                                                            
     2 - The message base method.                           
                                                            
     3 - Using Wayne Bell's NETUP program, or one of        
         several NETUP clones.                              
                                                            
                                                            
     THE EMAIL METHOD                                       
     ~~~~~~~~~~~~~~~~                                       
In the beginning, with only a few systems, you can update   
your network easily via email, or by just making the files  
available for download from your system.  This method is    
probably adequate up to about 25 systems.  If your network  
grows beyond this size, you will begin to find problems:    
                                                            
  o    Some sysops just don't get around to installing the  
       files                                                
  o    Unknown systems will begin to show up in email and   
       message bases on BBS's where the sysop has not       
       updated his board with the new files.                
                                                            
     THE MESSAGE BASE METHOD                                
     ~~~~~~~~~~~~~~~~~~~~~~~                                
One semi-automatic method of updating the network, that     
will work well for up to about 50-75 systems, is to use a   
special update message base.  This message base would be    
hosted by you, and you would network validate the message   
base.  On all subscribing systems (everyone in the network  
must subscribe), the message base would be set to ONE       
message, storage type 0.                                    
                                                            
To update your network, zip up the bbslist.net and          
connect.net files into one file (called, for example        
NODELIST.ZIP), then uuencode that file.  Post the uuencoded 
message on the message base.  All subscribing systems would 
then have a batch file to run during maintenance, something 
like this:                                                  
                                                            
     COPY C:\WWIV\MSGS\*. UPDATE.UUE                        
     UUDECODE C:\WWIV\MSGS\UPDATE.UUE                       
     PKUNZIP -o C:\WWIV\MSGS\NODELIST C:\WWIV\DATA          
     ERASE C:\WWIV\MSGS\*.                                  
     ERASE C:\WWIV\MSGS\*.UUE                               
     ERASE C:\WWIV\MSGS\*.ZIP                               
                                                            
As soon as WWIV recognizes the changes, network analysis    
will automatically run, sending the sysop feedback as       
normal.                                                     
                                                            
It is critical that the message base be ONLY one message,   
and that there are NO other files without extensions in     
\MSGS, which is normally the case. Make sure you delete     
any *. files from \MSGS just to make sure when initially    
setting up this method.                                     
                                                            
I'm certain that some of you will see ways to make this     
method more efficient, but the above should give you the    
concept.  Of course, if you're capable, you could write     
special software to accomplish the updates, but the         
above method is something that anyone can easily do, it's   
relatively secure, since you host the message base and      
validate it, and it requires no further sysop intervention  
once the message base and batch file is installed.          
                                                            
     USING NETUP                                            
     ~~~~~~~~~~                                             
                                                            
When IceNET grew to about 75 systems, I realized that       
something must be done to improve the updating technique.   
We had gone though the stages of using email, a message     
base, and even had ICENETUD, a special program written by   
Icefreezr, IceNET 3@1 (Alan Carauna) that worked with a     
message base somewhat similar to the way Space Dynasty      
works.                                                      
                                                            
From a suggestion by DEATH KNIGHT, IceNET 1@7, I emailed    
Wayne Bell, telling him 'IceNET needs your help', to which  
he graciously responded to by offering me NETUP for $300.   
When you buy NETUP, you get three files, the NETUP.EXE,     
and two special files DE1.EXE and EN1.EXE.  As the Network  
Coordinator for your network, only YOU have EN1.EXE on your 
system, and all other systems have the special DE1.EXE      
(this file goes into the special DATA directory you set up  
in WWIV421A+ just for your network).                        
                                                            
When you execute NETUP.EXE, you will see the following menu 
on your system.  Just hit the letter, and the rest is       
automatic.                                                  
                                                            
                                                            
     Found:     22 AC's    278 systems                      
     Using standard BBSLIST.NET and CONNECT.NET files.      
     B> Send BBSLIST.NET to network                         
     C> Send CONNECT.NET to network                         
     H> Send FBACKHDR                                       
     N> Send WWIVnews                                       
     F> Send feedback                                       
     R> Check registration info                             
     Q> Quit                                                
     Which?                                                 
                                                            
                                                            
For normal updates, I just type in NETUP B C, and don't     
even have to use the menu.  Recently, in order to have the  
updating more uniform, I've begun running NETUP in a batch  
file during maintenance, which runs every other day.  With  
the rapid growth of IceNET in recent times, this frequency  
of network updates is required.                             
                                                            
If you are going to run a WWIV network, you will not find a 
better resource than Wayne Bell to help you with your       
software needs for updating your network. As usual with     
Wayne's policy, once you've registered NETUP, he will be    
there for you to answer questions and provide updates to    
NETUP as they are released.                                 
                                                            
In conclusion, if you want to start a network, then do it   
right.  Work with others to establish your THEME, POLICY,   
and GUIDELINES.  Use the methods above to begin updating    
your network. If you a lucky, and have a lot of friends to  
help you like I did, one day you probably will buy NETUP,   
as your network will have grown to the point it's a         
necessity.                                                  
                                                            
I'd like to thank all of the sysops who are in IceNET, and  
in effect, allow me to be a 1@1 for a premium network. I'd  
also like to thank Wayne Bell, and Filo for all their       
support in so many ways.                                    
                                                            
Running a network is a lot of work and responsibility.      
It's also a tremendous amount of fun. I'm having the time   
of my life!                                                 
                                                            
If you have any questions or there is something I can help  
you with in starting your network, feel free to email me,   
Jim, 1@1, IceNET :).  If you haven't yet joined IceNET, let 
me know and I'll send you an application, which also        
includes the IceNET Policy Statement. As a member of        
IceNET, you can see how we do things by your participation  
on the IceNET Sysop's Only sub, or the IceNET Guidelines    
Formation Committee sub. Your users will also gain access   
to a wide variety of IceNET message bases.                  
                                                            
Happy Networking!                                           
                                                            
   Jim 1@1 IceNET, August 1993                              
                                                            

10.  TROUBLE-SHOOTING NETWORK CONNECTIONS
======================================================
                                                            
       Utilizing the NETWORK is really very simple.  If you 
have tried everything you can think of to remedy a problem  
and are unable to do so, contact one of the Sysops of a     
SUPPORT Board and enlist aid.  Sometimes there are problems
with the code and/or its compatibility with different       
modems; however, those type of problems can only be         
addressed after all other avenues have been thoroughly      
explored, and even then that may not be the solution.  For  
example, many WWIV Sysops have registered the WWIV          
software, obtained the source code and made extensive       
modifications to the BBS.EXE.  In that event, it may be a   
modification that is causing the problem rather than the    
network software.                                           
                                                            
    When seeking help, be prepared to provide information   
on your system, your modem, the error messages you get and  
so forth.  Debugging network problems is usually a process  
of eliminating the various possible sources of problems one 
by one.  Any information which you can provide to speed     
this process makes it easier on all concerned.              
                                                            
    A few common problems, and their solutions, are describ-
ed next.                                                    
                                                            
You force callout and the cursor returns to WFC             
===============================================             
                                                            
    First, be sure that you are attempting to force the     
call during any agreed upon hours.  If it is not during     
the agreed upon hours, the network software will prompt     
you "Are you sure?"  An affirmative response will allow the 
call to proceed.  If the call does not connect, you should  
double check the CALLOUT.NET, CONNECT.0, and BBSLIST.x to   
be sure that no typographical errors were made.  Zeros can- 
not be o's, group designators must be correct, etc.         
                                                            
    Also, under Net20 and later you should ensure that all  
files in your network dATA directory are correct as they    
affect your board and the board that you connect with.  For 
example, a failure to show your connection will cause an    
error.                                                      
                                                            
    If no typographical errors were made, run network3.exe  
from DOS level and force a reanalysis.  If after doing all  
of these things, the board will still not call out, go to   
your network data and delete BBSDATA.NET, BBSDATA.IND, and  
BBSDATA.ROU as well as CONTACT.NET and rerun the NETWORK3   
program which will force the reestablishment of the deleted 
files.  This will often cure the problem.  If it does not,  
first check your NETDAT0.LOG in GFILES to see if it         
provides any clue as to the nature of the problem.  If not, 
you should then contact one of the support boards and       
explain your problem in full detail.   The command line     
NETWORK3 Y will force local feedback to be sent to you from 
the network software.  The resulting information may be     
useful in determining problems in your network setup.       
                                                            
Your board calls out and gets a "Bad PW" message            
===============================================             
   The "Bad Password" message will show up in your net log  
which is readable from WFC by pressing N.  If that is the   
case and a successful connection has never been made, then  
the remote sysop should ascertain that the CALLOUT.NET is   
correct.  If so, then check the CONNECT.x and BBSLIST.x.    
If a successful connection has been made in the past and a  
password between the two boards has been established, then  
try again as line noise may be the culprit.  If the "Wrong  
Password" persists over several tries, then it is possible  
that a file has become corrupted.  In this event, both you  
and the remote sysop need to delete the password which was  
generated by the network and let the net software           
reestablish the password.  If you have never successfully   
connected with the other board, then the error may be due   
to the other sysop's not having setup for the connection.   
You should contact him and ascertain whether or not the     
connection if reflected in his CONNECT.xxx file or          
CALLOUT.NET file.  It may also be that a faulty connection  
caused his board to create a password whereas yours did     
not.                                                        
                                                            
Your board calls and gets a "NO NET" message                
============================================                
    This occurs when an unsuccessful connection occurred.   
Often it is only because the other board is busy.  The      
remedy is to try again.  If the board is a new board and    
you know it is not busy, then both you and the other sysop  
should make certain that all files are in the proper        
places.  There are several Binary files created by the      
network.  These are CONTACT.NET and BBSDATA.*. Sometimes    
these files will become corrupted and this may be the       
cause of a failure to establish a connection.  You may      
delete these two files from the DATA directory and then run 
NETWORK3.EXE again.  This re-analysis will recreate those   
two files and may cure the problem.  This problem (no net)  
may also occur when the modems have connected but are not   
recognizing each other's signal. It may be that one modem   
thinks the connection is at 14.4k whereas the other thinks  
it is at 12k or something else.                             
                                                            
                                                            
11.  FUTURE DIRECTIONS
======================================================
                                                            
    In the near future, WWIV BBS software is likely to      
include some of the following features:

    Networked File Directories - The NFD concept is
similar to message bases.  You subscribe to a NFD
and when you or one of your users select a file from
that directory, a request is sent to the host system
for that file subject to Sysop approval.

    File Transfer System - FTS is based on the FILEnet
file transfer software.  This future enhancement will
allow a network to permit the transfer of files in much
the same way as messages and email are sent today.  This
system further allows the ability to send files as
attachments to messages.

    DirectMail - Based on the FidoNet crash mail concept.
Users with a sufficient SL have the option of flagging a
message as DirectMail which will be sent directly to the
destination system (if it accepts DirectMail) upon logoff.

    Internal Packet Linking -  IPL is based on FLink by
Dennis Meyers. WSS has aquired the rights to FLink and
will be incorporating the abililty to link packets from
different networks over a single connection in a future
version of the software.
                                                            
                                                            
                                                            
Appendix A - Macro Language
======================================================
                                                            
    A macro is not normally needed for calling another BBS  
with the network software.  However, when it is needed for  
reasons discussed in the body of the documentation, then it 
should be used.  Use of a macro is indicated by using a %x  
in the CALLOUT.NET with at least one space following the    
node number and before the % sign.  The x should be an      
integer.  In the network data directory, a file called      
Mx.NET should be created which contains the macro.  The x   
should be the same integer as that used in the CALLOUT.NET. 
You may have several different macros where they are        
necessary.                                                  
                                                            
    The network macros should have one of the COMMAND words 
listed below on the left margin of the macro, followed by   
additional information within quotes following the command  
line.                                                       
                                                            
    The commands supported are listed below in alphabetical 
order.  It is common to have DEBUG as the first line of the 
macro.                                                      
                                                            
DEBUG  -- This command should start the macro and should be 
followed by an open and close quote ("").  This will cause  
results to be echoed to the screen.                         
                                                            
DIAL -- This command causes the modem to dial whatever      
number that you put there.  (For example, DIAL "631-5841"). 
You can also use two replaceable parameters with this       
command, %1 for area code and %2 for the 7 digit phone      
number shown in BBSLIST.x.                                  
                                                            
FAILURE -- This command allows you to define a failure      
condition.  Typically the failure is "BUSY".                
                                                            
PARITY -- This command allows you to set the parity at      
something other than 8N1.                                   
                                                            
SEND -- This command causes whatever is in quotation marks  
to be sent via the modem.  The information in quotes must   
end  with a left brace ({) which in the macro language      
indicates a carriage return.  You can also use the send     
command to dial the phone if yout put everything that must  
be provided to the modem (for example,                      
SEND "ATDT631-5841{" would cause the modem to dial the      
number indicated.                                           
                                                            
SETBAUD -- This command allows you to set the baud rate for 
the call.                                                   
                                                            
SPEED --  This command allows you to set the comport speed  
for the call.                                               
                                                            
SUCCESS -- This command allows you to define a success      
string.                                                     
                                                            
TIMEOUT -- This command will cause the modem to pause for   
the number of seconds indicated or until a WAITFOR          
condition has been met, whichever comes first.              
                                                            
WAIT -- This command is similar to the TIMEOUT command      
except that the modem or macro will wait the number of      
seconds indicated regardless of any following WAITFOR       
condition.                                                  
                                                            
WAITFOR -- Anything in quotes following this command will   
be the condition that the macro waits for before            
continuing.                                                 
                                                            
Additional Information on Macros is in Appendix K which is  
chapter 24 in this version of the net docs.                 


Appendix B - Macro Examples
======================================================
                                                            
    In conjunction with DIAL or SEND, you may use %1 for    
the area code and %2 for the 7 digit telephone number.  If  
you use DIAL, you do not need to use the ATDT command; but  
with SEND you need it.                                      
                                                            
   Using the simple script language contained above, you    
can develop elaborate scripts.  In our area, we have        
written scripts that logged the network onto QBBS and       
RBBS boards and selected Door programs which were WWIV      
setups which in turn ran the network.                       
                                                            
   If you have trouble developing the scripts to use for a  
particular application, you should be able to get help from 
any Support Board.  You will need a text file taken from a  
screen capture of what you are logging into.  Then the      
support board should be able to help you develop the        
appropriate script for you to use.                          
                                                            
 Dial Without Dialing 1 or area code                        
                                                            
     DEBUG ""                                               
     DIAL "%2"                                              
                                                            
Dial With a 1 but not area code                             
                                                            
     DEBUG ""                                               
     DIAL "1,%2"                                            
                                                            
Dial With a 1 and Area Code                                 
                                                            
     DEBUG ""                                               
     DIAL "1,%1,%2"                                         
                                                            
                                                            
Make a Connection, Wait a few Seconds, Send 22 for Special  
Access and then the phone number (without area code)        
                                                            
     DEBUG ""                                               
     DIAL "555-1212"            (see comments below)        
     WAIT "5"                                               
     SEND "22{"                                             
     WAIT "5"                                               
     Send "%2{"                                             
                                                            
That macro would dial a special access number (do not use   
the one shown as that is the long distance information      
service).  The macro then waits 5 seconds and sends a       
special access code (22) and waits another 5 seconds before 
sending the phone number (last 7 digits listed in CONNECT.*)
                                                            
These scripts can be very sophisticated and employ the VERBS
shown in the other section dealing with Macros.  If you     
have any problems using these, please feel free to ask a    
support board for help.  Remember that Macros should begin  
with M, be followed by a number and be placed in the network
data directory for the network that you are calling.  The   
CALLOUT.NET file is then modified to show the macro to be   
used when calling that particular board.  Consider the      
following entry for CALLOUT.NET:                            
                                                            
 @4001 %1 &&                                                
                                                            
The %1 informs the software to use M1.NET as the macro.     
                                                            
                                                            
                                                            
Appendix C - Network message types
======================================================
                                                            
   The network recognizes various types of major and        
minor type messages, and these are often reflected during   
the analysis which takes place after a network message is   
received.  The information which follows briefly explains   
each of these message types.                                
                                                            
These types may be expanded in the future.                  
                                                            
main type 1 - net info                                      
     (all type 1 msgs must be use method==1)                
     0 - feedback to sysop                                  
     1 - bbslist.net                                        
     2 - connect.net                                        
     3 - subs.lst                                           
     4 - wwivnews.net                                       
     5 - fbackhdr.net                                       
     6 - Additional wwivnews.net text                       
     7 - categ.net                                          
     8 - networks.lst                                       
     9 - Files sent from NC                                 
                                                            
                                                            
main type 2 - email                                         
     (no method requirements)                               
     minor type not used                                    
                                                            
                                                            
main type 3 - post (from host to subscriber.                
                    numeric sub types only)                 
     (no method requirements)                               
     minor type is sub type                                 
                                                            
                                                            
main type 4 - Network Files (future)
                                                            
main type 5 - pre-post (from subscriber to host.            
              numeric sub types only)                       
     (no method requirements)                               
     minor type is sub type                                 
                                                            
                                                            
main type 6 - external msgs                                 
     (no method requirements)                               
     minor type is external message type                    
                                                            
                                                            
main type 7 - email by name                                 
     (no method requirements)                               
     minor type not used                                    
     (name of destination user at start of msg text)        
                                                            
                                                            
main type 8 - net edit msgs                                 
     0  - A partial update to the BBSLIST information.      
     1  - A request for BBSLIST information to be changed.  
     2  - A partial update to the connection information.   
     3  - A request for connection information to change.   
     4  - An update to NETEDIT's registration record.       
     5  - A transmittal of the installation message.        
     6  - A request for to transmit a registration record.  
     7  - A response to request for a registration record.  
     8  - A remote request for a net analysis ("/A").       
     9  - An ASCII text response to a remote analysis.      
     10 - Network Editor E-mail and/or automatic feedback.  
     11 - A message reporting an error condition.           
     12 - A request for installation and ver information.   
     13 - A request for a remote node's ALIASES.NET file.   
     14 - A request for a node's aliases.                   
     15 - A response to the alias request.                  
                                                            
main type 9 - subs.lst                                      
     0 - subs.lst                                           
     1 - subs.1                                             
     2 - subs.2                                             
     ...                                                    
                                                            
                                                            
main type 10 - UNUSED                                       
                                                            
                                                            
main type 11 - bbslist.*                                    
     (method must be 1 or ((minor_type % 256)+256))         
 0..255   - bbslist.<minor-type>                            
          - full bbslist update NC-net                      
 257..511 - bbslist.a<minor-less-256-in-hex>                
          - full bbslist update GC-NC                       
 513..767 - bbslist.<minor-type>                            
          - partial bbslist up NC-net                       
                                                            
                                                            
main type 12 - connect.*                                    
     (method must be 1 or ((minor_type % 256)+256))         
 0..255   - bbslist.<minor-type>                            
          - full connect update NC-net                      
 257..511 - bbslist.a<minor-less-256-in-hex>                
          - full connect update GC-NC                       
                                                            
                                                            
main type 13 - unused                                       
                                                            
                                                            
main type 14 - group info (from GC)                         
     (method must be 257..511)                              
     0 - email to sysop                                     
                                                            
                                                            
main type 15 - ssm                                          
     (no method requirement)                                
     minor type unused                                      
                                                            
                                                            
main type 16 - sub add request                              
     (no method requirement)                                
     0 - sub by name, sub name first part of text           
     other - minor-type is sub-type                         
                                                            
                                                            
main type 17 - sub drop request                             
     (no method requirement)                                
     0 - sub by name, sub name first part of text           
     other - sub type is minor type                         
                                                            
                                                            
main type 18 - sub add response                             
     0 - sub by name, sub name is first part of text        
     other - sub type is minor type                         
     first byte of text (after sub name, if any) is status  
     of request                                             
                                                            
                                                            
main type 19 - sub drop response                            
     0 - sub by name, sub name is first part of text        
     other - sub type is minor type                         
     first byte of text (after sub name, if any) is status  
     of request                                             
     1 - not host                                           
     2 - not there (can't drop you)                         
                                                            
                                                            
main type 26 - post by name                                 
     (no method requirements)                               
     minor type unused                                      
     sub type is first part of msg text                     
     This is from subscriber to host, and from host to net  
                                                            
main type 27 - new external                                 
     (no method requirements)                               
     minor type is external type                            
     (see Appendix J)

main type 28 - game packs
     minor type assigned by WSS
     Used for transmitting game data
                                                            
  NOTE: all major type 1, 11, 12, and 14 messages are       
appropriately source-verified.                              
                                                            
  Information for this appendix supplied by Wayne Bell
                                                            
                                                            
                                                            
                                                            
                                                            
Appendix D - Identifiers Used in BBSLIST
======================================================

    Effective in Net37, the BBSlist identifiers have
been changed.  The previous modem type identifiers have
not been used since net34 was released.  To allow for a
more seamless operation with third party add-ons and to
provide future expanability some of the identifiers have
been changed.  It is IMPERATIVE that network coordinators
make the required changes in their respective network
files as soon as is possible to prevent network problems.
The following are the identifiers in use as of Net37:


  $ - System is PPP capable (See PPP Project Documentation)
  \ - System runs Fido frontend
  | - System is a telnet node
  < - System refuses links           (future expansion)
  > - System uses FTS/BLT system     (future expansion)
  ! - System accepts direct connects (future expansion)
  / - System is unregistered
  ? - System accepts faxes
  _ - System is a dead end node
  + - System is network server
  = - Unused

  & - Network Coordinator
  % - Group Coordinator
  ^ - Area Coordinator
  ~ - Subs Coordinator
                                                            
    The identifiers above may be stacked together.  For     
example, "$\|" would indicate the system participate in the PPP Project,
has a Fido Front End and is telnet capable.
                                                            
    The identifier for a dead-end node should not be used   
except in emergencies.  It is a means to force the network  
to treat a node that would NOT normally be a dead end node  
as if it were one in order to facilitate temporary          
re-routing of messages.                                     
                                                            
Appendix E - Private Networks
======================================================
                                                            
   The network software may be used for any legitimate      
private network as long as the user understands that the    
author is under no obligation to provide the software which 
distributes network updates and as long as the functioning  
of the private network does not interfere in any way with   
the functioning of other WWIV-based networks.  WSS
assumes no responsibility for insuring the operation of
any private networks utilizing the software.
                                                            
    Further, the WWIV support board Sysops are under no     
obligation to explain how to set up and/or operate a        
private network.  Of course, even for private networks, in  
order to continue using the WWIV network software past the  
two month trial period, you must have either registered     
WWIV, or (for BBS software that is in no way based on WWIV  
software) registered the WWIVnet software.  The NetUp package
developed and distributed by WSS and used by some networks
for updating their network files may be purchased for $100
by contacting 1@50 on most WWIV based networks or
wss@wwiv.com on the Internet.


Appendix F - Automated subboard requests
======================================================
                                                            
  Net29 and above support automated subboard subscriptions. 
In order for this to work, BOTH systems (the host and the   
subscriber) must be running Net29 or later.  The program    
'REQ.EXE' can be used to subscribe or drop subboards.       
                                                            
  There are some files associated with automated            
subscription under Net29, Net30, and Net 31:                
                                                            
  ALLOW.NET (in the DATA directory) - lists subboard types  
that are under automated control.  If you host sub type     
1701, and you want systems to be able to automatically      
subscribe to it, you would have the number 1701 in the      
ALLOW.NET file.  If a sub type is not listed in the file,   
or the file does not exist, then sysops will not be able to 
automatically subscribe to the subboard.                    
                                                            
  DISALLOW.NET (in the DATA directory) - lists system       
numbers that are NOT allowed to automatically subscribe     
/drop subboards.  If you want to keep a certain system      
from subscribing to any of your subs, place their system    
number in the DISALLOW.NET file.                            
                                                            
SA*.NET (in GFILES directory) - This is a text file that is 
sent, as part of a pseudo-email, to a sysop when they are   
added to a sub.  If you host sub 1701, then the file        
'SA1701.NET' would be appended as part of a piece of mail   
to the sysop that is subscribed to the sub.  It can give    
any rules of the sub, etc.                                  
                                                            
The DISALLOW.NET file may still be used with NET32 and      
higher.                                                     
                                                            
    SR*.NET (in GFILES directory) - If a system is not      
allowed to automatically subscribe to a sub (if the sub     
isn't listed in the ALLOW.NET, for example), then this      
piece of mail is appended to a message informing the        
sysop that he cannot be automatically added to the sub.     
The file should list why it isn't under automated control,  
and if it would be worth the effort to email the sysop      
and ask for it.  This option also works with NET32 and      
higher.                                                     
                                                            
  The REQ.EXE program is very simple to use.  You need to   
know only if you want to add or drop the subboard, the sub  
type, and the host.  You then put all this info on a        
command-line, such as:                                      
                                                            
  REQ A 1701 1                                              
                                                            
  To REQuest an Add to type 1701 hosted by @1.  To drop the 
sub, you'd say:                                             
                                                            
  REQ D 1701 1                                              
                                                            
  You should get email back from the system when you are    
automatically added/dropped from a subboard.  You will get  
no mail back, and nothing will happen, if the remote system 
isn't running net29 or later.  If you request to be added   
to a subboard that you don't have configured into your      
system (in //boardedit), then when the response comes back  
indicating you were added, the network will automatically   
request that you be dropped from the subboard (since there  
is nowhere for the  messages to go), and you will NOT get   
an indication in feedback.                                  
                                                            
Appendix G - Multi-Networking
======================================================
                                                            
     Beginning with NET31 and v4.21a of WWIV it is possible 
to network among WWIV-based networks rather easily.  The    
methodology for doing this is discussed more thoroughly in  
the documentation for WWIV v4.22.  Key things to remember   
about multi-networking:                                     
                                                            
     a)  Each network should be in its own data directory.  
     b)  Each network should be setup in wwivconfig option N      
     c)  All files unique to a network should be put in     
         that network's DATA directory.                     
     d)  Network directories should be DOS legal names.     

Appendix H - USING HS/LINK
======================================================
                                                            
  HS/Link WILL work properly on most WWIV systems using its 
DEFAULT settings (NO HSLINK.CFG file).  Put HSLINK.EXE in   
your main BBS directory. Add a caret (^) to the desired     
lines in CALLOUT.NET and have the systems you connect do    
the same (it must be present at BOTH ends). Once this is    
down, if you have 103k free when the system attempts a NET  
callout and HST protocol is NOT in use, it will use         
HS/Link for the NET transfer.                               
                                                            
  This probably will NOT work if you are using PC Pursuit.  
(see below)                                                 
                                                            
   For more information on using and optimizing HS/Link for 
WWIV, download and read WWIVHSLK.ZIP which can be found on  
most Source Distribution Systems, and many others. It may   
also appear under the filename of HSLKWWIV.ZIP              
                                                            
CURRENT HS/LINK VERSION :                                   
                                                            
   Be sure to use the LATEST release of HS/Link. While the  
current version is always compatible with older versions,   
you will not get the benefit of the latest enhancements and 
fixes if you are using an old version.                      
                                                            
LOG FILE                                                    
                                                            
  Starting with v1.13D0, HS/Link will create a logfile if   
the environment variable HSERR is defined. To create a      
logfile called HSLOG.TXT on your C drive in your Gfiles     
directory, just add this line to your autoexec.bat file.    
SET HSERR=C:\GFILES\HSLOG.TXT  HS/Link will keep appending  
to this file, so you will want to provide some means of     
erasing, renaming, and or zipping it in your nightly event. 
                                                            
 === CAUTIONS if using a CONFIG file ===                    
                                                            
DOWNLOAD DIRECTORY (-U) :                                   
                                                            
     This option controls the destination directory for     
incoming files. By default, HS/Link will put incoming files 
into the "current" directory.  This is where WWIV is        
expecting to find them. WWIV changes to the 'TEMP' direct-  
ory before receiving files. The BBS will move the files     
to where they belong, so the -U OPTION SHOULD NOT BE USED   
for the BBS.                                                
                                                            
FORCE REMOTE TO USE LOCAL OPTIONS (-!)                      
                                                            
    This option causes the remote (called) end to use some  
of the options specified by the calling end. This does NOT  
affect any of the options having to do with security, such  
as the upload path, or the overwrite option. It does affect 
block size (-s), xon/xoff (-hx), and windows (-w). NET32    
will append the -! option to the HS/Link command line for   
outgoing calls, thus forcing the remote to use these        
settings for NET transfers. Since it is not present on the  
command line for incoming NET calls, the calling system     
will be able to use the settings that are best for his      
phone lines. It SHOULD NEVER BE PRESENT IN THE CFG FILE THE 
BBS WILL BE USING!                                          
                                                            
MINIMUM BLOCKS (-nm) :                                      
                                                            
     Removes block numbers from each block, thus saving a   
few bytes. No improvement in performance has been measured. 
It's effect is similar to that of Ymodem-G, and the         
results can be catastrophic if an error does creep in. This 
option SHOULD NEVER BE USED!                                
                                                            
SLOW HANDSHAKE (-hs) :                                      
                                                            
     Sends Xoff or lowers RTS during disk I/O. This causes  
the computer to signal the modem not to send any data       
during disk I/O. It is available for systems with slow disk 
access. It may help if you get frequent CRC errors or COM   
overruns on clean lines. Be sure NOT TO DISABLE Xon/Xoff    
HANDSHAKING IF THIS OPTION IS USED.                         
                                                            
  Information for this appendix supplied by Lance Halle
                                                            
Appendix I - Symbols in SUBS.XTR
======================================================
                                                            
    You are reminded that you should not modify these       
symbols directly.  Always use BOARDEDIT when making changes 
to this file.                                               
                                                            
Meaning of symbols                                          
                                                            
    A typical entry in SUBS.XTR might look like this:       
                                                            
  !8                                                        
  @Novice & Veteran Sysops Helping Each other with WWIV     
  #0                                                        
  $WWIVnet 22050 3 0                                        
                                                            
!x  =   The number of the Sub on the board (ie the sub      
        index in BOARDEDIT.                                 
@   =   The long description for the sub (for auto-subs-    
        info)                                               
#0  =   Flags (currently not used but for future expansion) 
$NETWORK  SubType Flags  Host Category                      
                                                            
Flags are 1 for auto-addrop, 2 for auto-info (3 for both).  
                                                            
Host is 0 if you are the host (you host it), otherwise the  
host system #.                                              
                                                            
Category will be an option that will permit the sysop to    
self-classify a sub according to pre-defined categories,    
thus facilitating the maintenance of network wide SUBS.LST  
type files.  The categories will be listed in CATEG.NET     
which will be found in the network data directory.          
                                                            
                                                            
Appendix J - External Message Interface
======================================================
                                                            
   Net33 (and later versions) will include a method whereby 
messages for external programs can be transferred through   
the network.  This does not describe how to read network    
data files, or how to write net packets, only how to        
integrate a program that does those things with the         
network.  (see the WWIV source code, or WWIVnet technical   
docs, for info on that.)                                    
                                                            
    All received message packets that are destined for the  
local system are stored into "LOCAL.NET" in your network    
data directory.  The network2.exe program is then run to    
process the messages.  If any messages are of the "new      
external" type (main_type_new_extern, 0x001b), then they    
may be saved for processing by an external net program.     
                                                            
                                                            
    Each external network program requires a program (.exe  
or .com, NOT .bat), which will take as parameters a         
filename of a network file (p*.net format), and a network   
number identifier (.net_num).  Each external network        
program can take as input a contiguous range of             
minor_type's.                                               
                                                            
    External network programs are described in the          
'EPROGS.NET' which (optionally) exists in the network data  
directory.  The eprogs.net file is a text file, and has a   
line describing one external net program per line.  Each    
line has three pieces of information: the program name      
(1-8 chars), the starting minor_type, and the stopping      
minor_type.  So, for example, if an external net program    
'netprog.exe' is to handle main_type 0x1b, minor types      
100-103, then the line in the eprogs.net file for that      
processor would be:                                         
                                                            
netprog 100 103                                             
                                                            
(If the program handles only one minor_type, then the       
starting and stopping minor_types should both be the same,  
and equal to the minor_type to be processed.)               
                                                            
   As local.net is processed, any main_type_new_extern      
messages encountered cause network2 to search the           
eprogs.net file to see if any external net programs are     
set up to handle that minor_type.  If none are found, the   
net message is thrown away.  If there are two or more       
programs listed to process that minor_type, only the first  
receives the message.  Net messages accepted for an         
external net program are stored to a temporary file while   
local.net has been processed.  After local.net has been     
completely processed, and deleted, network2 runs the        
external net programs, in order, passing them the           
filename of the temporary net file for that program, and    
an indication of which network is being processed.  After   
the program exits, the temporary net file is deleted.       
                                                            
   Note that it IS allowable for an external net program    
to create a p*.net file for outgoing messages, OR to put    
net messages to the local.net file which will be            
immediately re-processed by the BBS.                        
                                                            
   Please do not blindly grab minor_types.  If you need a   
lot of separate message types, the message type can be      
stored in the text part of the message and a single         
minor_type used instead.                                    
                                                            
   There are also local.net pre-processors allowed in       
net32.  The preprocessors are listed in the 'epreproc.net'  
file in the network data directory, one per line.  BEFORE   
network2 processes ANY of local.net, each preprocessor is   
run, in order, passing each the ".net_num" parameter to     
indicate which network is being processed.  The pre-        
processor may then scan through local.net, and mark as      
deleted (main_type=65535) any message processed by that     
preprocessor.  The preprocessor may even append additional  
messages to the local.net file, if that is desired.         
                                                            
                                                            
Appendix K - WSS Operational Policies
======================================================

                       WWIV Software Services LLC
                              PO Box 4468
                         Johnson City, TN 37602

Reference:  WSS Operational Policy as of: 2 January 2000

1. General:  WWIV Software Services (WSS) dictates policy for the
software under its control only and does not attempt to influence
the operation of any network in any manner.  Network policies are
dictated by the Network Coordinator (NC) or administrative body
of the individual networks.  WSS does however, reserve the right
to interpret our policy for the individual user and/or network
administrator(s).  Any question as to applicability or
interpretation of these policies should be brought to the
attention of WSS BEFORE the user or network official take any
action.  Decisions or interpretations rendered by WSS on any
issue are final.  WSS reserves the right to revise, rescind,
expand or alter the terms and conditions of this policy at any
time and may do so without notice.  Revised policy will be
grandfathered in most cases to allow no degradation of
eligibility, status, or position of the individuals it affects.

2. Distribution, Software Registration and License: WWIV BBS and
and NetXX programs are distributed under the shareware concept.
The user has 60 (sixty) days to evaluate suitability of the
software to his or her needs. Not later than the sixtieth day,
the user must register the software using one of the methods
contained in paragraph 3 below, or discontinue use of the
software and remove all operational copies from his or her
computer(s).  The user may download evaluation versions of the
next release to try the software again and the 60-day trial
starts over.  Reinstallation of the same version, for any reason,
after the initial 60-day trial DOES NOT, constitute a new trial
period and is a violation of the shareware license agreement and
is illegal.  When purchasing a registration, the user is not
purchasing the software itself but is purchasing a license to use
the software.  Registration does not imply nor entail ownership
of the software.  The user's license may be revoked by WSS at
any time should he or she violate any provision of this document
or the specifications contained in the license agreements
contained in the distribution archives.

3. Registration Options:  Registration entitles the user to
free upgrades to all releases under the major revision
registered.  For example, if a user registered version 4.10, s/he
is entitled to free upgrades to all 4.xx releases.  Upgrade fees
for major revisions may or may not be charged and if applicable,
will be published well in advance of major releases.  There are
currently two methods of registration are available:

      a. Normal Mail in Registration: Registration is $80.00 (US)
        for the DOS platform of the BBS Software and $25.00 (US)
        for the network software alone for use with other BBS
        systems. Pricing for other platforms will be published
        as they are released.  

        b. Registration Payment Plan: WSS offers a payment plan
        for the purchase of BBS registrations.  The payment plan
        for 4.30 consists of four payments of $25.00 (US).  Each
        payment extends the users trial period by sixty days.
        ALL PAYMENTS ARE NON REFUNDABLE.  If a user fails to
        make scheduled payments on time or to complete the
        payment plan within 240 days (8 months), the account
        will be in default, the payment plan will be terminated
        and no refund will be issued.  The registration number
        and passcode are not issued nor is the user registered
        until all payments have been made.  WSS will notify any
        network administration of payments received based on the
        requests of the user.

4. Instance Upgrades: The unregistered shareware version allows
the user to run a single instance of the BBS software.
Registered versions allow two instances.  At the time of
registration or at a later date, the user may purchase upgrades
to allow the operation of more instances.  The upgrade pricing
is as follows:
   
   ÚÄÄÄÄÄÄÄÄÄÄÄÄÄÄÂÄÄÄÄÄÄÂÄÄÄÄÄÄÂÄÄÄÄÄÄÂÄÄÄÄÄÄÂÄÄÄÄÄÄ¿
   ³Upgrade From  ³   2  ³   4  ³   8  ³  16  ³  32  ³
   ÃÄÄÄÄÄÄÄÄÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄ´
   ³Upgrade to 4  ³  $20 ³      ³      ³      ³      ³
   ÃÄÄÄÄÄÄÄÄÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄ´
   ³Upgrade to 8  ³  $45 ³  $25 ³      ³      ³      ³
   ÃÄÄÄÄÄÄÄÄÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄ´
   ³Upgrade to 16 ³  $80 ³  $60 ³  $35 ³      ³      ³
   ÃÄÄÄÄÄÄÄÄÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄ´
   ³Upgrade to 32 ³ $120 ³ $100 ³  $75 ³  $45 ³      ³
   ÃÄÄÄÄÄÄÄÄÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄÅÄÄÄÄÄÄ´
   ³Unlimited     ³ $220 ³ $200 ³ $175 ³ $145 ³ $100 ³
   ÀÄÄÄÄÄÄÄÄÄÄÄÄÄÄÁÄÄÄÄÄÄÁÄÄÄÄÄÄÁÄÄÄÄÄÄÁÄÄÄÄÄÄÁÄÄÄÄÄÄÙ
   
5. Transfer of Registrations: REGISTRATIONS MAY ONLY BE
TRANSFERRED BY WWIV SOFTWARE SERVICES.  Transfer requests must
include Old Owner and New Owner Transfer forms; a new
registration form completed by the new owner and a check or
money order for $25.00 (US).  It is up to the parties involved
as to who pays the transfer fee.  Any sales price beyond the
transfer fee are the concern of the parties involved and are not
the responsibility or concern of WSS.  The necessary forms for
transfers may be obtained by e-mailing WSS.  Transfers will not
be processed until all completed forms and fees are received.
All entitlements to source code and SDS Access for the Old Owner
are terminated upon the proper execution of the transfer.

6. Registration Exemptions:  Subject to the conditions below,
registration exemptions are authorized to be granted by the
Network Coordinators of:

    FILEnet     GLOBALnet   IceNet
    TerraNet    WWIVLink    WWIVnet

The NC of these networks may grant an exemption for systems
acting in the capacity of network servers.  NC's may place
additional requirements on the system; however, the following
minimum criteria must be met in order to grant the exemption:

    a. The requesting sysop must have purchased a valid
    registration for at least one copy of WWIV and must be
    running a public BBS on the network in question using
    that registration number.

    b. The primary purpose of the exempt system must be the
    movement of network traffic and not operate as a public
    dialup system.  User accounts on the server will be limited
    to number one accounts of connecting systems generated by
    the server operator.

    c. The server operator will provide a dialup telephone
    number or Internet address (telnet) for the system to allow
    the NC or WSS to log on to the system.  This is to verify
    that the system is in fact a server system and maintains
    compliance with both WSS and network policy.

    d. The requesting system must operate for the good of the
    network as a whole in the judgement of the network
    administration.

Network Coordinators desiring authorization to grant exemptions
should e-mail WSS directly.

7. Source Code Availability: Currently, registration of the BBS
software entitles the user to the source code to the BBS.  If,
at any time in the future, it becomes impossible or too difficult
to control the distribution of source code, this policy may be
rescinded.  FOR SECURITY REASONS, THE SOURCE CODE TO 4.x INIT.EXE,
NETWORK SOFTWARE OR NETUP IS NOT AVAILABLE TO ANYONE.  Source
code to the current version of WWIV may be obtained on disk
directly by sending a completed registration form and $10.00 (US)
to WSS.  Registered users may also download the current source
code from an authorized Source Distribution System (SDS).  A
list of dialup SDS Systems is available upon request from WSS.
SDS systems are authorized by WSS to distribute source code
without charge to registered users after verification of their
registration information with WSS.  In order to download the
source code from a SDS, the registered user must mail WSS FROM
the SDS system using the Registration Verification System
installed on all SDS sites.  (Type //SDS from the mail menu) and
provide the following information:

        a.  Registration Number
        b.  Registration Passcode (if issued)
        c.  Real Name
        d.  Address at the time of registration (if no passcode
            has been issued)

   Source code access is also available via the Internet on our
Internet SDS at http://sds.wwiv.com/.  You will be required to
provide a through d above on this site during the application
process.  Processing of these applications is normally
accomplished within three business days.

8. Source Code Modification Publication: Registered users may
publish modifications on sub-boards designed for that purpose on
individual networks.  It is the responsibility of the host of
these subs to ensure that only registered users are permitted to
subscribe to subs where modifications are posted. Source code
modifications that contain more than 50 lines of original BBS
code require a release authorization for publication from WSS.
E-mail the mod in its entirety to WSS.  Releases or Denial of
Release will be issued within five business days.

9. Modification Access Restrictions: Registered sysops will
control access to all BBS modifications available for download,
viewing, reading or capture on their system.  The registration
information for ALL individuals desiring access to modifications
in any form must be verified with WSS before granting access.
Email WSS for the required modification to send access requests.
WSS will only accept validation requests generated by this
authorized modification.

10. Source Code License Agreement: Unauthorized distribution of
WWIV BBS Source Code or portions thereof is a crime.  Registered
and/or unregistered individuals found in violation of the Source
Code License Agreement contained in the source code archive will
be prosecuted to the fullest extent of both civil and criminal
laws.  All registered users should review of the Source Code
License Agreement to ensure they fully understand and are in
compliance with it.  Registered users in violation of this
agreement will have theirregistration and license permanently
revoked in addition to any legal action taken.

11. WSS Source Distribution Systems (SDS):  WSS has several
systems specially authorized to distribute source code to
registered sysops.  The number of systems is limited and only
the most qualified systems are selected for this function.
Meeting all the qualifications of the criteria listed below is no
guarantee of selection.  

  a. You MUST be the sysop (#1) of your system.

  b. You MUST have been a registered sysop for at least 2 years.

  c. You MUST have been running your BBS continuously for the
     last 2 years.

  d. Your BBS MUST be a full time system, open to anyone who
     wishes to call.   No part-time boards, closed boards, or
     boards that require a new user password to sign on.

  e. You MUST be 21 years of age or older and provide a
     photocopy of an official photo ID to WSS with your
     application.

  f. You MUST have been a member of at least one major network
     for a minimum of one year. (preferably WWIVnet, WWIVLink
     IceNet, TerraNet or FILEnet)

  g. You MUST provide a list of at least 20 registered WWIV
     Sysops who want to be able to download the WWIV Source
     Code from you, listing their real names and registration
     numbers.

  h. Upon acceptance, you must be willing to sign a
     distribution agreement with WSS that outlines your legal
     responsibilities and obligations as a Source Distribution
     System.

12. WSS Support Board Network:  WSS provides a network of highly
skilled, knowledgeable sysops to the BBS community.  Sysops
selected for this status are time tested and have been recognized
for the amount and quality of support they offer.  Below is a
description of the types of support offered and selection
criteria for each:

    a. The Support Coordinator and active Support Boards select
    new Support Boards (SB).  To become an official Support
    Board, the sysop, as a minimum, must meet the requirements
    of 11a through 11d above.  In addition, the following
    conditions must be met:

        1. The sysop must maintain a library of all official
        WSS releases, and a reasonably stocked library of WWIV
        support files, readily accessible to the public, without
        restrictions or ratios.

        2. The system must offer Auto Sysop Validation (ASV)
        and/or Guest Sysop Account (GSA)

        3. You MUST have been a member of at least one major
        network for a minimum of one year. (preferably WWIVnet,
        WWIVlink, IceNet, TerraNet or FILEnet)

        4. The sysop must be thoroughly knowledgeable concerning
        BBS and network operations and will be required to
        provide prompt, courteous replies to requests for
        assistance as well as extensive assistance to new sysops
        who may request help.

    b. WSS and the active Core Sysops select Core Support Boards
    (CSB).  To be considered for Core Status, the sysop must have
    a minimum of 2 years of exemplary service as a Support Board.
    There is no application process as with the SB system.  Core
    Support Boards are selected solely on tenure and merit of
    service.

    Support Board status of either type may be removed at any
time by either WSS or the Support Coordinator if the sysop fails
to meet minimum requirements or when individual conduct is
contrary to the spirit and intent of the support network or
relects negatively on WSS or WWIV as a whole.
```
