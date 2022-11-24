# Installing and configuring ROS Noetic

1. To install ROS Noetic on your ubuntu PC, just follow the wiki instructions as depicted [here](http://wiki.ros.org/noetic/Installation/Ubuntu).
2. Additionally, you will need to install catkin tools for python 3:
```sh
sudo apt install python3-catkin-tools
```
3. Create your catkin workspace from your desired path as:
```sh
mkdir -p catkin_ws/src
cd catkin_ws/
```
4. For building the workspace, our preferred command is catkin build:
```sh
catkin build
```
## Known issues and how to address them

- If you get into an error with Python libraries when compiling your workspace, you can first test which is your PYTHONPATH
  ```sh
  echo $PYTHONPAT
  ```
  If the Python path is not the one from where you want to compile your workspace, you can change it when compiling as:
  ```sh
  catkin build -DPYTHON_EXECUTABLE=/usr/bin/python3
  ```
 - More problems to come!
