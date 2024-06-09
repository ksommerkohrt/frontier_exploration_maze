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

ros2 launch frontier_exploration classical_exploration.launch.py

