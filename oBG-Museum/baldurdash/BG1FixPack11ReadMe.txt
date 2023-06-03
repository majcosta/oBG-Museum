2001 - July - 07

This self-installing archive package contains several separate fix archives to resolve post-official-patch problems in Baldur's Gate/Tales Of The Sword Coast. This ReadMe file has been placed in your Baldur's Gate 2 folder; you may leave it there or delete it at your discretion.

This file and its accompanying FixPack was obtained from my webpage at http://members.home.com/mrkevvy

The following separate fix archives are contained in this self-installing package (newest to oldest in order of addition):

-------------------------------------------------------------------------
Newly Added/Updated Fixes
-------------------------------------------------------------------------

Ordulinian Quest Reward Fix

File ORDULI.DLG; an edited version of the dialog definition for the character Ordulinian, a priest found in the Sorcerous Sundries shop in Baldur's Gate. It resolves a bug which causes his quest reward of a cloak to not be given. He is supposed to reward the player with a Cloak Of Non-Detection, but the dialog command to cause this to happen fails to take into account that he doesn't have the cloak with him; it must be created. He now gives the intended reward.

Thanks to Dan Simpson (of FAQ fame) for pointing this out!

-------------------------------------------------------------------------

Magic Missile Damage Fix

Files SPWI003.SPL and SPWI112.SPL; edited versions of the spell definition files for the 1st level wizard spell Magic Missile. They resolve a bug with the amount of damage done by the Magic Missiles. This may have been a limitation of the early BG Infinity engine that spell effect damage could only be of xDy, not xDy + z modifier form, and the spells were created first as the Wand Of Magic Missiles does the correct 1D4 + 1 damage.

Note: The previous FixPack changed the Wand Of Magic Missiles' damage to match the (incorrect) damage of the other Magic Missile spells, but as 1D4+1 is the correct amount, the Wand Of Magic Missiles file will be removed if it is found as these changes now finally correct all instances of Magic Missile in the game.

-------------------------------------------------------------------------
Existing Fixes
-------------------------------------------------------------------------

Aldeth Sashenstar Betrayal Fix

Files ALDETH.DLG, AR0128.BCS, AR1100.BCS, FLAMAL.BCS and FLAMAL.CRE; edited (and newly created) dialog definition file for Aldeth Sashenstar, area control script for AR0128 (Merchant League 2nd floor) and AR1100 (Baldur's Gate SW,) and newly created creature definition and creature control scripts for a specific Flaming Fist Enforcer. They complete a neglected (possibly forgotten) element of the Aldeth Sashenstar story: he will betray the player if he is spoken to in Chapter 7. The reasoning behind the conclusion that this may have been forgotten about during development is that the creature file for the Flaming Fist he summons was never created, nor did his dialog scripting attempt to summon it, so if he happened to be spoken to in Chapter 7, he would betray the player to Biff The Understudy. This would also occur if he hadn't been talked to since Cloakwood until Chapter 7. This is only supposed to occur after saving the Consortium, which is not an option in Chapter 7. Now, if the Consortium hasn't been saved by Chapter 7, he will no longer be found in front of it, nor will he be found in the Consortium after the Dukes have been saved, and the betrayal event will be completed properly should it be encountered.

-------------------------------------------------------------------------
Albert Doesn't Give The Reward For Rufie Fix

File ALBERT.DLG; an edited version of the dialog definition file for Albert, the "boy" met near Nashkel who wants his lost "puppy" named Rufie found. It corrects an omission where Albert, on leaving, says that he is giving another "chew toy" to the player, but gives nothing. He will now give an appropriate "chew toy" that Rufie might have removed from someone in the area. :^)

-------------------------------------------------------------------------
Gorpel Hind's Multiple Maulers Of The Undermountain Fix

