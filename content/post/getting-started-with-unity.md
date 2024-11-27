+++
date = '2024-11-11T17:52:20+01:00'
draft = true
title = 'Getting Started With Unity VR and the Meta Quest VR Headset'
+++

To make our VR dreams become reality us students were given a Meta Quest VR headset. We could either get a Meta Quest 2 or 3. I got a Meta Quest 2. I already set this headset up before for another university course, but at that time I was unaware that the Meta Quest Link app exists, which makes debugging a lot easier. For my previous project I was reading out logs to debug (yes it was painful). So this time I installed the Meta Quest Link app and the unity version we needed for the Unity project we were given.

To get started I used a finished version of the [Unity 3D Beginner: Roll-a-Ball Game](https://learn.unity.com/project/roll-a-ball) we were given within our course. Our task was then to turn this project into a VR project.

I simply followed the instructions from the course:
- export the non-VR Roll-a-Ball Game as a package
- import the non-VR Roll-a-Ball Game as a package in a new project
- set up the project as a VR project
    - create a floor
    - add an OVR Interaction Rig and delete the main camera
    - change the controller setting to touch in the left and right controller
- then resize the original Roll-a-Ball-Game content however needed (I had to scale it down a lot)
- change the canvasses so they work well in VR:
    - Render Mode: World Space
    - replace old texts with TMP texts and update the scripts accordingly
- remove the speed variable and Update function from the PlayerController script, which controls the ball
    - we don't need it anymore, because the ball has a Rigidbody component, which reacts to physics: the ball will move, when the player moves the board
- finally, add a grab interaction via right click > Interaction SDK on the board and it's done

The final game then looked like this: image here
