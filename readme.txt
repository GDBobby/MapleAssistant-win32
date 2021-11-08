THIS IS AN OLD VERSION WITH LESS FUNCTIONALLY THAN THE SFML PORT
	for the SFML port visit https://github.com/GDBobby/MapleAssistant


v1.1 - code rearranged/cleaned
	corsair custom mix added
	dps for different skills displayed concurrently
	clearer usage for elestaff with mages
	small bucc formula error fixed (no longer using lines to account for barrage bonus)
	
	

Notes :
-when a dev changes booster from +2 to +3, chain lightning speed is 630, paralyze&angelray is 690


@~@~@~@~@~@~@~@~@
class IDs

bowmaster 	0
marksman 	1
darkknight	2
hero		3
paladin		4
i/l			5
f/p			6
bishop		7
shadower	8
nightlord	9
bucc		10
corsair		11
@~@~@~@~@~@~@~@~@


@~@~@~@~@~@~@~@~@
weapon IDs

0 bow
1 xbow
2 spear
3 1hsword
4 2hsword
5 1ham
6 2ham (2h axe/mace)
7 elestaff
8 dagger
9 claw
10 knuckle
11 gun
@~@~@~@~@~@~@~@~@


~@~@~@~@~@~@~@~@~@~
weapon info layout

weapon multiplier (multipled by 10 cause no decimal)

(skill 1, speed 2) (skill 2, speed 2)
...
(singletarget skill 1, speed 6) (st2, sp6) (mt1, sp6) (multitarget 2, speed 6)
(if applicable, the next row is the spamming speed, i.e. boomerang step)
~@~@~@~@~@~@~@~@~@~


~@~@~@~@~@~@~@~@~@~
job info layout

Name
mastery
Attack1 Attack2(skill names) --- (if you add/remove skills, update the skill structs)
percent1 percent2
lines1 lines2
critchance (before SE)
critdmg (before SE, default is 0)
other modifiers default value is 1 (elemental charges, shadow partner, combo, berserk etc)
	include elemental staff and elemental amplification
	Paladin is ordered Holy Fire Lightning Ice
	currently multiplied by 100 to prevent decimals, default is 100
~@~@~@~@~@~@~@~@~@~