Files AR0116.ARE, AR0116.BCS and GORPEL.DLG; edited versions of area definition file and area control script for AR0116 (the Helm And Cloak Inn in Baldur's Gate; AR0116.BCS did not exist previously) and the dialog definition file for Gorpel Hind, the leader of the Merry Fools adventurers found there. They resolve the bug whereby speaking to Gorpel Hind repeatedly causes the Maulers Of The Undermountain, an adventuring group that will attack the player and party, to appear as many times as Gorpel Hind is talked to. They will now only appear once.

-------------------------------------------------------------------------
Arrows Of Biting Damage Fix

Files AROW05.ITM, AROW12.ITM and AROW14.ITM; edited versions of the item definition files for the Arrow Of Biting poisoned arrows. They resolve the bug whereby these arrows give a strength bonus to damage, like a thrown weapon would. Arrows are not supposed to give such a bonus (any damage bonus is provided by the bow and the archer's proficiency.)

-------------------------------------------------------------------------
Jalanta Mistmyr Pickpocket Exploit Fix

File JALANT.CRE; an edited version of the creature definition file for Jalantha Mistmyr, priestess of Umberlee. It resolves the exploit of being able to pickpocket the "Child's Body" item from her, thereby completing the Varci Roaringhorn quest without either killing her or paying her 2,000 gold pieces.

-------------------------------------------------------------------------
Ramazith Pickpocket Exploit Fix

File RAMAZI.CRE; an edited version of the creature definition file for Ramazith, a mage of Baldur's Gate. It eliminates the exploit of being able to pickpocket his Ring Of Protection +2 from him, and then obtain another which he drops when he is slain at the top of his tower.

-------------------------------------------------------------------------
Oublek Emerald Bounty Exploit Fix

File OUBLEK.DLG; an edited version of the dialog definition file for Oublek, the bounty bureaucrat of Nashkel. It resolves a minor exploit with the return of the emeralds stolen by Prism for their bounty. If they were returned one at a time, he would pay the bounty twice.

-------------------------------------------------------------------------
Taerom Fuirium Ankheg Shell Exploit

File TAEROM.DLG; an edited version of the dialog definition file for Taerom "Thunderhammer" Fuirium, the blacksmith of Beregost. It resolves a bug leading to an exploit whereby the player could sell Ankheg shells to him multiple times. The player is only supposed to be able to choose once between selling all shells for 500 gold, or making a shell into Ankheg Plate Mail +2 for 4,000 gold. This was definitely a bug, as the embedded script command to turn off the ability to sell shells to him again was present, but was not being accessed due to an incorrect command length reference.

-------------------------------------------------------------------------
Ulgoth's Beard Residents Hostile When Cult Attacks Fix

File CULT3.CRE; an edited version of the creature definition file for the cult wizard who appears when the player arrives in Ulgoth's Beard with the Soultaker dagger. It resolves the bug where some of the innocent residents of Ulgoth's Beard would go hostile when this character was attacked, though he is an enemy and is clearly threatening the player. The cause was a leftover AI reference only for use by innocents.

-------------------------------------------------------------------------
Bone Wardstone Doesn't Disable Trap Machine Fix

File TRAPDIS.BCS; an edited version of the control script for the Rune Carpet machine in Durlag's Tower. It resolves the problem with being unable to disable the device even though the player is in possession of the Bone Wardstone "key" for it. The cause was a different range requirement when disabling the machine than when merely looking at it, which made it appear if the player was too far away that it was broken.

-------------------------------------------------------------------------
Bandit Scalp Pickpocket Exploit Fixes

.CRE files ARGHAI, BANDCAP, BANDCR, BANDIC, BANDIT, BANDIT2, BANDIT3, BANDITA, BANDITC, BANDITCY, BILLY, CANTO, DRIBBE, HOBGOBC, JEMBY, KNOTT, NEVILL, RAEMON, REPMAN, TEYNGA, THUG and ZAKAR; edited versions of the creature definition files for bandit characters. They resolve the somewhat minor exploit and humourous oversight of being able to pickpocket all these bandits for their scalps (item can be sold for 50 gp to certain characters as bounty.)

-------------------------------------------------------------------------
Game Crash In Tremain Belde'ar Dialog Fix

File TREMAI.DLG; an edited version of the dialog definition file for the character Tremain Belde'ar, a Tymoran priest. It resolves a dialog definition file corruption that would crash the game if the second, then first responses were chosen in the first dialog with him at his home after being brought there by Varci Roaringhorn.

-------------------------------------------------------------------------
Thief Scimitar Use Fix

Files SW1H20.ITM, SW1H22.ITM and SW1H23.ITM; edited versions of the item definition files for the Scimitar, Scimitar +1 and Scimitar +2 (Rashad's Talon) items. They resolve the inconsistency, which may or may not have been a bug, that thieves cannot use these weapons. I based the decision that this was an inconsistency and to change this on the following:

1) The two most powerful scimitars in the game are Drizzt's. They are both usable by thieves, and it's too late to take this ability away given the number of players who kill Drizzt for his items. Both these Scimitars' restrictions and descriptions do not exclude thieves, so this appears deliberate.
2) Thieves have full access to Scimitars in Baldur's Gate 2. There is even a thief character named Habib who dual-wields them (and throws them at player characters.)
3) There is no specific restriction on thieves from Scimitars in either the AD&D 2nd Edition Player's Handbook, the Arms & Equipment Guide, nor the Complete Thief's Handbook. While the ability is not granted, nor is it restricted.
4) Scimitars are no heavier and do no more damage than long swords, which thieves can use.
5) The speed factor of scimitars is lower than that of long swords, which would make them more appropriate thieves' weapons; minimal speed factor means a faster backstab (or in this case 'backslash.') And although scimitars are not thrusting weapons, neither are clubs, which thieves can also backstab (or 'backwhack') with.

