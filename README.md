1 概述 

    gorilla robot是一套通用室内机器人解决方案，如扫地机器人、家庭服务机器人与商用清洁机器人等。gorlla robot支持x86和arm双平台，支持ros1、ros2和fast-dds三种通信方式，一键启动，无需配置过多环境，可以使用gazebo模拟器进行功能快速开发和调试。

2 功能

    |         节点         |              描述                                            |
    |----------------------|------------------------------------------------------------- |
    | noumenon             | UI界面，主要有建图，导航，重定位等功能                          |    
    | scheduler            | 调度中心，统筹一切的指令                                       |
    | gorilla_slam         | 建图，定位，寻找主方向，重定位，地图美化，地图分区等功能          |    
    | gorilla_navigation   | 导航模块，有通用地图，全局规划，局部规划，沿边，覆盖，巡检，指点   |
    | gorilla_bridge       | 与底板进行数据交换，指令交换                                    |
    | baseplate            | 产生数据，执行指令                                             |
    | tf_broadcaster       | 传感器外参数据的发布                                           |
    | gorilla_sensros      | lidar，camera等传感器数据的预处理与发布                         | 

3 系统框架  
       ![gorilla_robot_system_framework](https://github.com/GorillaKalman/gorilla_robot/assets/168891181/bcbe819c-fa3d-48fa-8ceb-1c77593ddbcb)

4 软件框架
      ![gorilla_robot_software_framework](https://github.com/GorillaKalman/gorilla_robot/assets/168891181/6c1dd13d-83b6-4c40-ba02-1686386c7d12)
