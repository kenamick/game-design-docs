Spitflyer Effect
========================

_(Design document)_

![Terrain Demo](http://i.imgur.com/yyhwNhK.png)

## Preface

This is a game I designed back in 2006 while working at in the mobile field. I created a working prototype but then discontinued the project and later on left the company because of another offer. 

## Vision

The goal is to develop a minimalistic 3D third-person shooter game for handsets. The game action is carried out in outer space on the surface of space platforms and moons. Gameplay must be fast-paced/real-time/dynamic.

## Concept

A game in which the player has a Third-person perspective to the in-game world. Player controls a machine kind of battle armor which he has to keep safe of enemy projectiles. By destroying enemies, the player will gain various damage, speed and weapon bonuses. The player must complete a number of missions/quests in order to win. The 3D perspective will allow for 360° rotation and observation of the in-game level environment. Low-res textures must be carefully adjusted in order to represent the outer space look as realistic as possible. Players would have the complete freedom to move within the borders of each level area. 

The game would first be released as single-player title in which a number of battle modes (Skirmish, campaign, co-op) will be available. 

## Game Story

The year is 2415. Government forces from the colony **Terminus** in the system Vega are preparing to launch a new kind of war unit called the **Spitflyer**. These units are a product of the latest advancements in neuroscience technology used to train the perfect artificial intelligence for military purposes. For this purpose undercover government organizations aided by organized crime channels are kidnapping children from nearby colonies and are delivering them to government scientists to be used as experiment subjects.

In the second half of the year 2417 rebels from nearby military and economically weaker, colonies **Atira** and **Taristol II** are organizing a large scale attack against a secret government base on the moon **Efriador V**. The attack is repelled by the newly deployed Spitflyer units with which the beginning of a large scale civil war in the Vega sector is started. The authorities in Atira and Taristol II unite themselves under a rebel federation force against the corrupted Terminus government. However, in this distant from Earth system, the only hope they have left is a single Spitflyer unit that managed to preserve his human consciousness.

## Gameplay

The single-player game will have 2 types of game modes - One-Man-Army and Melee.
Multiplayer is not planned for the first release.

### One-Man-Army 
In this game mode the player would have to repel and survive enemy attacks for a given period of time. This game mode is meant as training mode in which the player should be brought into the in-game tactics, map features and bonuses. Enemies would be spawned from different angles and distance from the player.

#### Rules
The game A.I. will spawn enemy units from different angles and distance on the game map. Their will be to attack and destroy the player.

#### Goals
Each round continues until the player is destroyed no more than 3 times. After that the game switched to the main menu.

### Melee
This game mode is much more interesting for players that have already completed training. The player will have to fight several bots in _free for all_ type of game mode. A number of bonuses - weapons, damage or armor increase will be spawned on the map. 

#### Rules
In this game mode respawn map points and bonuses spawn points will be generated. In the beginning player and enemies will be spawned on non-adjacent map positions. Player will be able to take cover behind in-game obstacles. Enemy projectiles must not pass map obstacles. Bonuses will be collected both by player and enemies. Therefore, the player must be careful when on route to a bonus item.

#### Goals
The end goal would be to win by either scoring most [frags](http://bit.ly/1tmNyI) for given round time or by scoring a defined amount of frags first.

### Bonuses
By destroying enemies player will have the possibility to gain a bonus. Bonuses may be either _passive_ or _selectable_.

 Type | Description 
 ---- | ----------- 
Passive | A bonus that is immediately received without any player interaction.
Selectable | A bonus that the player may select to take or not to take.


  Bonus        | Type          | Description  
 ------------- |:-------------:| ------------ 
Synthetic Boost      | Passive | A drug which increases the speed neural connections are established and neurons transmitted. In result the player's Spitflyer gains significant reaction and movement speed as compared to the enemies. Visually this is much like the [Matrix bullet effect](http://en.wikipedia.org/wiki/Bullet_time). Player moves normally and enemies appear to move and shoot slower.
Blister Shells      | Passive |  An upgrade to player's ammo increasing the damage done.
Nano Beam | Passive |  Shoots a laser beam packet that contains assault type nanobots.  When attached to enemy armor, these nanobots will make their way to internal Spitflyer systems effectively deactivating it's engines and combat system. In result enemy HP will decrease in time and eventually enemy Spitflyer will self-destruct. The unit may still move and shoot until it's HP zeroes.
Nano Repair | Passive | Nanobots that repair the Spitflyer's armor.

## Units
There will be 4 types of Spitflyer units. The first two types will have no differences in hit points and damage but only visual texture changes.

  1. Spitflyer Nuf-59 - Federation unit class.
  2. Military Assault Flyers - Terminus government unit class.
  3. Vegan Missile Armour - Long range Terminus unit class. *(Not playable)*
  4. Vegan Battle Armour - Boss unit. *(Not playable)*

All unit classes will appear in the **One-Man-Army** training mode.  With 1st unit as the player and all other as enemies. Only unit classes 1 and 2 will be available when playing in **Melee** mode.

## Terrain & Environment
All missions are carried out in outer space. Terrain types are either space platforms or moon surfaces. The map will mostly be pre-rendered squared terrains with elevation features. No real-time terrain generation should be used due to low device CPU resources. When player moves on elevated surfaces his Y position must automatically adjust. There could be different obstacles or in-game structures placed on the map. Player may take cover behind such structures.  Terrain will be static which means no structures or objects may be destroyed during playing.

![Terrain Demo](http://i.imgur.com/JaMUCDP.png)

## Distributable game releases

### Demo
In the demo version players will have the chance to play in **Melee** mode for 2 to 3 minutes. Not all bonuses will be available but only 1 or 2. Full game sources for **One-Man-Army** and **Melee** modes must not be included in the game build. We must achieved this using our build system which already features preprocessing directives.

### Single-player release
Standard paid release with all gameplay elements included. This would be the first playable & tested version ready for market distribution.

### Multiplayer release
This would be and expansion version including multiplayer mode. Users might Bluetooth enabled handsets will be able to play the game in multiplayer/Melee mode. This would basically be a free for all mode where every kill will be considered a [frag](http://bit.ly/1tmNyI). Players with most frags for give round time will win the round.

___
© 2006 Petar Petrov
