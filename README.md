JelloShot
-------------------------------------
[Asset Store Link](http://u3d.as/15gd)  
© 2017 Justin Garza

PLEASE LEAVE A REVIEW OR RATE THE PACKAGE IF YOU FIND IT USEFUL!
Enjoy! :)

## Table of Contents

* [Contact](#Contact)
* [Description/Features](#Description-Features)
* [Terms of Use](#Terms-of-Use)
* [Overview](#Overview)
* [Folder Structure](#Folder-Structure)
* [Scripts](#Scripts)
	* [GameManager.cs](#GameManager.cs)
	* [LevelMaker.cs](#LevelMaker.cs)
	* [Themer.cs](#Themer.cs)
	* [PlayerDataManager.cs](#PlayerDataManager.cs)
	* [Other Scripts](#Other-Scripts)



## Contact  

Questions, suggestions, help needed?  
Contact me at:  
Email: jgarza9788@gmail.com  
Cell: 1-818-251-0647  
Contact Info: [justingarza.info/contact](http://justingarza.info/contact/)  
Alternate Website: [jgarza9788 - UnityPortfolio](https://github.com/jgarza9788/UnityPortfolio)  


## Description Features

Displays an energy shield/force field effects when impacted by projectiles, or raycasts.

* Easily customizable effect. Size, Color, * Speed, etc.
* Renders on simple and complex meshes.
* Simultaneous impact points support.
* Support for culling and non-culling.
* Distortion and Color!
* Unity Free friendly.
* Fully commented C# code.
* Awesome demos!


## Terms of Use

You are free to add this asset to any game you’d like
However:  
please put my name in the credits, or in the special thanks section. :)  
please do not re-distribute.  

## Overview

The JelloShot is a pretty basic game.
the Main Menu has buttons for Info, Menu/Toggles, Leaderboards, Play, and Customize/Shop.

![Imgur](https://i.imgur.com/EJmCmdz.png)

Game Play is just draging and letting go.

![Imgur](https://i.imgur.com/rxwxrU8.gif)

Customize/Shop is where users can spend coins to unlock 35 different jello characters.

![Imgur](https://i.imgur.com/ojw54Gl.png)

![Imgur](https://i.imgur.com/Mq9weOs.png)

![Imgur](https://i.imgur.com/BF8Cljg.png)

## Folder Structure

JelloShot contains a collection of other systems and resources, therefore the folder structure might seem a little confusing until you understand the systems and resources it is composed out of.

![Imgur](https://i.imgur.com/6pHbFkq.png)

**JellyObject**   
This contains my JellyObject asset from the asset store.

**JellyObject_CustomStuff**   
This contains scripts and resources to customize my JellyObject Asset.
(such as a special collision script)

**kenney.nl**  
Resources (mostly images/sprites) i obtains from Kenney's website.
(i will be donating a portion of the profit from this asset to him, but feel free to donate to him also)

**ParticleManipulator**  
This contains my ParticleManipulator Asset.
It allows particles to be sucked into the corner of the screen.

**PlayerAssets**  
This contains assets required by the different jello characters. (mostly emoji's)

**PoolManager**  
This contains assets PoolManager Script(s)

**SceneSwither**  
This contains the assets/scripts for the change screen effect(s).

**SimpleAudio**  
This contains the scripts for audio adjustments.


## Scripts 
below is a list of some of the key scripts that this game uses.

### GameManager.cs
This script manages the game's state.
Possible states include; BEGIN, PLAY, PAUSE, GAMEOVER.

![Imgur](https://i.imgur.com/mJBWuvB.png)

here are some of the variables and functions...

**StatePrev**  
the previous state of the game

**State**  
the current state of the game

**DistanceText**  
displays how far the player got (both last try, and best)

**DistanceStorage**  
when the player loops (goes throught the portal) this variable stores their distance to be added later

**ExtraPointButton**  
A Reference to the button that allows the player to gain extra points at the end of their try.

**ExtraPointCountText**  
The Text Object that shows how many extra points the player could gain.

**ExtraPointCount**  
The number of extra points the player will get.

**GameId_iOS**  
An Ad Id for iOS

**GameId_Android**  
An Ad Id for Android

**ShareVideo0**  
The first image for the ShareVideo button

**ShareVideo1**  
The second image for the ShareVideo button

**SetState(States NextState)**
switches the state of the game


### LevelMaker.cs
Creates and re-creates the level.

![Imgur](https://i.imgur.com/nyohNJ5.png)

here are some of the variables and functions...

**startLevelItem**  
The start level prefab ...the level will always start with this platform.

**endLevelItem**  
The end level prefab ...the level will always end with this platform.

**restartLevelItem**  
The portal that restarts the level

**levelItems**  
This is the pool of platforms (LevelItems) that each levels get made out of.

**spacing**  
The spacing between each platform

**levelItemCnt**  
how many levelsItems are each level

**createLevel()**
Creates the level.

**RebuildLevel()**  
Rebuilds the level after going through the portal.


### Themer.cs
Themes the level each time you play

![Imgur](https://i.imgur.com/IFqtSkM.png)

here are some of the variables and functions...

**GroundSpriteAtlas**  
The ground sprite atlas.

**BackgroundMaterial**  
The background material.

**backgrounds**  
The backgrounds.

**theme**  
The current theme (changes randomly).

**applyThemeOnAwake**  
The apply theme on awake (allow GameManager to apply theme).

**ApplyTheme(bool newTheme)**  
Applies the theme.

### PlayerDataManager.cs
controls/manages the data for each jello character.

![Imgur](https://i.imgur.com/m6YpoQh.png)

here are some of the variables and functions...

**key**  
The key.(basically the prefab name)

**minDistance**  
The minimum distance to be able to buy this character

**Cost**  
The cost of this character

**minDistanceLock**  
is this locked because of the distance

**Locked**  
The locked. (or not purchased yet)

**defaultPlayer**  
The default player.


### Other Scripts
Many other scripts are commented, however some are not.
Please feel free to reach out if you have any questions.









