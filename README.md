物理パラメータを入れるテスト中です。物理パラメータ入りは下記にブランチしています。  
https://github.com/Ninagawa123/roid1/tree/inatia

# [Roid1](https://github.com/Ninagawa123/roid1)
  
This is a URDF file of a small humanoid robot Roid1 and it's Rviz operation demo.  
You can operate the joints of the robot with sliders.  
And you can also import this URDF file into Unity via URDF-importer.  
Roid1は小型ヒューマノイドロボットのURDFファイルです。  
Rvizでモデルを表示し、スライダーで関節を曲げることができます。  
また、URDF-importerを使いUnity上にモデルをインポートすることもできます。  

<img width="600" alt="roid1" src="https://user-images.githubusercontent.com/8329123/189541198-b70175dd-b50d-4334-860d-81675eec0de5.png">
  
  
# Usage (View in Rviz)
  
This demo has been confirmed to work on ubuntu/ROS-melodic,noetic with Rviz.  
Rviz用のデモはROS-melodic,noeticのRvizで動作確認しています。  
コマンドプロンプトより下記のコマンドで導入からRvizへの表示までを試せます。
  
$ cd ~/catkin_ws/src/  
  
$ git clone https://github.com/Ninagawa123/roid1.git  
  
$ cd ~/catkin_ws/  
  
$ catkin build  
  
$ source ~/catkin_ws/devel/setup.bash  
  
$ roslaunch roid1 display.launch  
  
# Usage (View in Unity)  
  
Drop URDF folder into Unity Assets, and open "roid1_urdf_unity.urdf" in URDF folder with URDF-Importer.  
UnityのプロジェクトウィンドウのAssetsの中にURDFフォルダをドロップしてください。その後、roid1_urdf_unity.urdfのファイルをURDF-Importerで読み込んでください。  
URDF-Importerの使い方は、https://www.youtube.com/watch?v=-OvDCy6cbfU  
  
  
# Directory Tree

<pre>
~/catkin_ws/src/
└── roid1 #ros_package
    ├── README.md
    ├── CMakeLists.txt
    ├── package.xml
    ├── urdf_rviz.rviz
    ├── launch
    │   ├── display.launch
    │   └── display_meridian_demo.launch
    └── roid1_description
        ├── roid1_urdf.urdf
        ├── roid1_urdf_unity.urdf
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
