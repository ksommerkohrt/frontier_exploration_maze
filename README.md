# frontier_exploration

## Description
A frontier exploration module implementied with ROS 2, C++, and Python. Based on:

```
B. Yamauchi, "A frontier-based approach for autonomous exploration," Proceedings 1997 IEEE International Symposium on Computational Intelligence in Robotics and Automation CIRA'97. 'Towards New Computational Principles for Robotics and Automation', Monterey, CA, USA, 1997, pp. 146-151, doi: 10.1109/CIRA.1997.613851.
```

*Please note that this repository is a forked version of https://github.com/adrian-soch/frontier_exploration.git with minor edits to create a sample solution for a maze competition

> **Frontier Exploration**: Contains nodes for autonomous exploration, interfaces with the nav2 stack.

> **Frontier Interfaces**: Contains a custom ROS 2 service interface.

> **Learned frontier detector**: Contains scripts and tools for training and deploying a learned frontier detector.

## Getting Started

To get ready for development or execution:
```
# Clone the repo
git clone https://github.com/adrian-soch/frontier_exploration

# Build
colcon build
```

To run the exploration node:
```
# Start cognipilot simulation

ros2 launch frontier_exploration exploration.launch.py

### Training Data Collection

1. Launch a simalation or real robot that publishes occupancy grid maps to the `/map`  topic.
2. Then `ros2 run frontier_exploration collection_node`
   - This will preprocess the map through simple filtering operations
   - Save a map after the robot has travelled beyond a distance threshold


## Dataset

<a href="https://universe.roboflow.com/cas726/learned-frontier-detection">
    <img src="https://app.roboflow.com/images/download-dataset-badge.svg"></img>
</a>

Our dataset is available at the link above.
