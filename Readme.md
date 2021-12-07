## <u>TurtleSimFollowingRobot </u>
#### This repo, it is assignment for the autonomous robots course given by [Asst. Prof. Haluk BAYRAM](https://avesis.medeniyet.edu.tr/haluk.bayram) which i took while  i was doing my master's degree at Istanbul Medeniyet University.
-----------

### General Description
There are two turtle robots in the application. One of them is responsible for following the other from a distance. The distance can be set in the json file.

### Dependencies
- [Json Library](https://github.com/eteran/cpp-json)
### To Build
1. if you don't have ros installations your system and you are using ubuntu 20.4 distro. You can use my script. It's called rosinstallation.sh
    ```bash
    source rosinstallion.sh
    ```
2. Creating a catkin workspace
    ```bash
    mkdir catkin_ws
    cd catking_ws
    mkdir src
    catkin_make
    ```
3. Cloning the repository and building
    ```bash
    cd ~/catkin_ws/src
    git clone https://github.com/volkanunal/TurtleSimFollowingRobot.git
    cd ..
    catkin_make
    ```

### To run
1. Run roscore from terminal
    ```bash
    roscore
    ```
2. Run TurtleSim 
    ```bash
    rosrun turtlesim turtlesim_node
    ```
3. To run the project and see the output in the TurtleSim
    Open Terminal:
    ```bash
    cd ~/catkin_ws/src
    source devel/setup.bash
    rosrun hw3 follower_robot
    ```
    Open Another Terminal:
    ```bash
    source devel/setup.bash
    rosrun hw3 control_robot
    ```

## Demonstration

<p align="center">
  <img src="output/output.gif" />
</p>

    

      
    
