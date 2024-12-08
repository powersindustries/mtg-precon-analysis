### Magic the Gathering Preconfigured Commander Deck Analysis
This project contains analytics searches and calculations for all commander decks released by Wizards of the coast from 2023-2024. This repo acts as a companion piece for an episode of the Wild Dogs Podcast.

### Database
All cards can be found in a csv file labeled `cardDatabase.csv` within the `data` directory. The csv file uses the `;` character as their deliminator. The columns go in order of:
```
Name;Mana Cost;Type;Description;Color Identity;Sets;Decks
```

### Script Outputs
#### colors_analytics.py
```
----------------------------------------------------
Output for colors regardless of color pairing. Percentages are relative.
----------------------------------------------------
Red Overall 447, or 17.02857142857143%
Green Overall 589, or 22.438095238095237%
Blue Overall 548, or 20.876190476190477%
Black Overall 450, or 17.142857142857142%
White Overall 591, or 22.514285714285716%


----------------------------------------------------
Mono-colored percentages. How many cards are mono color?
----------------------------------------------------
Colorless Overall 605, or 23.047619047619047%
red 241, or 9.13570887035633%
green 369, or 13.987869598180438%
blue 308, or 11.675511751326763%
black 246, or 9.32524639878696%
white 379, or 14.3669446550417%


----------------------------------------------------
Two-colored pairing percentages. How many cards are duel color.
----------------------------------------------------
wu 31, or 1.1751326762699015%
rw 42, or 1.592115238817286%
bu 47, or 1.781652767247915%
bg 39, or 1.4783927217589083%
gr 25, or 0.9476876421531463%
ur 37, or 1.4025777103866566%
bw 38, or 1.4404852160727823%
br 33, or 1.250947687642153%
gw 37, or 1.4025777103866566%
ug 69, or 2.6156178923426836%


----------------------------------------------------
Three-colored pairing percentages.
----------------------------------------------------
wbg 5, or 0.18953752843062927%
guw 7, or 0.265352539802881%
wub 5, or 0.18953752843062927%
ubr 12, or 0.45489006823351025%
urw 18, or 0.6823351023502654%
brg 7, or 0.265352539802881%
rgw 17, or 0.6444275966641395%
rwb 7, or 0.265352539802881%
bgu 6, or 0.22744503411675512%
gur 3, or 0.11372251705837756%


----------------------------------------------------
Five-colored pairing percentages.
----------------------------------------------------
wubrg 5, or 0.18953752843062927%
```


#### commander_analytics.py
```
Commander mana curve analytics (How much mana you need to cast the commander).
0 mana : 0, 0.0%
1 mana : 0, 0.0%
2 mana : 2, 3.8461538461538463%
3 mana : 11, 21.153846153846153%
4 mana : 22, 42.30769230769231%
5 mana : 10, 19.230769230769234%
6 mana : 2, 3.8461538461538463%
7 mana : 1, 1.9230769230769231%
8 mana : 2, 3.8461538461538463%
9 mana : 0, 0.0%


Commander color count analytics (How many different colors you need to cast the commander).
1 color : 2, 3.8461538461538463%
2 color : 20, 38.46153846153847%
3 color : 26, 50.0%
5 color : 2, 3.8461538461538463%


Commander color pairing analytics (What colors do you need to cast the commander).
C: 1, 1.9230769230769231%
W: 1, 1.9230769230769231%
BG: 2, 3.8461538461538463%
BR: 1, 1.9230769230769231%
BU: 2, 3.8461538461538463%
BW: 3, 5.769230769230769%
GR: 1, 1.9230769230769231%
GU: 6, 11.538461538461538%
GW: 1, 1.9230769230769231%
RU: 2, 3.8461538461538463%
RW: 2, 3.8461538461538463%
BGR: 1, 1.9230769230769231%
BGU: 2, 3.8461538461538463%
BGW: 2, 3.8461538461538463%
BRU: 2, 3.8461538461538463%
BRW: 2, 3.8461538461538463%
BUW: 2, 3.8461538461538463%
GRU: 1, 1.9230769230769231%
GRW: 6, 11.538461538461538%
GUW: 2, 3.8461538461538463%
RUW: 6, 11.538461538461538%
BGRUW: 2, 3.8461538461538463%
```


#### mana_curve_analytics.py
```
0 mana: 1
1 mana: 98
2 mana: 430
3 mana: 606
4 mana: 478
5 mana: 312
6 mana: 181
7 mana: 89
8 mana: 34
9 mana: 9
10 mana: 10
11 mana: 3
12 mana: 5
13 mana: 0
14 mana: 0
```


