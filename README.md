# Maze

08/26/2017

Scott Hwang

snhwang@alum.mit.edu

Maze is the assignment for Project 3 of the Udacity Virtual Reality Nanodegree Program. The software is written for use with the Google Cardboard virtual reality (VR) system. The scene shows a maze through which the player must navigate through to find a key. The key unlocks the door of a temple which holds a treasure chest. Entering the Temple is the goal of the game.

## Implementation
The program is based on a template "starter" Unity project which was provided by Udacity. The Udacity VR forum on Slack was helpful for solving some of the problems and questions I had while finishing this project.

The project was completed using Unity 5.5.1f1 and Google VR 1.0. The submitted implementation is for the Android operating system. The submitted build was generated on Windows 10 computer and tested on a Samsung S8+ phone running Android 7.0. The program was built for a minimum level of Android 4.4 but was not tested on any other phone.

## Changes

### 8/26/2017
Since  version 1 from 8/25/2017, I implemented the changes recommended by the Udacity reviewer.

1) The key was visible from the starting point since I had placed in on top of the fountain. I replaced the fountain with a shorter pedestal to lower the altitude of the floating key so it is no longer viewable from other sites within the maze. I moved the fountain to near the starting point and placed a large rotating coin on its top.

2) I added a string parameter to the ResetScene function of the SignPost script so that the name of the scene after the reset can be specified in the Unity editor. Presumably, this will useful if other scenes are added later and the reset would then take the player to another scene if specified.

## Instructions
Navigate throught the maze by clicking on the waypoints (shown as light green cubes). Along the way, the player can pick up coins by clicking on them. Click on the key to obtain it. Obtaining the key automatically unlocks the door to the temple. Click on the door to open it. In the temple, there is a a treasure chest and a sign indicating the player's victory. Clicking on the sign resets the game.

## Notes and Modifications

1) The audio files that were provided in the template for the door opening and door closing were difficult to hear. I amplified them externally using Audacity (https://sourceforge.net/projects/audacity/) then imported them back into Unity. I reduced the volume of the background ambient sound using the Unity editor.

2) I used the Unity Asset, Mesh Baker (by Ian Deane, found at the Unity Asset Store), to combine most of the wall elements for the maze.

3) One waypoint is high above the maze. This was placed just for the purposes of obtaining the screenshot which is included with my submission.
