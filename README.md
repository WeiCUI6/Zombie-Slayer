# Zombie-Slayer

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Game Description: a First-Person Shooter game which you can use your weapons (AK47 or M4A1) to shoot and kill zombies ambushed in the woods. This game is a personal project and is based on the Unreal Engine 4.26

## Requirement

[Unreal Engine 4.26](https://www.unrealengine.com/en-US/)

## Game logic and functionality

* Game interface
  * **Player's HP and Armor**: on the bottem left corner
  * **The minimap (radar)**: on the top left corner to let you get information about your current location and zombies' location
  * The **message panel**: at the bottem of the minimap, which shows status of your current object (e.g. Kill all zombies)
  * The **Timer**: on top of the minimap (radar)
  * A **gun (AK-47)**: is always your first equipped gun, and the icon is shown on the bottem right corner
  * **Ammo Count**: on bottem right corner
  * A **shooting sight** is always in the center of the screen
  <img src="Images/3.jpg" style="width:500px"></img>
  
  * Player models
  * All the original models and their animations were found from **[Mixamo](https://www.mixamo.com/)**, which is a pretty good game model website run by Adobe
  * There are three types of player **models**:
    * **Policeman**: a policeman-like model with yellow skin
    * **RobotX**: a robot-like model with dark pink skin
    * **RobotY**: a robot-like model with dark blue skin
    * <img src="Images/9.jpg" height="200px"></img> <img src="Images/11.jpg" height="200px"></img> <img src="Images/10.jpg" height="200px"></img>

  * **Animations**:
    * **Walk** towards four different directions
    * **Run** towards four different directions
    * **Jump** without affecting upper part body (**achieved by unity3d body mask**)
    * **Shoot** without affecting lower part body (**achieved by unity3d body mask**)
    * **Unity Blend Tree**
      * This makes the player walk or run more naturally. It uses interpolation function to map different combinations of user input to different animations.
      * ![img](Images/4.jpg)

  * **State Machine**
    * There are multiple layers in the player state machine.
    * <img src="Images/5.jpg" style="width:420px"></img>
    * <img src="Images/6.jpg" style="width:420px"></img>
    * <img src="Images/7.jpg" style="width:420px"></img>
    * <img src="Images/8.jpg" style="width:420px"></img>

* Player movement
  * Walking && Running && Aiming
    * <img src="https://cloud.githubusercontent.com/assets/5276065/12594065/02a72084-c429-11e5-84b7-39de1a51d991.jpg" style="width:420px"></img>
    * <img src="https://cloud.githubusercontent.com/assets/5276065/12594070/02be2234-c429-11e5-874a-880a710742c1.jpg" style="width:420px"></img>
    * <img src="https://cloud.githubusercontent.com/assets/5276065/12594601/c34c19f0-c42b-11e5-9c90-2f2e384030ef.jpg" style="width:420px"></img>
    * <img src="https://cloud.githubusercontent.com/assets/5276065/12594069/02b960be-c429-11e5-90b1-49e0ff6be56a.jpg" style="width:420px"></img>
  * Jumping
    * <img src="https://cloud.githubusercontent.com/assets/5276065/12594068/02b1568a-c429-11e5-9bbe-cee8760c079b.jpg" style="width:420px"></img>
  * Dying
    * <img src="https://cloud.githubusercontent.com/assets/5276065/12594067/02abdd9a-c429-11e5-887f-0c830090ff49.jpg" style="width:420px"></img>
    * <img src="https://cloud.githubusercontent.com/assets/5276065/12594066/02aa6d34-c429-11e5-86ce-ef458bb7f7c3.jpg" style="width:420px"></img>

* Gun model
  * The original gun model (AK-47) was from Unity Assets Store
  * **Shooting animation are added** by setting keyframes in unity3d animation panel
  ![img](Images/12.jpg)

* Bullet effects
  * Bullets hitting different materials will cause different effects
    * Wood
    <img src="Images/13.jpg" style="width:510px"></img>
    * Ground
    <img src="Images/14.jpg" style="width:510px"></img>
    * Metal
    <img src="Images/15.jpg" style="width:510px"></img>
    * Concrete
    <img src="Images/16.jpg" style="width:510px"></img>
    * Water
    <img src="Images/17.jpg" style="width:510px"></img>
    
    
## License

[MIT License](https://github.com/Armour/Multiplayer-FPS/blob/master/LICENSE)
