Orbital Scavengers
===============================

_(Design Document)_

## Preface

This is a game concept I wrote back in 2004. Back then I was learning & making progress with OpenGL and I wanted to push that effort into a productive direction. Also, I was pretty inspired by the **Homeworld** title. I think I had been looking the game's [source code](http://www.fileplanet.com/137429/130000/fileinfo/Homeworld-Source-Code) as [Relic](http://www.relic.com/) posted it for free in 2003 and I really had the urge to write a game in pure C and OpenGL. 
I started gathering a team to work on this game as a freeware title. However, later I had to start a 'real' job and the project got disbanded.

## Concept

In the far future, a large number of humanity's orbital space stations are surrounded by garbage. Tourist ships, trade ship, corporations, etc. are all just pushing their garbage out in space effectively turning the space around space stations and platforms a *no-fly* zone. 

Player would take command of a space ship whose task would be to protect space stations from pollution & garbage left by tourist ships, insterstellar garbage carriers, pesky aliens, creatures from other dimensions which warped in just to throw their junk around and make some funny noises and others. Players should also protect the station from sudden meteor showers.
This would be a 3D game and the complete action would be carried out in deep space ([Babylon 5](http://en.wikipedia.org/wiki/Babylon_5) anyone?). The player will have complete control of her ship in all 3 axes movement. Camera view would be pretty similar to how it's done in **Homeworld** or the **Star Wars - Fighter** series.

![Homeworld screenshot](http://i.imgur.com/W11kEis.jpg)

_(Homeworld)_

## Game Story

Game story should be simple, fun and appealing to the player, so he can jump right into action.

In the far future, the 31st century, everyone has their own space-car and travelling around solar systems and the galaxy is little to no problem. Human nature however, did not change much. Everyone just ejects it's garbage around planets and space stations and the problem has taken immense proportions. Some planets are hardly accessible from all the junk flying around and some space stations have to clean junk constantly in order to provide a safe docking passage to ships. 
A political war is being waged by garbage collection & waste disposal corporations for territory, influence and money. Two of the biggest corporations are:
  * J.E.R.K.K. Corp. _(Junk ExteRmination & Karate Killers)_ - Founded by old generations of garbage collecting professionals.
  * I.D.I.O.T Enterprises _(Idle Dancers Ironing Obnoxious Trash)_ - Founded by a team of ex- playboy models which quickly took a large chunk of the galactic services market.

![I.D.I.O.T. corp](http://i.imgur.com/xLSR9wv.jpg)

_(Had to put a pretty girl here)_

The goal of the _Campaign mode_ would be to find out why did the galaxy became so polluted in the first place. Each mission will add some pieces to the story. The culmination will be at the last level where the player will meet the supreme multi-dimensional entity that looks upon the galaxy. It will then award the player with the ultimate answer ...something like 6x7 ;)

## Gameplay

Much like arcade games the gameplay should be quick, fast-paced and the player would be required to react quickly and use her reflexes, e.g., if several enemy targets are approaching at once player would be required to choose which one to attack (maybe the closest) and then quickly proceed to attack another.

Player gets the role of a _orbital-scavenger_. A mercenary from a given services corporation hired by space stations to keep their surroundings clear of garbage. Every space station would have a perimeter (more like a radius with the station in the center) that must be kept clean of pollution. Player would be paid space credits for a job well done which he can later use to buy upgrades for his ship. Space stations would not be limited only to such from human origins but the player would in fact be able to choose different stations from within the galaxy. And these may belong to other alien races which would pay space credits for the services the player provides. Traveling through the Galaxy would be possible by selecting marked places on a star map. Only places matching the skill and level of the player will be shown. 

Only single player mode is planned for the current version. There would be a campaign mode where players may choose which space stations in which part (solar system) of the galaxy to work for. Not all of the stations would be immediately accessible and some would only be accessible if certain missions are completed first, e.g., protection of Station X in order to be employed later by station Y.

The players will have the option to upgrade their space ships. Characteristics such as _speed_, _armour_, _shield_, _maneuverability_. Also they will be able to buy and upgrade weapons of different power and shooting range, e.g., some weapons would be more powerful in close range but less accurate. To buy weapons and upgrades players must spend space credits, which they will get for certain enemy kills and mainly from collecting garbage. Such style kills would be:
  * Destroying a large number of enemies in given period of time.
  * _Impressive kills_, e.g., destroy an enemy with long range weapon with single shot and then immediately shoot another in close range.

The ship a player chooses will have a garbage collection limit and in order for the ship to be able to collect more garbage player must buy upgrades. Upgrades can be bought at the beginning of each level. 

### Enemies

Enemies will be scripted for each level. They will appear from different locations on the map and they will move towards the space station area.

  * Tourists - Simplest of all enemies. They will approach the target area and stop at a  random distance then drop one junk item and leave.
  * Garbage ships - Similar to garbage trucks they hold a large amount of garbage. If not stopped, they will leave a big pile of junk floating around the space station. They will travel either alone or in convoy with mercenaries protecting the garbage ship against attacks from the player.
  * Multi-dimensional aliens - A race of little purple men. Their ships would be relatively small compared to humans. The form of their ships is the stereotypical round, circular with a kind of glass on top. They will move really fast and only in straight direction. They will leave traces of junk in the direction of movement.
  * Meteor shower - Meteors are approaching the space station. The player will have to destroy the threat.

The enemy types should be designed with different 3D models and textures to increase variety and minimize graphical repetitiveness.

### Level Design

The game action is in outer space. Every level consists of an target area that must be protected, i.e., clean of garbage.  The center of this area will be the space station being protected. The target area will have different radius depending on the size of space stations. 
Depending on space station type - human, alien, different kind of enemy ship models (and textures) will be spawned. Player would be able to move only in the range defined by the target area radius +/- some distance outside in order to 'meet' enemies approaching.

Each level may add to the in-game atmosphere by adding some flying metal boxes or low-poly objects floating around the space station. 

Player will have to protect each space station for given time. If in the define time period the junk indicator reaches critical level the mission would be considered unsuccessful and the game will end.

### Game levels & settings

Player would have the choice to select skins and logo graphical elements for her ship. Logos may be uploaded as images within the game.

Levels will be created using a Level editor. Therefore, players would have the possibility to create their own levels and plans of action. For example, a level may be created where scripted enemies appear from one direction and others from another direction. The script system would allow for details such as time and position of warping to be adjusted. The scripted levels should be part of some sort of Skirmish game mode which has nothing to do with player profile in Campaign mode.,


## Environment 

Game action will be carried out in outer space. A [skybox](http://en.wikipedia.org/wiki/Skybox_(video_games)) rendering could be used to simulate parallax view. Different tiles might be used depending on the level and solar system the player has chosen to play in. Additional artifacts like distant moons, moving meteors or pieces of scrap or passing ships in the distance could be rendered to increase realism.

## Camera 

The player would be given the option to choose whether he wants to play in firs-person or third-person view. He will have full control of the camera but in general he will be able to locate enemies on a radar display part of the user interface.

![Concept game screen](http://i.imgur.com/TrfUG7C.jpg)

## Controls

Players will use be done using mouse & keyboard. Keys and actions will be configurable in the game menu. Controls via joystick may also be added.

### Keys and buttons

  * *Up* - forward acceleration
  * *Down* - backwards acceleration
  * *Left* - left strafe
  * *Right* - right strafe 
  * *Mouse/Wheel* - Z-axis rotation
  * *Button1* - fire
  * *Button2* - alternative fire/weapon change (_configurable_)
  * *Button3* - weapon change

### Aiming

A crosshair will be displayed during playing in the center of the screen (fixed position). When player targets an enemy the crosshair will change size and color. For enemies located in close range the crosshair will increase in size and for distant enemies the corsshair size will decrease. 
Players should be allowed to choose different UI styles for the crosshair.

## Weapons

### Ammunition types

| Undepletable | Rockets/Projectiles | Energy based |
| -------------| --------------------| -------------|
| AE           | AR                  | AG           |

### Range types

| Close range | Long range | Inter-long range |
| -------------| --------------------| -------------|
| RC           | RL                  | RE           |

### Damage types

| Minor damage | Average damage      | Big damage   | Splash damage |
| -------------| --------------------| -------------| -------------|
| DS           | DM                  | DB           | DX           |

### List

Ammo | Range | Damage | Name      | Description                                                                            
------|-------|--------|-----------|--------------
AE | RC | DS | Dual-Machine Cannon | Shoots high speed large caliber shots. Does little damage but has endless ammunition. 
AR | RL | DB | Starfall Rockets | Long range rockets. 2 or 4 may be burst at a time.
AG | RE | DS | Lizard spheres | At sight these would look like little green spheres. Extremely fast but doing little damage. They are shout in bursts of 4 or 8 (alternative shot).
AG | RL | DM | Laser Cannon | Standard laser gun. Shoots in bursts. 
AG | RL | DB | Proton Beam | A high frequency energy beam which is shot like a laser from the point of the player's ship to some point in space (given range). If an enemy ship passes through the beam it will take damage for as long as the beam hits it. No alternative shooting.
AG | RC | DX | Mini-Antimatter Bomb | A small ball-shaped weapon which when detonated destroys absolutely all enemies in its range. It is detonated automatically upon being hit by an enemy or it may alternatively be detonated by the player.
AR | RC | DX | Cloak Mines | Much like land mines. They are invisible to enemies and if an enemy enters their range they will detonate doing some significant damage.  This is true also for the player's ship.

Every weapon, depending on ammo type and power will deplete a certain number of ammo shells. Player will be able to collect ammo from destroyed enemies or bonus crated spawned on the map.

### Bonuses & Collectables

Bonuses and items to collect would be available when the player destroys enemy ships or flies through metal boxes shown as glowing particles on the radar map. Player should also get bonuses for _impressive kills_; destroying many enemy ships one after another.

Bonus types available:

  * +n pts. armour
  * +n pts. energy
  * +n pts. rockets
  * Credits (_money_)
  * 5th Madness Pack - 5 times more damage and speed.
  * Mobile-Stations - Small turrets the player may spawn and place around the play field. They will exist only for certain period of time and they will automatically engage enemies.
  * Speed Boost - increases ship speed for certain amount of time.


___
© 2004 [KenamicK Entertainment](http://kenamick.com/)