As well, this is not an "unbalancing" decision. Scimitars are rare in Baldur's Gate; there are few of them. Other than Drizzt's (which thieves could already use,) there is only one +2 scimitar and it's in the TOSC expansion. There are one or two +1's. So, Drizzt's scimitars are still by far the best in the game, and they were thief-friendly already.

-------------------------------------------------------------------------
Alignment By Class Table Fix

File ALIGNMNT.2DA; an edited version of the definition table of alignment by class. It resolves a bug whereby multiclass thieves were not permitted to be of any Lawful alignments, rather than being restricted only from Lawful Good, as single-class thieves are. This bug was carried over into Baldur's Gate 2: Shadows Of Amn as well.

-------------------------------------------------------------------------
Gauntlets Of Ogre Power Usage Fix

File BRAC06.ITM; an edited version of the item definition file for the Gauntlets of Ogre Power. It resolves the bug of Bards being unable to use this item. They are not restricted from it in the description, and it was confirmed by Senior Designer David Gaider that they should be allowed to, as this bug carried over into Baldur's Gate 2: Shadows Of Amn.

-------------------------------------------------------------------------
Game Crash When Entering Area AR0717 Fix

File AR0717.ARE; an edited version of the area definition file for AR0717, an unnamed house just east of the city of Baldur's Gate carnival, whose door faces north and so cannot be seen. It resolves a game crash that would occur when entering the house. This was caused by an undefined creature reference that could not be found by the engine.

-------------------------------------------------------------------------
Three Old Kegs Noblewoman Charm Exploit Fix

File NOBW8.DLG; an edited version of the dialog definition file for the unnamed noblewoman on the top floor of the Three Old Kegs Inn in the city of Baldur's Gate. It resolves a bug with her dialog that led to an exploit whereby she could be charmed and repeatedly talked to, and she would give a gem and 500 gold pieces to the talker every time. This was a definite bug as the Global instead of SetGlobal command was being used as an Action to change a variable; it was not an oversight of failing to anticipate the exploit.

-------------------------------------------------------------------------
Killing Marl After Calming Him Down Exploit Fix

File MARL.DLG; an edited version of the dialog definition file for the character Marl, found in Feldepost's Inn in Beregost. It resolves an oversight leading to an exploit with this character. Marl doesn't like adventurers and explains why, so the player can either fight him for 650XP, or talk sense to him and calm him down for 900XP. However, once he was calmed down and harmless, the player could then kill him for 650XP but with no loss of reputation or other consequences though he had then become a neutral innocent. The appropriate loss of reputation and possible consequences now occur if this is done.

-------------------------------------------------------------------------


Kevin Dorner
mrkevvy@home.com
aka Kivan Do'Urner, solo CG E F/M/T
aaka Elmonster, solo LN H M

This file and its accompanying FixPack was obtained from my webpage at http://members.home.com/mrkevvy