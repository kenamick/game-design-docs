Paramount Warlocks
========================

_(Design document/Game spec. in progress)_

## Foreword

When I first bought an Android powered smartphone, I immediately searched in the Marketplace for a game called - Archon.  This is a title from 1983 (How nice! The year I was born in.) distributed by EA (Electronic Arts at that time) in which you take control of a Light or Dark side wizard and his army. There is a chess-like game board on which the creatures and the wizard are positioned and you may move them around and fight against enemy creatures.

![Archon Game](http://i.imgur.com/Ihue1NI.png)

I don’t think a lot of people remember this title which is a shame since it introduced some really remarkable ideas for its time. It was remarkably easy to start playing. No advanced or detailed tutorials were required. It was just like you know how to play before you’ve even seen it. In 1994 the original team from Free Fall Associates developed a remake  called Archon Ultra which features better graphics and effects.

![Archon Ultra](http://i.imgur.com/UCZgCy7.png)
![Archon Ultra Battle](http://i.imgur.com/MO3MO7N.png)

What is also quite interesting is that even though it is a turn-based strategy the battles between creatures are in real time and you can control the movement and attack when in battle mode.

For some time I was thinking how to mix the powerful gameplay of Archon with the great in-game atmosphere of the game Heroes of Might and Magic 2. Now, you would notice I’m talking about version 2 of HOMM simply because this is the only version from the series that brought a great feeling of fantasy to me. It was probably a combination of graphics and music that made this happen but playing HOMM2 seemed like being always a part of an unique and pleasant adventure.

![HOMM2 Battle](http://i.imgur.com/EO2hpQ8.png)
![HOMM2 Map](http://i.imgur.com/tSTEpRP.png)
 
_(HOMM2 is game that features various creates and characters from Greek & Celtic mythology, Tolkein’s Hobbit and others)_

## Concept

The idea I have is to create game which features the simplicity of gameplay of Archon combined with the battle mechanics of HOMM2 added by an atmosphere of mysticism and sorcery. And of course, I have a lot of ideas I want to add to this already established base. 

* Player vs. Player or Player vs. AI TBS game.
* Isometric 2D terrain as game board.
* Using the four seasons - Winter, Spring, Summer, Autumn to empower warlocks magic powers and creatures damage.
* 4 warlock archetypes will be available in the game. Each with power boost for given season.
* Warlocks will have mana/energy and can summon creatures on the game board or cast attack or defense kind of spells.
* There will be static positions on the map which will give extra mana or healing power to the player that occupies them.
* Any type of creature may be summoned by any of the warlock archetypes. Some creatures will have favourable properties only if summoned by specific warlock archetype, e.g., a polar bear would have more attack or defense points if summoned by Winter Warlock.
* Random items - boosts, power ups, artefacts will be spawned on the map. A player would have to move his creature to that position to pick up the item.
* There will be no separate battle dynamics like in Archon. Creatures will attack enemy creatures directly on the game board.

This is a TBS game so players will play in turns and in each turn they can decide if they want to:
* Move a creature
* Cast a spell
* Attack enemy creature

Warlocks will be something like ingame heroes or commanders. The enemy player may kill a warlock but this would not end the game. Not until the last creature on the board falls.

## Release Goals
The target goal is to create a HTML5/Javascript game than can be played in the Web browser or on mobile devices. So, we need to support
* Web Browsers - Chrome, FireFox, Safari, IE10+
* iOS devices - iPhone, iPad
* Android devices - Tablets
* Windows 8 devices

The first goal is to create the game for Web browsers and Tablet devices. It can then be optimized to support smaller screens, e.g., iPhone, Android smartphones.

Because we want to support different devices we must use a common way to build the game for different platforms. There are some services that offer this for free:
* Adobe [PhoneGap](https://build.phonegap.com/) build
* [CocoonJS](http://www.ludei.com/) by Ludei
* [GameClosure](http://www.gameclosure.com/)


