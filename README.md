# ShapesDemo-TypeSupport

Shapes Demo TypeSupport package to use with [eProsima Fast DDS Shapes Demo](https://www.github.com/eProsima/ShapesDemo) on ROS 2 installations.

It can be built on a ROS 2 environment by running:

    $ colcon build

It can then be used to interact with topics created by Shapes Demo like so:

    $ source install/setup.bash
    $ ros2 topic echo /Square
    color: RED
    x: 175
    y: 215
    shapesize: 30
    ---
    color: RED
    x: 169
    y: 210
    shapesize: 30
    ---

    $ source install/setup.bash
    $ ros2 topic pub /Square shapes_demo_typesupport/idl/KeylessShapeType "{ color: BLUE, x: 155, y: 150, shapesize: 30}"
    publisher: beginning loop
    publishing #1: shapes_demo_typesupport.idl.KeylessShapeType(color='BLUE', x=155, y=150, shapesize=30)
