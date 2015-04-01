# All the old News Articles #

#### 1/26/09 ####

FIXED:
  1. Aimbot in the PK3's ( for an early release go to [issue 4](https://code.google.com/p/thz/issues/detail?id=4) and grab THZ-Aimbot.pk3 and tell me what you think )


UPDATES:

  1. Added chatballoons back into the SVN
  1. Updated the Hacked Client + QVM with the new CGAME builds
  1. Working on porting Score Scrolling from ioQuake3 into the qvm
  1. Working on a client side \mystats
  1. Considering porting google/mercury's FSM pvars to the cgame. ( + add a few )

BUGS:

~~So it seems that lord.undergamers hacked client was just a little bit more than a hacked QVM loader.~~

~~In short the aimbot functionality is broken in the pk3's ( [issue 4](https://code.google.com/p/thz/issues/detail?id=4) )~~ <-- FIXED SEE ABOVE

#### 1/22/09 ####

Triggerbot has been committed to the SVN, New PK3 has been dropped in the downloads section.


Triggerbot is functional

to turn on do

` \thz_triggerbot 1 `

and off

` \thz_triggerbot 0 `


I don't recommend using trigger bot with weapons you hold the trigger down with like the machine gun, las gun, psaw, and luci.

Works great with shotgun and Mass Driver and with all the alien classes.



#### 1/21/09 ####

Thanks to the gratuitous efforts of a fellow THZ user we should now Have working a
working triggerbot system.

Pending  my review I will update the code base to reflect the changes and update the
Downloads with a new new thz-**.pk3**



#### 1/08/09 ####

New PK3 Uploaded to [issue 3](https://code.google.com/p/thz/issues/detail?id=3) - Clean up code - which removes about 20 or so unused varialbes, and 2-3 unused functions.

I will update the issue with everything I removed soon.

until then grab the pk3 from: [issue 3](https://code.google.com/p/thz/issues/detail?id=3)

I have tested and verified it works without any issues.


#### 1/07/08 ####

Still Working on the Triggerbot System, Not working out so well. Problem is we get locked into a state of either shooting ( +attack ) or not shooting ( -attack ).

I believe this happens because cgs.clientinfo[trace.entityNum ](.md) doesn't update when your not looking at a player, which leaves us in a state of +attack.

Then it does update to NULL or zeroed out values when you die, which leaves us in a state of -attack.

Anyways, I hope to have triggerbot working soon.


Other things I'm working on include Code clean up and a builtin thzhelp for on demand help


#### 1/02/08 ####


Firstly, HAPPY NEW YEAR!

Next, I have updates. Now if you've ever tried using thz\_triggerbot you'll
notice it didn't work. HOPEFULLY I've fixed that. I'll spair you the gruelling
computer speak on the issue if you want to see what I've been doing then take
a look at the 'issues' section and read the comments I've made.

You will also find the new canidate for THZ-4.2.2 which contains the fix for
the triggerbot ( I hope ).


Anyways, If you want to try it let me give you the configuration info:

```
\thz_triggerbot 1
# do this to kill aliens

\thz_triggerbot 2
# do this to kill humans

\thz_triggerbot 0
# anything else will turn it off
```

#### 12/23/08 ####

Updated the QVM's ( Finally ). This is another Hacked Pk3 file witch again is easily installed by replacing the existing vms-1.1.0.pk3 with the new one.

NOTE: This new pk3 is named _thz-4.2.0.pk3_ so instead of downloading vms-1.1.0.pk3 you download the _thz-4.2.0.pk3_

NOTE: You should remove all previous qvm archives. I.E. delete/Move ( do a backup first ) the existing _vms-1.1.0.pk3_ and place _thz-4.2.0.pk3_ in its place.

You may need to rename _thz-4.2.0.pk3_ to _vms-1.1.0.pk3_ ( but I doubt it )


#### 12/16/08 ####

#### Created a new google code for my ziptool application. Check it out at ####

### [ziptool google code](http://code.google.com/p/ziptool/) ###



In other news, some of the more dedicated tremulous servers administration seems to be sweating a little at the idea of THZ's simplicity. None of them have a clue on how they would detect THZ to begin with rather than modifying the code that I am in control of. Unfortunately Some people have the idea that they will make there clients have identical cvars that will take precedence of the THZ cvars, which might mean that I will have to rename them every so often just so users don't get bit in the ass.


#### 12/10/08 ####

Oops!! So I was, erm.., testing the hacked _vms-1.1.0.pk3_ and I noticed a couple of bugs that I thought had been fixed in the latest versions of THZ.

Turns out that I spoofed an older version of THZ ( 4.0 I believe ). It seems to have happened when I making the file on my Mac. I still had the previous version of THZ from when I originally ported THZ to OS X.

Needless to say I'm a little embarrassed of my goof. :>

Luckily, I do happen to have the updated _pak_ but Its on my workstation so I will update the Downloads tomorrow.



#### 12/09/08 ####

I've finished a working copy of my **_crcSpoofer_** but will not be releasing it ATM.

What I have left to do for my Spoofer is
  1. Fix some issues where I don't free all memory allocated by _malloc()_
  1. Fix a couple broken functions which will make the code more universally applicable
  1. Add a few safety mechanisms so users can't destroy data.
  1. Random stuff ( general usability features, decide on a license etc )
<br>
the Spoofed vms-1.1.0.pk3 along with an install guide and if I get the time an install video.<br>
<br>
<br>
<br></li></ul>

<h4>12/06/08</h4>

Now that I'm coming to (what I hope to be) the end of my CRC32 zip file spoofer my thought is that I can make THZ a CGAME only hack removing the need for a hacked client to be used.<br>
<br>
<br>
<br>
Currently THZ-client has some spoofed code which sends the pure CRC32's to a server rather than the actual ones.<br>
By changing the CRC32 values in the pk3 we can send the pure CRC32's without needing to use a hacked client.<br>
<br>
<br>
<br>
In short, we will be able to port the HACKED CGAME to <b>ANY</b> <sup>1</sup>pure tremulous client.<br>
<br>
<br>
<br>
<sub>1. Pure: any client that can play on a server with pure settings</sub><br>
<br>
<br>
<h4>12/01/08</h4>


I've been working on a piece of C code that will spoof CRC32 values within zip/pk3 files.<br>
<br>
<br>
<br>
<br>
<del>Please visit fusionthz.net for updates and downloads. There you will be able to find<br>
discussions and a small community from which to ask troubleshooting questions.</del>


<h3>Fusionthz.net is gone. Being that it is I have uploaded the original Client Binary to the to the Downloads section.</h3>