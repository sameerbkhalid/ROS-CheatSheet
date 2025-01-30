# ROS Cheat Sheet

## ROS 1 Basics

### Setup
```bash
source /opt/ros/noetic/setup.bash   # Load ROS environment
roscore                              # Start ROS Master
```

### Nodes & Topics
```bash
rosrun <package> <node>              # Run a node
rosnode list                         # List active nodes
rosnode info <node>                   # Get node info
rostopic list                         # List available topics
rostopic echo <topic>                 # View topic data
rostopic pub <topic> <type> <msg>     # Publish data to a topic
rostopic info <topic>                 # Get topic info
```

### Messages & Services
```bash
rosmsg show <message_type>            # Show message structure
rossrv list                            # List all available services
rossrv show <service_type>             # Show service definition
rosservice call <service> <args>       # Call a service
rosservice list                        # List services
```

### Package & Workspace
```bash
catkin_make                           # Build the workspace
source devel/setup.bash               # Source the workspace
roscd <package>                       # Navigate to package directory
rospack list                          # List installed packages
rospack find <package>                # Find package path
```

## ROS 2 Basics

### Setup
```bash
source /opt/ros/humble/setup.bash     # Load ROS 2 environment
```

### Nodes & Topics
```bash
ros2 run <package> <node>             # Run a node
ros2 node list                        # List active nodes
ros2 node info <node>                  # Get node info
ros2 topic list                        # List topics
ros2 topic echo <topic>                # View topic data
ros2 topic pub <topic> <type> <msg>    # Publish to a topic
ros2 topic info <topic>                # Get topic info
```

### Messages & Services
```bash
ros2 msg show <message_type>           # Show message structure
ros2 service list                      # List all available services
ros2 service type <service>            # Show service type
ros2 service call <service> <args>     # Call a service
```

### Package & Workspace
```bash
colcon build                          # Build the workspace
source install/setup.bash             # Source the workspace
ros2 pkg list                         # List installed packages
ros2 pkg create <package_name>        # Create a new package
```

### Other Useful Commands
```bash
rviz2                                 # Start RViz visualization tool
gazebo                                # Start Gazebo simulator
```
