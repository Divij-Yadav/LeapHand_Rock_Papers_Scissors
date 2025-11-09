# LeapHand_Rock_Papers_Scissors

# **Overview**


This project focuses on creating an interactive and immersive **Rock-Paper-Scissors** game using the **Leap Motion Controller** to track hand gestures in real-time. The game leverages the Leap Motion’s hand-tracking capabilities to recognize the user's hand gestures and respond with a counter gesture, allowing players to compete in both **competitive** and **casual modes**.

### 1. **Objective and Scope**

The primary goal of this project was to develop a system where the user interacts with a digital environment via hand gestures, playing the classic game of **Rock-Paper-Scissors**. The Leap Motion Controller, connected to a camera, captures the user’s hand movements and translates them into corresponding gestures: Rock, Paper, or Scissors. Once the user makes a gesture, the system identifies it and generates an opposing gesture, mimicking the competitive aspect of the game. The two modes—**competitive** and **casual**—offer different levels of interaction and complexity, with competitive mode being more focused on accurate, quick responses, while casual mode offers a more relaxed experience.

### 2. **Gesture Recognition with Leap Motion**

The core of this project relies on **real-time gesture recognition** through the **Leap Motion Controller**.  Through software developed in conjunction with the Leap Motion SDK, the system identifies hand gestures as follows:
- **Rock**: A clenched fist.
- **Paper**: An open hand with fingers extended.
- **Scissors**: A fist with the index and middle fingers extended.

Once the user’s gesture is detected by the Leap Motion system, the software interprets it and compares it to the predefined gestures to determine the correct action.

### 3. **Game Flow and Modes**

The game operates in two distinct modes, each providing a unique gameplay experience:

- **Competitive Mode:** In this mode, the system tracks the user’s hand gestures in real-time, challenging the player to react quickly and accurately. After the user makes their gesture, the system generates a counter gesture based on the standard rules of Rock-Paper-Scissors (Rock beats Scissors, Scissors beats Paper, Paper beats Rock). The winner is immediately determined, and the game progresses rapidly. This mode emphasizes speed and precision, providing a dynamic and engaging experience.

- **Casual Mode:** This mode is designed to be more relaxed and focuses on a fun, leisurely experience. While the system still tracks gestures in real-time, there’s less pressure for immediate responses. The counter-gesture from the system is slower and provides more time for the player to observe and respond. It’s ideal for beginners or those looking to play a less competitive, stress-free version of the game.

### 4. **Real-Time Interaction and Counter Pose Generation**

A key feature of the project is the real-time feedback loop between the user’s input and the system’s response. After detecting the user's hand gesture, the system immediately generates a counter pose using the same hand-tracking capabilities. The counter-gesture is based on the rules of Rock-Paper-Scissors and is displayed on-screen, where the user can see both their own gesture and the system’s gesture at the same time.

This interaction happens instantaneously, making the gameplay feel more fluid and responsive. Additionally, the system’s gesture is not pre-programmed; it dynamically chooses a gesture based on the user’s input, ensuring a unique experience with every round.

<br>

# **Hardware Requirements**

Leap Hand Hardware
<br>

# **Installation procedures**

<br>

1. Install Dependencies using the following commands;
   
   1.1 `pip install empy==3.3.4 catkin_pkg pyyaml rospkg`

   1.2 `pip install dynamixel_sdk numpy`

<br>

2. Make a new workspace and clone the Leap Hand API using the command

   2.1 `mkdir -p ~/leap_hand_ws/src`

   2.2 `cd ~/leap_hand_ws/`

   2.3 `cd src`

   2.4 `git clone https://github.com/leap-hand/LEAP_Hand_API/tree/main/ros_module`

   2.5 `cd LEAP_Hand_API`

   2.6 `git clone https://github.com/Demolus13/Hand-Gesture-Recognition-Model.git`
   
   2.7 `catkin_make`

   2.8 `source devel/setup.bash`

<br>

# **Tutorial**

<br>

1. Create a script `rock_paper_scissors.py` in `LEAP_Hand_API` folder

2. Make the program file executeable using the command 

   `chmod +x rock_paper_scissors.py`

3. Open a terminal and type the command 

   `roslaunch leap_hand example.launch`

4. Open another terminal and type the command 

   `rosrun leap_hand rock_paper_scissors.py`

<br>

# **Results**


This project successfully demonstrated the use of the **Leap Motion Controller** for real-time hand gesture recognition, enabling an interactive Rock-Paper-Scissors game in both competitive and casual modes. By using the Leap Motion’s hand-tracking technology, we created an engaging experience that combines classic gameplay with cutting-edge gesture recognition.


<br>

# **Future Work**


Looking ahead, there are several potential improvements and enhancements:
- **Enhanced Gesture Library:** Expanding the game to recognize additional hand gestures could add variety and complexity to the game, such as adding new game modes or interactions beyond Rock-Paper-Scissors.
- **Multiplayer Capabilities:** Introducing multiplayer functionality, where players can compete against each other using their respective hand gestures, could add a social dimension to the game.
- **Improved Visual Feedback:** Enhancing the visual representation of gestures, including adding animations or 3D models for hand poses, could make the game more immersive and visually engaging.
- **Advanced AI Counter-poses:** Implementing more sophisticated artificial intelligence to make the system’s gesture selection more challenging or unpredictable could increase the competitiveness of the game.

Overall, this project provided valuable insights into real-time gesture recognition, offering a unique and engaging way for users to interact with a classic game using modern hand-tracking technology.


<br>

# **References**

<br>

Leap Hand documentation

https://leaphand.com/ 

Leap Hand API

https://github.com/leap-hand/LEAP_Hand_API/tree/main/ros_module

Hand recognition model 

https://github.com/Demolus13/Hand-Gesture-Recognition-Model/tree/main

<br>

# **CONTRIBUTORS**

<br>

Divij Yadav (M.Tech Mechanical Engineering student, IIT Gandhinagar)

Chetan Sharma (PhD Mechanical Engineering scholar, IIT Gandhinagar)   

Dharmesh Makvana  