#### type_analytics.py
```
All cards, count: 51
["Arcane Signet;{2};Artifact;{T}: Add one mana of any color in your commander's color identity.;;who,ixilan,marchOfTheMachine,commanderMasters,bloomburrow,wildsOfEldraine,modernHorizons3,lordOfTheRings,secretLair,fallout,allWillBeOne,duskmoore,thunder,karlovMannor;blastFromThePast,paradoxPower,masterOfEvil,timeyWimey,velociRampTor,exploreTheDeep,ahoyMatey,bloodRites,callForBackup,tinkerTime,growingThreat,divineConvocation,cavalryCharge,planeswalkerParty,enduringEnchantments,sliverSwarm,peaceOffering,squirreledAway,animatedArmy,familyMatters,virtueOfValor,faeDomination,eldraziIncursion,trickyTerrain,graveyardOverdrive,creativeEnergy,hostsOfMordor,ridersOfRohan,foodAndFellowship,elvenCounsel,rainingCatsAndDogs,angels,cuteToBrute,science,mutantMenace,hailCaesar,everLoyal,rebellionRising,corruptingInfluence,deathtoll,endlessPunishment,jumpScare,miracleWorker,quickDraw,grandLarceny,desertBloom,mostWanted,deepClueSea,revenantRecon,blameGame,deadlyDisguise\n", 'Sol Ring;{1};Artifact;{T}: Add {C}{C}.;;who,ixilan,marchOfTheMachine,commanderMasters,bloomburrow,wildsOfEldraine,modernHorizons3,lordOfTheRings,secretLair,fallout,allWillBeOne,duskmoore,thunder,karlovMannor;blastFromThePast,paradoxPower,masterOfEvil,timeyWimey,velociRampTor,exploreTheDeep,ahoyMatey,bloodRites,callForBackup,tinkerTime,growingThreat,divineConvocation,cavalryCharge,eldraziUnbound,planeswalkerParty,enduringEnchantments,sliverSwarm,peaceOffering,squirreledAway,animatedArmy,familyMatters,virtueOfValor,faeDomination,eldraziIncursion,trickyTerrain,graveyardOverdrive,creativeEnergy,hostsOfMordor,ridersOfRohan,foodAndFellowship,elvenCounsel,rainingCatsAndDogs,angels,cuteToBrute,science,mutantMenace,hailCaesar,rebellionRising,corruptingInfluence,deathtoll,endlessPunishment,jumpScare,miracleWorker,quickDraw,grandLarceny,desertBloom,mostWanted,deepClueSea,revenantRecon,blameGame,deadlyDisguise\n']


Total Artifact count: 328
Artifacts, count: 51, 

["Arcane Signet;{2};Artifact;{T}: Add one mana of any color in your commander's color identity.;;who,ixilan,marchOfTheMachine,commanderMasters,bloomburrow,wildsOfEldraine,modernHorizons3,lordOfTheRings,secretLair,fallout,allWillBeOne,duskmoore,thunder,karlovMannor;blastFromThePast,paradoxPower,masterOfEvil,timeyWimey,velociRampTor,exploreTheDeep,ahoyMatey,bloodRites,callForBackup,tinkerTime,growingThreat,divineConvocation,cavalryCharge,planeswalkerParty,enduringEnchantments,sliverSwarm,peaceOffering,squirreledAway,animatedArmy,familyMatters,virtueOfValor,faeDomination,eldraziIncursion,trickyTerrain,graveyardOverdrive,creativeEnergy,hostsOfMordor,ridersOfRohan,foodAndFellowship,elvenCounsel,rainingCatsAndDogs,angels,cuteToBrute,science,mutantMenace,hailCaesar,everLoyal,rebellionRising,corruptingInfluence,deathtoll,endlessPunishment,jumpScare,miracleWorker,quickDraw,grandLarceny,desertBloom,mostWanted,deepClueSea,revenantRecon,blameGame,deadlyDisguise\n", 'Sol Ring;{1};Artifact;{T}: Add {C}{C}.;;who,ixilan,marchOfTheMachine,commanderMasters,bloomburrow,wildsOfEldraine,modernHorizons3,lordOfTheRings,secretLair,fallout,allWillBeOne,duskmoore,thunder,karlovMannor;blastFromThePast,paradoxPower,masterOfEvil,timeyWimey,velociRampTor,exploreTheDeep,ahoyMatey,bloodRites,callForBackup,tinkerTime,growingThreat,divineConvocation,cavalryCharge,eldraziUnbound,planeswalkerParty,enduringEnchantments,sliverSwarm,peaceOffering,squirreledAway,animatedArmy,familyMatters,virtueOfValor,faeDomination,eldraziIncursion,trickyTerrain,graveyardOverdrive,creativeEnergy,hostsOfMordor,ridersOfRohan,foodAndFellowship,elvenCounsel,rainingCatsAndDogs,angels,cuteToBrute,science,mutantMenace,hailCaesar,rebellionRising,corruptingInfluence,deathtoll,endlessPunishment,jumpScare,miracleWorker,quickDraw,grandLarceny,desertBloom,mostWanted,deepClueSea,revenantRecon,blameGame,deadlyDisguise\n']


Total Creature count: 1300
Creature, count: 10, 

['Solemn Simulacrum;{4};Artifact Creature — Golem;When Solemn Simulacrum enters, you may search your library for a basic land card, put that card onto the battlefield tapped, then shuffle. When Solemn Simulacrum dies, you may draw a card.;;who,commanderMasters,bloomburrow,modernHorizons3,fallout,allWillBeOne,duskmoore,karlovMannor;masterOfEvil,eldraziUnbound,familyMatters,creativeEnergy,science,rebellionRising,deathtoll,endlessPunishment,miracleWorker,blameGame\n']


Total Instant count: 200
Instant, count: 17, 

['Swords to Plowshares;{W};Instant;Exile target creature. Its controller gains life equal to its power.;W;who,ixilan,marchOfTheMachine,commanderMasters,bloomburrow,wildsOfEldraine,modernHorizons3,lordOfTheRings,secretLair,fallout,allWillBeOne,duskmoore,karlovMannor;blastFromThePast,bloodRites,callForBackup,growingThreat,divineConvocation,cavalryCharge,planeswalkerParty,peaceOffering,virtueOfValor,creativeEnergy,ridersOfRohan,foodAndFellowship,angels,science,corruptingInfluence,miracleWorker,deepClueSea\n']


Total Sorcery count: 265
Sorcery, count: 12, 

['Cultivate;{2}{G};Sorcery;Search your library for up to two basic land cards, reveal those cards, put one onto the battlefield tapped and the other into your hand, then shuffle.;G;who,ixilan,marchOfTheMachine,commanderMasters,bloomburrow,lordOfTheRings,secretLair,fallout,allWillBeOne,duskmoore;paradoxPower,velociRampTor,callForBackup,sliverSwarm,peaceOffering,animatedArmy,foodAndFellowship,elvenCounsel,rainingCatsAndDogs,mutantMenace,corruptingInfluence,jumpScare\n']


Total Enchantment count: 311
Enchantment, count: 4, 

['Spirited Companion;{1}{W};Enchantment Creature — Dog;When Spirited Companion enters, draw a card.;W;marchOfTheMachine,commanderMasters,bloomburrow,secretLair;divineConvocation,enduringEnchantments,familyMatters,rainingCatsAndDogs\n']


Total Equipment count: 53
Equipment, count: 9, 

["Lightning Greaves;{2};Artifact — Equipment;Equipped creature has haste and shroud. (It can't be the target of spells or abilities.) Equip {0};;who,commanderMasters,modernHorizons3,lordOfTheRings,secretLair,fallout,duskmoore,thunder;masterOfEvil,timeyWimey,eldraziUnbound,graveyardOverdrive,elvenCounsel,angels,science,endlessPunishment,mostWanted\n"]


Total Aura count: 53
Aura, count: 3, 

['Shiny Impetus;{2}{R};Enchantment — Aura;Enchant creature Enchanted creature gets +2/+2 and is goaded. (It attacks each combat if able and attacks a player other than you if able.) Whenever enchanted creature attacks, you create a Treasure token. (It\'s an artifact with "{T}, Sacrifice this artifact: Add one mana of any color.");R;lordOfTheRings,thunder,karlovMannor;hostsOfMordor,mostWanted,blameGame\n']


Total Fancy Land count: 306
Fancy Land, count: 50, 

["Command Tower;;Land;{T}: Add one mana of any color in your commander's color identity.;;who,ixilan,marchOfTheMachine,commanderMasters,bloomburrow,wildsOfEldraine,modernHorizons3,lordOfTheRings,secretLair,fallout,allWillBeOne,duskmoore,thunder,karlovMannor;blastFromThePast,paradoxPower,masterOfEvil,timeyWimey,velociRampTor,exploreTheDeep,ahoyMatey,bloodRites,callForBackup,tinkerTime,growingThreat,divineConvocation,cavalryCharge,planeswalkerParty,enduringEnchantments,sliverSwarm,peaceOffering,squirreledAway,animatedArmy,familyMatters,virtueOfValor,faeDomination,eldraziIncursion,trickyTerrain,graveyardOverdrive,creativeEnergy,hostsOfMordor,ridersOfRohan,foodAndFellowship,elvenCounsel,rainingCatsAndDogs,cuteToBrute,science,mutantMenace,hailCaesar,everLoyal,rebellionRising,corruptingInfluence,deathtoll,endlessPunishment,jumpScare,miracleWorker,quickDraw,grandLarceny,desertBloom,mostWanted,deepClueSea,revenantRecon,blameGame,deadlyDisguise\n"]
```
