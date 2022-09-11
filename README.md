# Roid1 (執筆途中)

Roid1 is a URDF file of a small humanoid robot Roid1 and it's Rviz operation demo.
You can operate the joints of the robot with sliders.
  
And you can also import this URDF file into Unity via URDF-importer.

Roid1は小型ヒューマノイドロボットのURDFファイルです。
Rvizでモデルを表示し、スライダーで関節を曲げることができます。
また、URDF-importerを使いUnity上にモデルをインポートすることもできます。

# Usage (View in Rviz)

This demo has been confirmed to work on ROS-melodic,noetic with Rviz.
Rviz用のデモはROS-melodic,noeticのRvizで動作確認しています。

$ cd ~/catkin_ws/src/

$ git clone https://github.com/Ninagawa123/roid1.git

$ cd ~/catkin_ws/

$ catkin build

$ source ~/catkin_ws/devel/setup.bash

$ roslaunch roid1 display.launch

# Usage (View in Unity)

あとで書きます。

# Directory Tree

<pre>
~/catkin_ws/src/
└── roid1_urdf #ros_package
    ├── CMakeLists.txt
    ├── package.xml
    ├── roid1_urdf.urdf
    ├── urdf_rviz.rviz
    ├── launch
    │   ├── display_meridian_demo.launch
    │   └── display.launch
    └── roid1_description
        └── meshes    
            ├── c_chest_a.stl
            ├── c_chest_b.stl
            ├── c_head_a.stl
            ├── c_head_b.stl
            ├── c_waist.stl
            ├── dec_l_hipjoint_upperpoint.stl
            ├── dec_r_hipjoint_upperpoint.stl
            ├── dec_shoulderpoint.stl
            ├── l_ankle.stl
            ├── l_arm_lower.stl
            ├── l_arm_upper.stl
            ├── l_elbow.stl
            ├── l_foot_large.stl
            ├── l_hipjointlower.stl
            ├── l_hipjointupper.stl
            ├── l_leg_lower_a.stl
            ├── l_leg_lower_b.stl
            ├── l_leg_upper_a.stl
            ├── l_leg_upper_b.stl
            ├── l_shoulder.stl
            ├── r_ankle.stl
            ├── r_arm_lower.stl
            ├── r_arm_upper.stl
            ├── r_elbow.stl
            ├── r_foot_large.stl
            ├── r_hipjointlower.stl
            ├── r_hipjointupper.stl
            ├── r_leg_lower_a.stl
            ├── r_leg_lower_b.stl
            ├── r_leg_upper_a.stl
            ├── r_leg_upper_b.stl
            └── r_shoulder.stl
</pre>
