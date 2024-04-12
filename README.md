Fun C++ project where I used multi-threading in order to make a little gravity engine and sandbox where you can stack randomly chosen blocks together or take down little towers of blocks. It also has bouncing balls which slowly will stop bouncing or will collide with other falling objects or static objects on the ground. 

<img src="https://github.com/Kingerthanu/CPP_physicsEngine/assets/76754592/7cddc143-60bf-474e-909c-ca647f217e8e" alt="Cornstarch <3" width="95" height="159">

Project helped me in a lot of sectors in pipelining and trying to make streamlined code for differing objects. I also tried abstractifying things a little more and giving better interfacing to myself which was a benefit. Make sure you export this with all the .dlls if you want to run this Qt is kinda jank and have been trying to use openGL more.



----------------------------------------------

<img src="https://github.com/Kingerthanu/CPP_physicsSandBoxEngine/assets/76754592/b96e1c49-626c-415d-8543-11910143838d" alt="Cornstarch <3" width="55" height="49"><img src="https://github.com/Kingerthanu/CPP_physicsSandBoxEngine/assets/76754592/b96e1c49-626c-415d-8543-11910143838d" alt="Cornstarch <3" width="55" height="49"><img src="https://github.com/Kingerthanu/CPP_physicsSandBoxEngine/assets/76754592/b96e1c49-626c-415d-8543-11910143838d" alt="Cornstarch <3" width="55" height="49"><img src="https://github.com/Kingerthanu/CPP_physicsSandBoxEngine/assets/76754592/b96e1c49-626c-415d-8543-11910143838d" alt="Cornstarch <3" width="55" height="49">


**The Breakdown:**

  This C++ Program Works With The QT Framework In Order To Create A Window To Simulate A Simple Multi-Threaded Physics Engine.

  This Program Starts Initially By Creating Two Main Threads. One Will Be Our Physics Engine And The Other Will Be Our Window. 

  Firstly We Will Create Our Window; This Will Work As The Object In Which Holds And Maintains Our Worldspace. On Top  Of This Job It Will Consist Of Defining Our Size Of Window, As Well As Some Flags Like Ensuring Resizing Is Not Possible To Make Sure We Dont Have Unexpected Behaivor. We Also Will Call Upon A Button Class We Made In Which Sends A Signal Back To The Window When Pressed Telling It To Execute The Calls In The Map For Its Execution.

  The Two Buttons We Have Are To Either Spawn A Block Or Circle. 

  Each Object Type Has Unique Properties That Govern How It'll React In Our Worldspace.

  For A Block, It Will Be In A Constantly Sized Square Shape. This Square Shape Will Be Filled In With A Random Texture Grabbed At Instantiation. This Pool It Selects From Holds Only 3 Sprite-Textures.

  A Block Will Want To Fall To Ground Level All The Time But Can Be Interrupted By Other Block Instances Or Circles.

  A Circle Will--Under The Hood--Be A Square Likewise But Using A Circle Texture Will Give THe Illusion of It Being A Circle While Its Collision Box Is Actually A Square.

  A Circle When Instantiated Will Also Always Want To Reach The Floor Of Our Worldspace. When It Reaches It Though It Will Rebound Upwards, Proportional To The Height It Was Dropped From Minus Some Frictional Falloff. This Means When A Circle Falls, If It Collides With Something Like A Cube Or The Floor (Out Of Bounds) It Will Then Divert Its Velocity To Make It Go Upwards To Simulate It Bounding Up And Down.

  A Circle Will Also Have A Varying Amount Of Sprite Textures That It Could Use During Initialization As We Have Also 3 The Instance Will Randomly Choose From.

  All These Movements Will Be Done By A External Thread Running Our Physics Engine.

  The Physics Engine Will Be Fed In The Window It Will Be Associated With And Will Grab Its Current Entities To Do Actions Upon Them In The Worldspace. This Allows Our Physics To Be Done Independently From Our Windows Execution Thread Itself For Runtime As Well As Encapsulation/De-Coupling Principles. 

  This Program Taught Me A Lot Of Major Principles In Designing Software As I Saw This Program As Quite Daunting As I Wanted To Ensure Everything I Was Doing Was 100% Understood Through And Through So Even Things Like Setting Up Our MainWindow Were Huge Feats As I Tried Using No "Cheats" And Read Documentation Thoroughly Instead Of Trauma Dumping On Stack Overflow. While QT Is Annoying And Even Making A Window Should Be Celebrated, I Did Enjoy The Learning Experience From It As Even Though This Project Seems Quite Dainty I See It As One Of My Proudest Works Just From The Amount Of Things I Learned And Did To Ensure This Project Worked Properly Without Pushing A Lot Of Actions Off To Random Library Functions To Do The Heavy Lifting For Me.
  

<img src="https://github.com/Kingerthanu/CPP_physicsSandBoxEngine/assets/76754592/f19ff9a0-2f81-4fb9-a02d-0242fb998b0f" alt="Cornstarch <3" width="55" height="49"><img src="https://github.com/Kingerthanu/CPP_physicsSandBoxEngine/assets/76754592/f19ff9a0-2f81-4fb9-a02d-0242fb998b0f" alt="Cornstarch <3" width="55" height="49"><img src="https://github.com/Kingerthanu/CPP_physicsSandBoxEngine/assets/76754592/f19ff9a0-2f81-4fb9-a02d-0242fb998b0f" alt="Cornstarch <3" width="55" height="49"><img src="https://github.com/Kingerthanu/CPP_physicsSandBoxEngine/assets/76754592/f19ff9a0-2f81-4fb9-a02d-0242fb998b0f" alt="Cornstarch <3" width="55" height="49">


----------------------------------------------

<img src="https://github.com/Kingerthanu/CPP_physicsSandBoxEngine/assets/76754592/f4948d81-f91b-4b42-ac1a-cd4553ff385f" alt="Cornstarch <3" width="55" height="49"> <img src="https://github.com/Kingerthanu/CPP_physicsSandBoxEngine/assets/76754592/f4948d81-f91b-4b42-ac1a-cd4553ff385f" alt="Cornstarch <3" width="55" height="49"> <img src="https://github.com/Kingerthanu/CPP_physicsSandBoxEngine/assets/76754592/f4948d81-f91b-4b42-ac1a-cd4553ff385f" alt="Cornstarch <3" width="55" height="49"> <img src="https://github.com/Kingerthanu/CPP_physicsSandBoxEngine/assets/76754592/f4948d81-f91b-4b42-ac1a-cd4553ff385f" alt="Cornstarch <3" width="55" height="49">


**Features:**

![2024-01-1001-25-52-ezgif com-video-to-gif-converter](https://github.com/Kingerthanu/java_physicsEngine/assets/76754592/10dea34c-5ad5-412c-a9cf-c44448df58f6)


<img src="https://github.com/Kingerthanu/CPP_physicsSandBoxEngine/assets/76754592/1c477bd2-475c-434b-9488-4f929a171f53" alt="Cornstarch <3" width="55" height="49"> <img src="https://github.com/Kingerthanu/CPP_physicsSandBoxEngine/assets/76754592/1c477bd2-475c-434b-9488-4f929a171f53" alt="Cornstarch <3" width="55" height="49"> <img src="https://github.com/Kingerthanu/CPP_physicsSandBoxEngine/assets/76754592/1c477bd2-475c-434b-9488-4f929a171f53" alt="Cornstarch <3" width="55" height="49"> <img src="https://github.com/Kingerthanu/CPP_physicsSandBoxEngine/assets/76754592/1c477bd2-475c-434b-9488-4f929a171f53" alt="Cornstarch <3" width="55" height="49">

