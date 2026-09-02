# Track 02 — 工具地图（机器人与具身智能）

> Phase 1 Wave 2 · Track 02。locale=zh-CN。全部 `last_checked = 2026-09-02`。
> 本文件不是 awesome-list。每个工具都必须回答四件事：**谁维护、最近一次发布是什么时候、许可证是什么、什么情况下不该用它**。

## Source Manifest

| source_id | url | bucket | last_checked | author/host | note |
|-----------|-----|--------|--------------|-------------|------|
| T02-S001 | https://raw.githubusercontent.com/ros2/ros2_documentation/rolling/source/Releases.rst | surrogate_primary | 2026-09-02 | ROS 2 项目 | vendor docs — ROS 2 发行版与 EOL 原始表 — Lyrical Luth 2026-05-22 |
| T02-S002 | https://github.com/ros2/ros2 | verified_primary | 2026-09-02 | ROS 2 项目 | ROS 2 元仓库 — star 5,987 (2026-09-02) |
| T02-S003 | https://docs.ros.org/en/jazzy/Installation/DDS-Implementations.html | surrogate_primary | 2026-09-02 | Open Robotics | vendor docs — 可选 DDS 实现清单与默认值 |
| T02-S004 | https://github.com/ros-controls/ros2_control | verified_primary | 2026-09-02 | ros-controls | ros2_control 主仓库 Apache-2.0 star 990 |
| T02-S005 | https://control.ros.org/rolling/doc/ros2_control/doc/release_notes.html | verified_primary | 2026-09-02 | ros-controls | Kilted→Lyrical 迁移与 breaking change 清单 |
| T02-S006 | https://github.com/eProsima/Fast-DDS | verified_primary | 2026-09-02 | eProsima | Fast DDS — ROS 2 历史默认 RMW |
| T02-S007 | https://github.com/eclipse-cyclonedds/cyclonedds | verified_primary | 2026-09-02 | Eclipse Foundation | Cyclone DDS — 最常见的替代 RMW 实现 |
| T02-S008 | https://github.com/micro-ROS/micro_ros_setup | verified_primary | 2026-09-02 | micro-ROS | micro-ROS 构建工具 6.1.0 (2026-08-11) |
| T02-S009 | https://micro.ros.org/ | verified_primary | 2026-09-02 | micro-ROS 项目 | MCU 侧 ROS 2 — 支持的 RTOS 与板卡 |
| T02-S010 | https://github.com/OpenEtherCATsociety/SOEM | verified_primary | 2026-09-02 | OpenEtherCAT Society | SOEM v2.0.0 (2025-07-11) 用户态 EtherCAT 主站 |
| T02-S011 | https://gitlab.com/etherlab.org/ethercat | verified_primary | 2026-09-02 | IgH / EtherLab | IgH EtherCAT Master — 内核态主站 GPLv2 |
| T02-S012 | https://github.com/ros-industrial/ros_canopen | verified_primary | 2026-09-02 | ROS-Industrial | ros_canopen LGPL-3.0 — ROS 1 时代实现 |
| T02-S013 | https://github.com/ros-industrial/ros2_canopen | verified_primary | 2026-09-02 | ROS-Industrial | ros2_canopen — CiA 402 驱动栈 |
| T02-S014 | https://www.xenomai.org/ | surrogate_primary | 2026-09-02 | Xenomai 项目 | own site — 双内核实时方案现状 |
| T02-S015 | https://github.com/moveit/moveit2 | verified_primary | 2026-09-02 | MoveIt / PickNik | MoveIt 2 BSD-3 star 1,986; 2.15.1 (2026-08-29) |
| T02-S016 | https://moveit.ai/ | surrogate_primary | 2026-09-02 | PickNik Robotics | vendor docs — MoveIt 商业支持方 |
| T02-S017 | https://github.com/ompl/ompl | verified_primary | 2026-09-02 | Rice / Kavraki Lab | OMPL 2.0.2 (2026-08-14) 采样规划算法库 |
| T02-S018 | https://ompl.kavrakilab.org/ | surrogate_primary | 2026-09-02 | Kavraki Lab | originator — OMPL 官方文档与许可证说明 |
| T02-S019 | https://github.com/stack-of-tasks/pinocchio | verified_primary | 2026-09-02 | INRIA / LAAS | Pinocchio 4.1.0 (2026-07-07) BSD-2 刚体动力学 |
| T02-S020 | https://github.com/loco-3d/crocoddyl | verified_primary | 2026-09-02 | LAAS / Edinburgh | Crocoddyl 3.2.1 (2026-05-10) DDP 最优控制 |
| T02-S021 | https://github.com/leggedrobotics/ocs2 | verified_primary | 2026-09-02 | ETH RSL | OCS2 — 足式 MPC 工具箱 BSD-3 |
| T02-S022 | https://github.com/hungpham2511/toppra | verified_primary | 2026-09-02 | Hung Pham | TOPP-RA 0.6.10 (2026-08-28) 时间最优参数化 |
| T02-S023 | https://github.com/osqp/osqp | verified_primary | 2026-09-02 | OSQP 团队 | OSQP v1.0.0 (2025-03-21) Apache-2.0 QP 求解 |
| T02-S024 | https://github.com/Simple-Robotics/proxsuite | verified_primary | 2026-09-02 | INRIA Willow | ProxQP v0.7.3 (2026-05-11) BSD-2 |
| T02-S025 | https://github.com/coin-or/qpOASES | verified_primary | 2026-09-02 | COIN-OR | qpOASES LGPL-2.1 — 在线主动集 QP |
| T02-S026 | https://github.com/RobotLocomotion/drake | verified_primary | 2026-09-02 | TRI / MIT | Drake v1.56.0 (2026-08-14) BSD-3 |
| T02-S027 | https://drake.mit.edu/ | verified_primary | 2026-09-02 | Russ Tedrake 团队 | Drake 官方文档 — 优化与接触建模 |
| T02-S028 | https://github.com/google-deepmind/mujoco | verified_primary | 2026-09-02 | Google DeepMind | MuJoCo 3.12.0 (2026-08-20) Apache-2.0 star 14.9k |
| T02-S029 | https://mujoco.readthedocs.io/en/stable/computation/index.html | surrogate_primary | 2026-09-02 | Google DeepMind | vendor docs — 软约束接触求解器原理 |
| T02-S030 | https://github.com/google-deepmind/mujoco_warp | verified_primary | 2026-09-02 | Google DeepMind | MJWarp v3.12.0 (2026-08-20) GPU 后端 star 1.4k |
| T02-S031 | https://mujoco.readthedocs.io/en/stable/mjx.html | surrogate_primary | 2026-09-02 | Google DeepMind | vendor docs — MJX 与 MuJoCo 的功能差异清单 |
| T02-S032 | https://developer.nvidia.com/isaac/sim | surrogate_primary | 2026-09-02 | NVIDIA | vendor docs — Isaac Sim 5.x Apache-2.0 与硬件要求 |
| T02-S033 | https://github.com/isaac-sim/IsaacLab | verified_primary | 2026-09-02 | NVIDIA | Isaac Lab BSD-3 star 8,026; v3.0.0-beta2.patch1 (2026-07-02) |
| T02-S034 | https://isaac-sim.github.io/IsaacLab/main/source/setup/installation/index.html | surrogate_primary | 2026-09-02 | NVIDIA | vendor docs — Isaac Lab 安装与 Isaac Sim 版本绑定 |
| T02-S035 | https://github.com/isaac-sim/IsaacGymEnvs | verified_primary | 2026-09-02 | NVIDIA | Isaac Gym Preview 环境 — 已停更, 迁移至 Isaac Lab |
| T02-S036 | https://developer.nvidia.com/isaac-gym | surrogate_primary | 2026-09-02 | NVIDIA | vendor docs — Isaac Gym Preview 弃用公告 |
| T02-S037 | https://gazebosim.org/docs/latest/releases/ | surrogate_primary | 2026-09-02 | Open Robotics / OSRA | vendor docs — Gazebo 版本表 Jetty LTS 至 2031-05 |
| T02-S038 | https://github.com/gazebosim/gz-sim | verified_primary | 2026-09-02 | OSRA | gz-sim Apache-2.0 star 1,479 — 新 Gazebo 主仓 |
| T02-S039 | https://classic.gazebosim.org/ | surrogate_primary | 2026-09-02 | OSRA | own site — Gazebo Classic 停止支持公告 (2025-01) |
| T02-S040 | https://genesis-world.readthedocs.io/ | verified_primary | 2026-09-02 | Genesis 团队 | Genesis 官方文档 — 求解器与速度口径 |
| T02-S041 | https://github.com/Genesis-Embodied-AI/genesis-world | verified_primary | 2026-09-02 | Genesis 团队 | Genesis v1.3.3 (2026-08-13) Apache-2.0 star 29.9k |
| T02-S042 | https://github.com/mani-skill/ManiSkill | verified_primary | 2026-09-02 | UCSD Hao Su 组 | ManiSkill v3.0.1 (2026-04-21) Apache-2.0 star 3.3k |
| T02-S043 | https://github.com/haosulab/SAPIEN | verified_primary | 2026-09-02 | UCSD Hao Su 组 | SAPIEN 仿真内核 star 829 |
| T02-S044 | https://github.com/ARISE-Initiative/robosuite | verified_primary | 2026-09-02 | ARISE Initiative | robosuite v1.5.2 (2025-12-24) MuJoCo 系操作环境 |
| T02-S045 | https://github.com/bulletphysics/bullet3 | verified_primary | 2026-09-02 | Erwin Coumans 等 | Bullet3 / PyBullet — 最后 push 2025-10-22, 维护近停滞 |
| T02-S046 | https://pybullet.org/wordpress/ | surrogate_primary | 2026-09-02 | Bullet 项目 | own site — PyBullet 定位与文档入口 |
| T02-S047 | https://github.com/cyberbotics/webots | verified_primary | 2026-09-02 | Cyberbotics | Webots Apache-2.0 star 4.6k — 教育与竞赛主力 |
| T02-S048 | https://www.coppeliarobotics.com/ | surrogate_primary | 2026-09-02 | Coppelia Robotics | vendor docs — CoppeliaSim 商业授权与多引擎 |
| T02-S049 | https://github.com/StanfordVL/OmniGibson | verified_primary | 2026-09-02 | Stanford Vision & Learning | OmniGibson — BEHAVIOR-1K 的仿真后端 |
| T02-S050 | https://github.com/NVIDIA/warp | verified_primary | 2026-09-02 | NVIDIA | Warp — MJWarp 与 Newton 的底层可微 GPU 内核 |
| T02-S051 | https://github.com/newton-physics/newton | verified_primary | 2026-09-02 | NVIDIA / DeepMind / Disney | Newton 物理引擎 — Isaac Lab 3.0 新后端 |
| T02-S052 | https://github.com/opencv/opencv | verified_primary | 2026-09-02 | OpenCV 基金会 | OpenCV 5.0.0 (2026-06-26) 与 4.14.0 (2026-07-19) 双线 |
| T02-S053 | https://github.com/opencv/opencv/releases/tag/5.0.0 | verified_primary | 2026-09-02 | OpenCV 基金会 | OpenCV 5.0.0 release note — 破坏性变化清单 |
| T02-S054 | https://github.com/isl-org/Open3D | verified_primary | 2026-09-02 | Intel ISL | Open3D v0.19 (2025-01-10) — 正式版发布节奏放缓 |
| T02-S055 | https://github.com/PointCloudLibrary/pcl | verified_primary | 2026-09-02 | PCL 社区 | PCL 1.15.1 (2025-08) — 维护型更新为主 |
| T02-S056 | https://github.com/UZ-SLAMLab/ORB_SLAM3 | verified_primary | 2026-09-02 | Univ. Zaragoza | ORB-SLAM3 GPL-3.0 — 最后 push 2024-07-24 |
| T02-S057 | https://github.com/HKUST-Aerial-Robotics/VINS-Fusion | verified_primary | 2026-09-02 | HKUST 沈劭劼组 | VINS-Fusion GPL-3.0 — 最后 push 2024-05-23 |
| T02-S058 | https://github.com/rpng/open_vins | verified_primary | 2026-09-02 | UD RPNG | OpenVINS GPL-3.0 — 2025-11-30 仍有更新 |
| T02-S059 | https://github.com/borglab/gtsam | verified_primary | 2026-09-02 | GT Borg Lab | GTSAM 4.3a2 (2026-08-04) BSD 因子图后端 |
| T02-S060 | https://github.com/ethz-asl/kalibr | verified_primary | 2026-09-02 | ETH ASL | Kalibr 相机-IMU 标定 — 最后 push 2024-03-30 |
| T02-S061 | https://github.com/IFL-CAMP/easy_handeye | verified_primary | 2026-09-02 | TUM CAMP | easy_handeye — ROS 手眼标定包装器 |
| T02-S062 | https://github.com/marcoesposito1988/easy_handeye2 | verified_primary | 2026-09-02 | Marco Esposito | easy_handeye2 — ROS 2 版本 |
| T02-S063 | https://github.com/NVlabs/FoundationPose | verified_primary | 2026-09-02 | NVIDIA Labs | FoundationPose — NVIDIA 源代码许可, 非商用条款 |
| T02-S064 | https://github.com/megapose6d/megapose6d | verified_primary | 2026-09-02 | INRIA Willow | MegaPose — 新物体 6D 位姿估计 |
| T02-S065 | https://ai.meta.com/sam2/ | surrogate_primary | 2026-09-02 | Meta AI | own site — SAM 2 项目页与许可证说明 |
| T02-S066 | https://github.com/introlab/rtabmap | verified_primary | 2026-09-02 | IntRoLab | RTAB-Map BSD — 移动机器人 RGB-D SLAM |
| T02-S067 | https://github.com/cartographer-project/cartographer | verified_primary | 2026-09-02 | Cartographer 项目 | Cartographer Apache-2.0 — 最后 push 2024-01-05 |
| T02-S068 | https://github.com/realsenseai/librealsense | verified_primary | 2026-09-02 | RealSense AI (原 Intel) | librealsense — 组织已从 IntelRealSense 迁出 |
| T02-S069 | https://www.realsenseai.com/ | surrogate_primary | 2026-09-02 | RealSense AI | vendor docs — 从 Intel 独立后的官网与产品线 |
| T02-S070 | https://www.stereolabs.com/products/zed-2 | surrogate_primary | 2026-09-02 | Stereolabs | vendor docs — ZED 2i 双目相机规格 |
| T02-S071 | https://ouster.com/products/hardware/os1-lidar-sensor | surrogate_primary | 2026-09-02 | Ouster | vendor docs — OS1 数字激光雷达规格 |
| T02-S072 | https://www.livoxtech.com/mid-360 | surrogate_primary | 2026-09-02 | Livox 览沃 | vendor docs — Mid-360 非重复扫描雷达规格 |
| T02-S073 | https://github.com/huggingface/lerobot | verified_primary | 2026-09-02 | Hugging Face | LeRobot v0.6.1 (2026-08-03) Apache-2.0 star 27.2k |
| T02-S074 | https://huggingface.co/docs/lerobot/index | verified_primary | 2026-09-02 | Hugging Face | LeRobot 官方文档 — 数据集格式与硬件支持 |
| T02-S075 | https://github.com/Physical-Intelligence/openpi | verified_primary | 2026-09-02 | Physical Intelligence | openpi Apache-2.0 star 13.6k — π0/π0.5 权重 |
| T02-S076 | https://github.com/octo-models/octo | verified_primary | 2026-09-02 | Berkeley RAIL 等 | Octo MIT — 最后 push 2024-07-31, 已停更 |
| T02-S077 | https://github.com/openvla/openvla | verified_primary | 2026-09-02 | Stanford / Berkeley 等 | OpenVLA MIT — 最后 push 2025-03-23 |
| T02-S078 | https://github.com/ARISE-Initiative/robomimic | verified_primary | 2026-09-02 | ARISE Initiative | robomimic MIT — 模仿学习标准实现与消融 |
| T02-S079 | https://github.com/google-research/rlds | verified_primary | 2026-09-02 | Google Research | RLDS — 强化学习数据集格式与工具 |
| T02-S080 | https://github.com/leggedrobotics/rsl_rl | verified_primary | 2026-09-02 | ETH RSL | RSL-RL — 足式 GPU PPO 参考实现 star 2.9k |
| T02-S081 | https://github.com/Toni-SM/skrl | verified_primary | 2026-09-02 | Toni Serrano | skrl MIT — 多仿真器统一 RL 库 |
| T02-S082 | https://github.com/DLR-RM/stable-baselines3 | verified_primary | 2026-09-02 | DLR-RM | SB3 MIT star 13.8k — 教学与基线用 |
| T02-S083 | https://docs.ray.io/en/latest/rllib/index.html | verified_primary | 2026-09-02 | Anyscale / Ray 项目 | RLlib 文档 — 分布式 RL 调度 |
| T02-S084 | https://github.com/real-stanford/diffusion_policy | verified_primary | 2026-09-02 | Columbia / Stanford / TRI | Diffusion Policy 官方实现 MIT |
| T02-S085 | https://github.com/NVIDIA/Isaac-GR00T | verified_primary | 2026-09-02 | NVIDIA | Isaac GR00T N1.6 (2026-04) Apache-2.0 star 8.0k |
| T02-S086 | https://github.com/TheRobotStudio/SO-ARM100 | verified_primary | 2026-09-02 | The Robot Studio | SO-100/SO-101 开源低成本臂 Apache-2.0 |
| T02-S087 | https://github.com/tonyzhaozh/aloha | verified_primary | 2026-09-02 | Tony Z. Zhao (Stanford) | ALOHA 双臂遥操作硬件与 ACT |
| T02-S088 | https://mobile-aloha.github.io/ | surrogate_primary | 2026-09-02 | Stanford | originator — Mobile ALOHA 硬件清单与成本 |
| T02-S089 | https://github.com/wuphilipp/gello_software | verified_primary | 2026-09-02 | Philipp Wu (Berkeley) | GELLO — 低成本关节映射遥操作主手 |
| T02-S090 | https://github.com/rerun-io/rerun | verified_primary | 2026-09-02 | Rerun | Rerun 0.37.0 (2026-09-01) Apache-2.0 star 11.4k |
| T02-S091 | https://foxglove.dev/pricing | surrogate_primary | 2026-09-02 | Foxglove | vendor docs — 定价与免费额度, 已转商业闭源 |
| T02-S092 | https://github.com/ros2/rosbag2 | verified_primary | 2026-09-02 | ROS 2 项目 | rosbag2 — MCAP 默认存储插件 |
| T02-S093 | https://mcap.dev/ | surrogate_primary | 2026-09-02 | Foxglove | vendor docs — MCAP 容器格式规范 |
| T02-S094 | https://github.com/PlotJuggler/PlotJuggler | verified_primary | 2026-09-02 | Davide Faconti | PlotJuggler 4 beta3 (2026-08-15) MPL-2.0 star 6.1k |
| T02-S095 | https://www.unitree.com/g1 | surrogate_primary | 2026-09-02 | 宇树科技 Unitree | vendor docs — G1 23-43 DOF, 35kg, US$13.5K |
| T02-S096 | https://www.unitree.com/go2 | surrogate_primary | 2026-09-02 | 宇树科技 Unitree | vendor docs — Go2 四足规格与版本分层 |
| T02-S097 | https://github.com/unitreerobotics/unitree_sdk2 | verified_primary | 2026-09-02 | 宇树科技 Unitree | unitree_sdk2 BSD-3 — DDS 底层控制接口 |
| T02-S098 | https://github.com/unitreerobotics/unitree_ros2 | verified_primary | 2026-09-02 | 宇树科技 Unitree | 官方 ROS 2 桥接 — CycloneDDS 配置与网口绑定 |
| T02-S099 | https://github.com/unitreerobotics/unitree_rl_gym | verified_primary | 2026-09-02 | 宇树科技 Unitree | 官方 RL 训练与 sim2real 部署示例 |
| T02-S100 | https://www.agibot.com/ | surrogate_primary | 2026-09-02 | 智元机器人 AgiBot | vendor docs — 远征/灵犀产品线 |
| T02-S101 | https://github.com/AgibotTech/agibot_x1_train | verified_primary | 2026-09-02 | 智元机器人 AgiBot | AgiBot X1 开源本体的 RL 训练代码 |
| T02-S102 | https://www.openloong.org.cn/ | verified_primary | 2026-09-02 | 上海国地共建人形创新中心 | OpenLoong 开源社区 — 青龙公版机 |
| T02-S103 | https://github.com/loongOpen | surrogate_primary | 2026-09-02 | OpenLoong 社区 | vendor docs — OpenLoong 组织页 — 控制与仿真仓库 |
| T02-S104 | https://www.jaka.com/ | surrogate_primary | 2026-09-02 | 节卡 JAKA | vendor docs — 协作臂产品线与控制器 |
| T02-S105 | https://www.aubo-robotics.cn/products | surrogate_primary | 2026-09-02 | 遨博 AUBO | vendor docs — iS/i 系列 3-35kg, ±0.02~0.05mm 重复定位 |
| T02-S106 | https://www.inovance.com/ | surrogate_primary | 2026-09-02 | 汇川技术 Inovance | vendor docs — 国产伺服驱动/控制器 供应商 |
| T02-S107 | https://www.dobot-robots.com/ | surrogate_primary | 2026-09-02 | 越疆 Dobot | vendor docs — CR/Nova 协作臂与教育线 |
| T02-S108 | https://www.rokae.com/ | surrogate_primary | 2026-09-02 | 珞石 ROKAE | vendor docs — xMate 柔性协作臂 |
| T02-S109 | https://www.universal-robots.com/products/ | surrogate_primary | 2026-09-02 | Universal Robots | vendor docs — UR e 系列与 UR AI Accelerator |
| T02-S110 | https://franka.de/franka-research-3 | surrogate_primary | 2026-09-02 | Franka Robotics | vendor docs — FR3 7 轴力矩传感, 3kg/855mm/±0.1mm |
| T02-S111 | https://robotiq.com/products/adaptive-grippers | surrogate_primary | 2026-09-02 | Robotiq | vendor docs — 2F-85/2F-140 自适应夹爪 |
| T02-S112 | https://schunk.com/ | surrogate_primary | 2026-09-02 | SCHUNK | vendor docs — 工业夹爪与快换系统 |
| T02-S113 | https://www.ati-ia.com/products/ft/sensors.aspx | surrogate_primary | 2026-09-02 | ATI Industrial Automation | vendor docs — 六维力/力矩传感器选型表 |
| T02-S114 | https://www.shadowrobot.com/dexterous-hand-series/ | surrogate_primary | 2026-09-02 | Shadow Robot | vendor docs — Shadow 灵巧手自由度与价格区间 |
| T02-S115 | https://www.inspire-robots.com/ | surrogate_primary | 2026-09-02 | 因时机器人 Inspire | vendor docs — 灵巧手与微型伺服 |
| T02-S116 | https://www.anybotics.com/robotics/anymal/ | surrogate_primary | 2026-09-02 | ANYbotics | vendor docs — ANYmal 工业巡检四足 |
| T02-S117 | https://bostondynamics.com/products/spot/ | surrogate_primary | 2026-09-02 | Boston Dynamics | vendor docs — Spot 与 Spot SDK 开放度 |
| T02-S118 | https://dev.bostondynamics.com/ | surrogate_primary | 2026-09-02 | Boston Dynamics | vendor docs — Spot SDK 文档与 API 边界 |
| T02-S119 | https://www.harmonicdrive.net/ | surrogate_primary | 2026-09-02 | Harmonic Drive | vendor docs — 谐波减速器背隙与精度口径 |
| T02-S120 | https://precision.nabtesco.com/ | surrogate_primary | 2026-09-02 | Nabtesco | vendor docs — RV 减速器负载与刚度 |
| T02-S121 | https://www.leaderdrive.com/ | surrogate_primary | 2026-09-02 | 绿的谐波 Leaderdrive | vendor docs — 国产谐波减速器规格 |
| T02-S122 | https://www.siasun.com/ | surrogate_primary | 2026-09-02 | 新松 SIASUN | vendor docs — 国产工业与移动机器人整机 |
| T02-S123 | https://www.efort.com.cn/ | surrogate_primary | 2026-09-02 | 埃夫特 EFORT | vendor docs — 国产工业机器人本体与集成 |
| T02-S124 | https://www.zeroerr.cn/ | surrogate_primary | 2026-09-02 | 零差云控 ZeroErr | vendor docs — 一体化关节模组与谐波方案 |
| T02-S125 | https://www.limxdynamics.com/ | surrogate_primary | 2026-09-02 | 逐际动力 LimX | vendor docs — 双足/人形本体与开源栈 |
| T02-S126 | https://www.robotera.com/ | surrogate_primary | 2026-09-02 | 星动纪元 RobotEra | vendor docs — 人形本体与灵巧手 |
| T02-S127 | https://www.galbot.com/ | surrogate_primary | 2026-09-02 | 银河通用 Galbot | vendor docs — 轮式双臂与合成数据路线 |
| T02-S128 | https://www.fftai.com/ | surrogate_primary | 2026-09-02 | 傅利叶 Fourier | vendor docs — GRx 人形与康复机器人 |
| T02-S129 | https://www.ubtrobot.com/ | surrogate_primary | 2026-09-02 | 优必选 UBTECH | vendor docs — Walker 系列与工业场景落地 |
| T02-S130 | https://github.com/InternRobotics/InternUtopia | verified_primary | 2026-09-02 | 上海 AI Lab InternRobotics | GRUtopia 更名为 InternUtopia — 场景级仿真 |
| T02-S131 | https://github.com/ros-navigation/navigation2 | verified_primary | 2026-09-02 | Nav2 项目 | Nav2 — ROS 2 移动机器人导航栈 |
| T02-S132 | https://docs.nav2.org/ | verified_primary | 2026-09-02 | Nav2 项目 | Nav2 官方文档 — 行为树与规划器插件 |
| T02-S133 | https://github.com/ros2/rmw_zenoh | verified_primary | 2026-09-02 | ROS 2 项目 / ZettaScale | rmw_zenoh — DDS 之外的中间件选项 |
| T02-S134 | https://developer.nvidia.com/isaac/ros | surrogate_primary | 2026-09-02 | NVIDIA | vendor docs — Isaac ROS GPU 加速感知包 |
| T02-S135 | https://github.com/moveit/moveit_task_constructor | verified_primary | 2026-09-02 | MoveIt 项目 | MTC — 多阶段操作任务规划 |
| T02-S136 | https://github.com/newton-physics/newton | verified_primary | 2026-09-02 | NVIDIA/DeepMind/Disney | Newton — 2025 起的新可微物理引擎 |
| T02-S137 | https://github.com/UniversalRobots/Universal_Robots_ROS2_Driver | verified_primary | 2026-09-02 | Universal Robots | 官方 UR ROS 2 驱动 — 产线常见接入路径 |
| T02-S138 | https://github.com/frankarobotics/franka_ros2 | verified_primary | 2026-09-02 | Franka Robotics | 官方 franka_ros2 — FR3 的 ROS 2 接入 |
| T02-S139 | https://github.com/facebookresearch/sam2 | verified_primary | 2026-09-02 | Meta AI | SAM 2 Apache-2.0 — 分割与掩码传播 |
| T02-S140 | https://github.com/AgibotTech/agibot_x1_hardware | verified_primary | 2026-09-02 | 智元机器人 AgiBot | AgiBot X1 开源硬件图纸与 BOM |
| T02-S141 | https://docs.ros.org/en/rolling/Installation/RMW-Implementations/Non-DDS-Implementations/Working-with-Zenoh.html | surrogate_primary | 2026-09-02 | Open Robotics | vendor docs — Zenoh 已列为 ROS 2 tier-1 中间件 |
| T02-S142 | https://github.com/eclipse-zenoh/zenoh-plugin-ros2dds | verified_primary | 2026-09-02 | Eclipse Zenoh | DDS↔Zenoh 桥 — 跨网段/弱网部署常用 |


## 阅读说明（三条口径约定，先读这个再读工具卡）

**第一条：精度只有两个词，别混。**
厂商 datasheet 上写的「±0.02 mm」几乎总是**重复定位精度（pose repeatability）**——同一条指令反复走，末端落点的散布。它**不等于**你让机器人去空间里某个坐标、它真能到那个坐标的能力，那叫**绝对定位精度（pose accuracy）**。同一台工业臂，重复定位 ±0.03 mm、绝对定位常在 **0.5–2 mm** 量级，差一到两个数量级 (evidence: [T06-S006, T06-S089])。**只要你的方案里出现「相机告诉机器人去哪」，你吃的就是绝对精度，不是重复精度**；想把绝对精度拉回来，唯一的路是机器人标定 + 手眼标定，而不是换一个 datasheet 数字更好看的臂。本文件里所有精度数字都标了是哪一种，没标的一律当未知。

**第二条：仿真数字必须带三件套——引擎、步长、并行数。**
「20 万 FPS」这种话单独出现没有信息量。同一个场景，换求解器（MuJoCo 的软约束 vs PhysX 的 TGS）、换时间步长（1 ms vs 5 ms）、换并行环境数（1 vs 4096），吞吐能差两个数量级，而且**不同引擎之间的成功率完全不可比** (evidence: [T05-S055])。本文件里凡是给了吞吐数字的，都注明了谁在什么硬件上测的；查不到测试条件的，写「未公开测试条件」。

**第三条：许可证决定你能不能拿它做产品，比 star 数重要得多。**
这一行的开源栈里混着四类完全不同的许可证，后果差别极大：
- **Apache-2.0 / BSD / MIT**（ROS 2、MuJoCo、Isaac Lab、LeRobot、OpenCV）——商用无障碍，是产品栈的主体；
- **GPL-3.0**（ORB-SLAM3、VINS-Fusion、OpenVINS、ArduPilot）——**链接进你的闭源产品就触发传染**。学术复现随便用，产品里用要么换实现要么谈商业授权，这是国内交付里最常见的隐性法务雷；
- **LGPL / MPL-2.0**（ros_canopen、PlotJuggler）——动态链接可接受，改了库本身要开源；
- **CC BY-NC / 非商用数据集**（AgiBot World 是 CC BY-NC-SA 4.0）——**拿它训出来的模型进商业产品是违约的**，而且 SA 条款要求衍生物同样开放 (evidence: [T05-S034])。

> 覆盖度声明：本轨共考察 **74 个候选工具/平台**，保留 **53 个**写成条目（必备 11 / 场景特化 24 / 新兴 9 / 硬件 9 格）。淘汰的 21 个见文末「不进任何层」。


## 总览（按 tier 分组）

> Decay 口径：**low** = 24 个月以上被显著改变的概率 < 20%；**medium** = 12–24 个月内 20–40%；**high** = 12 个月内 > 40%（新兴层默认 high）。

### 必备层（11 个）——不用它，你要么自己造一遍，要么招不到能接手的人

| 工具 | 一句话 | 许可证 | 最近发布 | Decay | Evidence |
|------|--------|--------|----------|-------|----------|
| ROS 2 | 机器人软件的事实通用底座：进程间通信 + 包管理 + 工具链 | Apache-2.0 | Lyrical Luth 2026-05-22 (LTS→2031-05) | low | T02-S001, T02-S002 |
| ros2_control | 把「控制器」和「硬件驱动」解耦的标准框架，实时环里的那一层 | Apache-2.0 | 6.9.0 / 2026-08-10 | low | T02-S004, T02-S005 |
| MuJoCo（含 MJX / MJWarp） | 接触仿真的学术事实标准，软约束求解器 + 极快单机迭代 | Apache-2.0 | 3.12.0 / 2026-08-20 | low | T02-S028, T02-S030 |
| Isaac Sim + Isaac Lab | GPU 大规模并行 RL 训练的工业级路径，绑 NVIDIA 生态 | Apache-2.0（+ NVIDIA 补充条款） | Isaac Lab 3.0-beta2.patch1 / 2026-07-02 | medium | T02-S032, T02-S033 |
| Gazebo（Jetty） | ROS 生态默认的系统级仿真：传感器插件、多机、世界建模 | Apache-2.0 | Jetty 2025-09（LTS→2031-05） | low | T02-S037, T02-S038 |
| MoveIt 2 | 机械臂运动规划的默认集成层：碰撞检查 + 规划 + 执行 + 场景 | BSD-3 | 2.15.1 / 2026-08-29 | low | T02-S015 |
| Pinocchio | 刚体动力学与解析导数，几乎所有现代控制/优化库的底座 | BSD-2 | 4.1.0 / 2026-07-07 | low | T02-S019 |
| OpenCV | 图像处理与标定的地板，5.0 与 4.x 双线并行 | Apache-2.0 | 5.0.0 / 2026-06-26；4.14.0 / 2026-07-19 | low | T02-S052, T02-S053 |
| LeRobot | 模仿学习与 VLA 的默认数据格式 + 训练 + 真机部署一条龙 | Apache-2.0 | v0.6.1 / 2026-08-03 | medium | T02-S073, T02-S074 |
| Rerun | 多模态机器人数据的可视化与时间轴调试，取代自己写 RViz 插件 | Apache-2.0 | 0.37.0 / 2026-09-01 | medium | T02-S090 |
| rosbag2 + MCAP + PlotJuggler | 记录、回放、翻曲线——出了事故只有这三样能救你 | Apache-2.0 / MPL-2.0 | PlotJuggler 4 beta3 / 2026-08-15 | low | T02-S092, T02-S093, T02-S094 |

### 场景特化层（24 个）——选它 = 接受一个具体代价

| 工具 | 什么场景选它 | 代价 | Decay | Evidence |
|------|-------------|------|-------|----------|
| Drake | 需要可验证的接触建模 + 凸优化/轨迹优化，愿意读教材 | 学习曲线陡；生态自成一体，与 ROS 集成要自己搭 | low | T02-S026, T02-S027 |
| Genesis | 想要一个 Python-native、跨材料（刚体/软体/流体）的新仿真器 | 2024 年底才发布，接口仍在变；sim-to-real 证据链短 | high | T02-S040, T02-S041 |
| ManiSkill 3 + SAPIEN | GPU 并行的**操作**任务基准 + 视觉观测吞吐 | 绑 SAPIEN 渲染栈；与 Isaac 的分数不可比 | medium | T02-S042, T02-S043 |
| robosuite | 需要一套干净、可复现的 MuJoCo 操作环境做算法消融 | 单机为主，并行吞吐远不如 GPU 方案 | medium | T02-S044 |
| Webots | 教育、竞赛、多机器人系统课程；开箱即用模型多 | 工业交付几乎不用；物理保真度不适合接触密集任务 | medium | T02-S047 |
| CoppeliaSim | 快速搭一个含 PLC/传送带/多机的工位原型，脚本化强 | 商业授权（教育版免费，商用付费）；社区规模小 | medium | T02-S048 |
| PyBullet / Bullet3 | 只做教学与老论文复现 | **主仓最后 push 2025-10-22，实质维护停滞**；不要作为新项目基座 | high | T02-S045, T02-S046 |
| OMPL | 需要经典采样式规划算法（RRT*/PRM/BIT*）本体 | 只管几何路径，不管动力学与时间参数化 | low | T02-S017, T02-S018 |
| Crocoddyl | 足式/全身的 DDP-类最优控制，要解析导数与实时性 | 需要懂最优控制；调不好就发散 | medium | T02-S020 |
| OCS2 | 足式 MPC 的成套实现（ANYmal 系血统） | 编译重、文档薄、耦合 ROS 1 时代习惯 | medium | T02-S021 |
| TOPP-RA | 把几何路径变成满足速度/加速度/力矩约束的时间轨迹 | 只解决时间参数化这一小段，不是规划器 | low | T02-S022 |
| OSQP / ProxQP / qpOASES | 控制环里的二次规划（WBC、MPC、导纳控制） | 三者在**热启动**与**病态问题**上表现差别大，必须实测 | low | T02-S023, T02-S024, T02-S025 |
| Nav2 | 轮式/移动底盘的导航栈：行为树 + 代价地图 + 恢复行为 | 面向 2D/2.5D 移动；不解决操作与力控 | low | T02-S131, T02-S132 |
| GTSAM | 需要自己写因子图后端（多传感器融合、标定、SLAM） | 要理解因子图与流形优化，不是拿来即用的 SLAM | low | T02-S059 |
| ORB-SLAM3 / VINS-Fusion / OpenVINS | 视觉惯性定位的学术基线 | **三者都是 GPL-3.0**，闭源产品里用会传染 | medium | T02-S056, T02-S057, T02-S058 |
| Open3D / PCL | 点云处理、配准、可视化 | Open3D 正式版节奏放缓（v0.19 / 2025-01）；PCL 以维护更新为主 | medium | T02-S054, T02-S055 |
| Kalibr / easy_handeye(2) | 相机内参、相机-IMU 外参、手眼标定 | Kalibr 最后 push 2024-03-30；ROS 2 侧要用 easy_handeye2 | medium | T02-S060, T02-S061, T02-S062 |
| FoundationPose / MegaPose / SAM 2 | 无 CAD 或少样本的 6D 位姿与实例分割 | FoundationPose 是 NVIDIA 源代码许可（**非商用**），落地要换实现 | high | T02-S063, T02-S064, T02-S139 |
| robomimic + Diffusion Policy | 模仿学习的标准实现与消融基线 | 论文级封装，工程化（数据管线、监控、回滚）要自己补 | medium | T02-S078, T02-S084 |
| RSL-RL / skrl / SB3 / RLlib | 大规模 RL 训练与调度 | RSL-RL 极简但只服务足式；SB3 单环境教学向；RLlib 重 | medium | T02-S080, T02-S081, T02-S082, T02-S083 |
| micro-ROS + SOEM/IgH + CANopen | 从上位机一路打到 MCU 与伺服驱动的真实控制链路 | 每一层的实时性都要自己证明；没人替你担保抖动 | low | T02-S008, T02-S010, T02-S011, T02-S013 |
| Isaac ROS | Jetson/RTX 上要把感知延迟压下去，需要 GPU 零拷贝管线 | 深度绑 NVIDIA 硬件；与 JetPack/Isaac Sim 三方版本对齐是持续负担 | medium | T02-S134 |
| Foxglove | 团队要共享一份现场数据并批注，需要云端协作 | 核心工具已转商业闭源；数据不能出内网的项目直接出局 | medium | T02-S091, T02-S093 |
| RealSense / ZED / Ouster / Livox | 深度与激光的输入端选型 | 产品线变动是主要风险（RealSense 已从 Intel 独立） | medium | T02-S068, T02-S069, T02-S070, T02-S071, T02-S072 |

### 新兴层（9 个）——`stability: experimental`，半年后可能换名字或不存在

| 工具 | 出现时间 | 为什么值得盯 | Decay | Evidence |
|------|---------|-------------|-------|----------|
| MuJoCo Warp（MJWarp） | 仓库建于 2025-03-17 | 把 MuJoCo 搬到 GPU 的官方路线，版本号已与 MuJoCo 主线对齐（3.12.0 / 2026-08-20） | high | T02-S030 |
| Newton | 2025 起，NVIDIA + DeepMind + Disney Research 联合 | Isaac Lab 3.0 的新物理后端，可能重排「谁是并行仿真默认」 | high | T02-S051, T02-S136 |
| Isaac Lab 3.0（beta） | 3.0-beta 2026-03，beta2.patch1 2026-07-02 | 多物理后端 + 可插拔渲染 + 无 Kit 工作流，是一次架构级重写 | high | T02-S033, T02-S034 |
| Genesis | 首发 2024-12 | Python-native、多材料、宣称极高吞吐；争议也集中在吞吐口径 | high | T02-S040, T02-S041 |
| openpi（π0 / π0.5） | 仓库建于 2024-10-21 | 第一批把 VLA 权重 + 微调脚本以 Apache-2.0 公开的，star 13.6k | high | T02-S075 |
| Isaac GR00T N1.x | 仓库建于 2025-03-11，N1.6 于 2026-04 | NVIDIA 押注的开源人形基础模型 + 合成数据管线 | high | T02-S085 |
| rmw_zenoh | 已进入 ROS 2 tier-1 中间件 | DDS 之外的第一个官方选项，跨网段/弱网场景直接改善 | medium | T02-S133, T02-S141 |
| SO-101 + LeRobot 硬件生态 | SO-100 2024，SO-101 2025 | 把「采数据」的门槛从几万美元压到千元级，改变了谁能进这一行 | high | T02-S086, T02-S073 |
| InternUtopia（原 GRUtopia） | 2024 发布，2025 更名 | 中国侧场景级（城市/室内）具身仿真，与 InternRobotics 体系绑定 | high | T02-S130 |


## 一、必备层 — 不用它你就得自己造一遍

### 1. ROS 2

- **One-liner**：进程间通信 + 包管理 + 构建/调试工具链的通用底座。它的真实价值不在技术先进，而在**「换个人也能接手」**——招人、外包、集成第三方硬件，都默认你在这上面。
- **Tier**：必备
- **维护方**：Open Source Robotics Alliance（OSRA，Open Robotics 于 2024 年重组后的治理实体）(evidence: [T05-S028])
- **许可证**：Apache-2.0（核心包）
- **发行版与生命周期（这张表决定你的项目寿命）**：
  | 发行版 | 发布 | EOL | LTS |
  |---|---|---|---|
  | Lyrical Luth | 2026-05-22 | 2031-05 | 是 |
  | Kilted Kaiju | 2025-05-23 | **2026-12** | 否 |
  | Jazzy Jalisco | 2024-05-23 | 2029-05 | 是 |
  | Humble Hawksbill | 2022-05-23 | 2027-05 | 是 |
  (evidence: [T02-S001])
- **成熟度信号**：`ros2/ros2` 元仓库 star 5,987、最后 push 2026-09-01（2026-09-02 查）(evidence: [T02-S002])。注意 star 数在这里是**误导性指标**——ROS 2 的代码分散在数百个仓库里，元仓库的 star 不代表采用度。
- **真实使用门槛**：
  - **不是拿来就能用**：一台真机跑起来通常要自己写 hardware interface、配 QoS、调 DDS 发现、处理多网卡与时间同步。第一次从零到能动，一个熟手 2–5 天，新手两周起。
  - **QoS 配错是这一行第一大玄学 bug**：`reliable` 配到高频传感器上会积压，`best_effort` 配到指令上会丢包。ROS 2 官方把 QoS 单列成概念页是有原因的 (evidence: [T06-S067])
  - **中间件是可换的**：Fast DDS、Cyclone DDS 之外，**Zenoh 已进入 tier-1**，跨网段/弱网/多机场景可以直接换 `rmw_zenoh` 而不改业务代码；可选实现清单见官方文档 (evidence: [T02-S003, T02-S006, T02-S007, T02-S133, T02-S141])
- **什么情况下不该用它**：
  1. **硬实时控制环放在 ROS 2 里** — ROS 2 **不自带实时性**。它的设计允许你构建实时系统（执行器可配、可用 RT 内核），但默认发行版跑在通用 Linux 上，抖动到毫秒级很正常。1 kHz 力控环要放在 PREEMPT_RT 或 MCU 上，用 EtherCAT/CANopen 下行，ROS 2 只当上位机 (evidence: [T06-S072, T06-S070])
  2. **只做一个纯视觉算法 demo** — 上 ROS 2 是纯负担，直接 Python 脚本 + Rerun 更快
  3. **单片机独立产品** — 用 micro-ROS 或干脆不用 ROS
- **近 12 个月变化**：Lyrical Luth 于 2026-05-22 发布并成为新 LTS（支持到 2031-05）；Kilted Kaiju 将于 **2026-12 EOL**，**任何 2026 年新开的项目都不应该起在 Kilted 上** (evidence: [T02-S001])
- **Decay risk**：low（作为底座，24 个月内被取代概率 < 20%）／但**发行版本身每年换**，pin 版本这件事永远是 medium 风险

### 2. ros2_control

- **One-liner**：把「控制器算法」和「硬件驱动」拆开的标准框架——你写一次 hardware interface，就能复用社区所有控制器；或反过来。
- **Tier**：必备（只要你真的驱动一台机器人，而不是只跑仿真）
- **维护方**：ros-controls 组织（Bence Magyar / Denis Štogl 等长期维护）
- **许可证**：Apache-2.0
- **成熟度信号**：star 990、最后 push 2026-09-02；同日发布三条支持线 6.9.0 / 5.17.0 / 4.47.0（2026-08-10），对应不同 ROS 2 发行版 (evidence: [T02-S004])
- **真实使用门槛**：概念多（controller manager、resource manager、hardware component 的 lifecycle、command/state interface），文档密度大。**门槛主要在第一次**：写通一个 hardware interface 之后，后面加控制器很快。
- **什么情况下不该用它**：
  1. 你的机器人厂商已经提供了闭源实时控制器且不开放接口（多数工业臂本体）——这时 ros2_control 只能包一层，得不到实时收益
  2. 你只需要发关节位置指令、不需要控制器热切换与资源仲裁——直接用厂商 SDK 更省事
- **近 12 个月变化**：Kilted → Lyrical 有明确的 breaking change 清单，**跨发行版升级不是无痛的**，官方专门维护迁移说明 (evidence: [T02-S005])
- **Decay risk**：low

### 3. MuJoCo（含 MJX / MuJoCo Warp）

- **One-liner**：接触仿真的学术事实标准。2021 年被 DeepMind 收购并开源，从此成了论文默认。
- **Tier**：必备
- **维护方**：Google DeepMind
- **许可证**：Apache-2.0（这是它 2021 年后爆发的直接原因——之前是商业授权）
- **成熟度信号**：star 14,873、最后 push 2026-09-02；最近五个版本 3.12.0 (2026-08-20) / 3.11.0 (2026-07-28) / 3.10.0 (2026-06-23) / 3.9.0 (2026-05-27) / 3.8.1 (2026-05-11)——**月度发布节奏** (evidence: [T02-S028])
- **接触求解器的性质（这是选型的关键）**：MuJoCo 用**软约束 / 凸优化型**接触模型（可配的 solref/solimp），它的好处是**数值稳定、不容易穿模、可微**；代价是**接触是"软"的**——真实刚性碰撞的冲击力被平滑掉了。后果很具体：**在 MuJoCo 里插销装配、拧螺丝、刮擦这类刚性接触任务的行为，和真机差别最大**；而抓取、推动、腿式支撑相这类任务迁移得相当好 (evidence: [T02-S029, T06-S076])
- **MJX 与 MuJoCo Warp 的关系（容易搞混）**：
  - **MJX** = MuJoCo 的 JAX 重写，跑 GPU/TPU 上做大规模并行；**功能是 MuJoCo 的子集**——不支持全部约束类型、传感器、碰撞几何组合，官方专门列了差异表。**把 MuJoCo 模型直接扔进 MJX 常常跑不动或行为不同** (evidence: [T02-S031])
  - **MuJoCo Warp（MJWarp）** = 基于 NVIDIA Warp 的 GPU 后端，仓库建于 2025-03-17，版本号已与主线对齐（v3.12.0 / 2026-08-20）。这是 DeepMind 的新赌注，**它和 MJX 在长期是重叠的** (evidence: [T02-S030, T02-S050])
- **什么情况下不该用它**：
  1. **需要高保真的刚性接触与摩擦细节**（精密装配的力曲线）——MuJoCo 的软接触会系统性低估冲击，改用 Drake 的水弹性接触模型或直接上真机
  2. **需要传感器渲染吞吐**（大批量 RGB-D 训练）——MuJoCo 的渲染不是它的强项，ManiSkill / Isaac Lab 更合适
  3. **需要流体、软体、可变形材料**——原生支持有限
- **Decay risk**：low

### 4. NVIDIA Isaac Sim + Isaac Lab

- **One-liner**：GPU 上开几千个并行环境跑 RL 的工业级路径。足式运动控制的绝大多数落地策略是在这条线上训出来的。
- **Tier**：必备（如果你做 RL / 足式 / 大规模合成数据）；否则是场景特化
- **维护方**：NVIDIA
- **许可证**：Isaac Sim 已开源，**Apache-2.0 + NVIDIA 补充许可条款**；Isaac Lab 为 BSD-3-Clause (evidence: [T02-S032, T02-S033])
- **成熟度信号**：Isaac Lab star 8,026、最后 push 2026-09-02；`v3.0.0-beta2.patch1` 于 2026-07-02，对应 Isaac Sim 6.0.1；稳定线为 v2.3.x（对应 Isaac Sim 5.0+）(evidence: [T02-S033])
- **它和 Isaac Gym 的关系（必须讲清，因为老教程全是错的）**：
  - **Isaac Gym（Preview 版）**是 2021–2022 年的独立产品，`IsaacGymEnvs` 是它的环境集合。**它已经停止更新**，NVIDIA 官方路径是迁移到 Isaac Lab (evidence: [T02-S035, T02-S036])
  - 中间还夹过一个 **Orbit**（Isaac Lab 的前身，2023 年改名）。所以你在网上会看到 Isaac Gym / IsaacGymEnvs / Orbit / Isaac Lab 四个名字指着一条演进线——**只有 Isaac Lab 是活的**
  - **2026 年正在发生第三次断层**：Isaac Lab 3.0 引入多物理后端（含 Newton）、可插拔渲染、kit-less 工作流，是架构级重写。这意味着 **2.x 的环境代码不保证平移到 3.0**
- **真实使用门槛（这是它最被低估的部分）**：
  - **强绑 NVIDIA GPU**，且对显存与驱动版本敏感；没有 RTX 级显卡基本别开始
  - 安装体量以十 GB 计，Omniverse Kit 依赖链复杂，**在无网/内网环境部署是一件独立的工程**
  - 资产要走 **USD** 格式；从 URDF/MJCF 转过来通常需要手工修补物理属性
- **什么情况下不该用它**：
  1. **只跑单环境的算法调试** — 启动开销比迭代还长，MuJoCo 快十倍
  2. **没有 NVIDIA 显卡 / 必须跑在 CPU 集群上** — 直接出局
  3. **想要一个能长期锁定不变的仿真基座** — 过去 5 年它改了 4 次名字与架构，pin 版本是必须的
- **Decay risk**：medium（产品本身长期存在，但**接口层 12 个月内显著变化的概率超过 40%**）

### 5. Gazebo（Jetty）

- **One-liner**：ROS 生态默认的**系统级**仿真器——重点不是接触物理有多准，而是传感器插件、多机器人、世界与光照建模一应俱全。
- **Tier**：必备（做移动机器人 / 系统集成）
- **维护方**：OSRA
- **许可证**：Apache-2.0
- **版本与生命周期（改名史是坑）**：Gazebo → Ignition Gazebo（2019 起）→ 2022 年改回 **Gazebo**（新代码库），老的叫 **Gazebo Classic**。当前：**Jetty（2025-09 发布，LTS 至 2031-05）**、Harmonic（2023-09，LTS 至 2029-05）、Ionic（2024-09，非 LTS，2026-12 EOL）(evidence: [T02-S037])
- **成熟度信号**：`gz-sim` star 1,479、最后 push 2026-09-02；gz-sim11 预发布 2026-08-20 (evidence: [T02-S038])
- **什么情况下不该用它**：
  1. **接触密集的操作任务** — 它的物理默认是 DART/ODE 系，接触参数难调，做插孔装配不如 MuJoCo/Drake
  2. **大规模并行 RL** — 它是单实例系统仿真，不是万环境并行的形态
  3. **还在用 Gazebo Classic 的教程** — Classic 已停止支持，新项目起在 Classic 上等于起在废墟上 (evidence: [T02-S039])
- **Decay risk**：low（Jetty 的 LTS 到 2031）

### 6. MoveIt 2

- **One-liner**：机械臂运动规划的集成层——碰撞检查、规划、时间参数化、执行、场景管理打包在一起。
- **Tier**：必备（机械臂方向）
- **维护方**：MoveIt 社区，商业支持方是 **PickNik Robotics** (evidence: [T02-S016])
- **许可证**：BSD-3-Clause
- **成熟度信号**：star 1,986、最后 push 2026-09-02；2026 年内连续发版 2.15.0 (2026-08-12)、2.15.1 (2026-08-29)、2.5.10 (2026-09-01，老线维护) (evidence: [T02-S015])
- **真实使用门槛**：配置一套 MoveIt 需要 URDF + SRDF + 运动学插件 + 控制器接口全部对齐，**`moveit_setup_assistant` 走一遍只是起点**。真机上碰撞模型（尤其是工装、线缆、相机支架）不建全，规划出来的轨迹会撞。
- **「能跑通 demo」与「能进产线」的差距在这里最明显**：
  - MoveIt 的 demo（在 RViz 里拖一个球，机械臂避障过去）十分钟就能跑
  - 产线上真正难的是：**节拍**（默认规划器出的轨迹又慢又绕）、**可重复性**（采样式规划每次路径不同，工艺工程师不接受）、**异常恢复**。多数产线交付最后是**离线示教 + 固定轨迹**，MoveIt 只在换型与避障工位上用
  - 需要多阶段任务（抓 → 移动 → 放，中间有约束）时用 **MoveIt Task Constructor**，但它的文档与稳定性明显弱于主线 (evidence: [T02-S135])
- **什么情况下不该用它**：固定节拍、固定工装、路径不变的产线——直接示教器示教，MoveIt 是纯负担
- **Decay risk**：low

### 7. Pinocchio

- **One-liner**：刚体动力学 + **解析导数**。它是 Crocoddyl、大量 MPC/WBC/IK 实现的地基，你可能没直接用过但一定在依赖它。
- **Tier**：必备（做控制/优化）
- **维护方**：INRIA / LAAS-CNRS（Justin Carpentier 等）
- **许可证**：BSD-2-Clause（商用友好，这在学术库里不是默认）
- **成熟度信号**：star 3,704、最后 push 2026-09-02；4.1.0 (2026-07-07)、4.0.0 (2026-04-13)——**4.0 是大版本，API 有变** (evidence: [T02-S019])
- **什么情况下不该用它**：只需要正/逆运动学、不需要动力学与导数时，用 KDL 或厂商 SDK 更轻
- **Decay risk**：low

### 8. OpenCV

- **One-liner**：图像处理与相机标定的地板。机器人里 90% 的「标定」代码最后调的是 OpenCV。
- **Tier**：必备
- **维护方**：OpenCV 基金会
- **许可证**：Apache-2.0（4.5.0 起从 BSD-3 改为 Apache-2.0）
- **成熟度信号**：star 90,686、最后 push 2026-09-02。**当前是双线并行**：**OpenCV 5.0.0 于 2026-06-26 发布**，同时 4.x 线仍在更新（4.14.0 / 2026-07-19）(evidence: [T02-S052, T02-S053])
- **2026 年的实际决策**：**新项目别急着上 5.0**。5.0 是有破坏性变更的大版本，而机器人栈里大量下游包（ROS 的 vision_opencv、各家相机 SDK）仍以 4.x 为准。稳妥做法是继续 4.x，等下游生态跟上 (evidence: [T02-S053])
- **什么情况下不该用它**：需要 GPU 端到端流水线（解码 → 预处理 → 推理）时，OpenCV 的 CUDA 模块拼不出完整链路，用 Isaac ROS / DeepStream 系更合适 (evidence: [T02-S134])
- **Decay risk**：low

### 9. LeRobot

- **One-liner**：把「采数据 → 存成统一格式 → 训策略 → 部署到真机」这条链做成一个包。它是 2024 年以后模仿学习与 VLA 的默认入口。
- **Tier**：必备（学习驱动的操作方向）
- **维护方**：Hugging Face
- **许可证**：Apache-2.0
- **成熟度信号**：star **27,156**（2026-09-02 查）、最后 push 2026-09-02；v0.6.1 (2026-08-03)、v0.6.0 (2026-07-08)、v0.5.1 (2026-04-07)、v0.5.0 (2026-03-09) (evidence: [T02-S073])。**版本号还在 0.x**——这是重要信号：**接口仍在破坏性变化**。
- **它真正解决的问题**：不是算法，是**数据格式与硬件接入的碎片化**。在它之前每个实验室一套 HDF5 结构；现在 `LeRobotDataset` 成了事实标准，Hub 上能直接下别人的数据 (evidence: [T02-S074, T05-S098])
- **门槛**：低到危险——一个 SO-101 + 一台笔记本就能开始。**这正是它的风险**：入门快，但「采了 50 条数据策略不 work」之后的所有问题（数据质量、相机位姿一致性、动作空间定义）它不替你解决
- **什么情况下不该用它**：
  1. **做力控/接触密集任务** — 它的主线数据管线是视觉 + 关节位置，力/力矩通道支持不成体系
  2. **做工业级部署** — 0.x 的接口稳定性不支持长期维护；产品化通常要 fork 冻结
  3. **足式运动控制** — 那是 RL 的地盘（RSL-RL + Isaac Lab），不是这条线
- **近 12 个月变化**：v0.5.0（2026-03）增加 Unitree G1 支持并进入 ICLR 2026 相关工作；此后半年内又发了 0.6.0/0.6.1 两个次版本 (evidence: [T05-S027, T02-S073])
- **Decay risk**：medium（项目本身会活，但**接口 12 个月内变的概率很高**）

### 10. Rerun

- **One-liner**：把时间序列 + 图像 + 点云 + 位姿放在同一条时间轴上看。调机器人时你 80% 的时间在「对齐几个数据流」，它就是干这个的。
- **Tier**：必备（调试与数据检查）
- **维护方**：Rerun（瑞典公司，rerun.io）
- **许可证**：Apache-2.0（**SDK 与 viewer 都开源**，这是它与 Foxglove 的关键差别）
- **成熟度信号**：star 11,384、最后 push 2026-09-02；0.37.0 于 2026-09-01 发布，0.36.3 于 2026-08-26——**周级发布节奏** (evidence: [T02-S090])
- **什么情况下不该用它**：
  1. **需要长期归档与团队协作的数据平台** — Rerun 定位是本地/进程内可视化，团队级数据管理是 Foxglove 的地盘
  2. **需要与 rosbag 生态深度耦合** — rosbag2 + PlotJuggler 的路径更直接
- **Decay risk**：medium（公司支撑，商业模式仍在演进；**0.x 版本号意味着 API 会变**）

### 11. rosbag2 + MCAP + PlotJuggler（记录与回放三件套）

- **One-liner**：出了事故，能不能复盘只取决于你有没有录、录得全不全。这三样是这条链上的默认件。
- **Tier**：必备
- **维护方 / 许可证**：rosbag2（ROS 2 项目 / Apache-2.0）；**MCAP**（Foxglove 发起的容器格式 / 开源规范）；PlotJuggler（Davide Faconti / **MPL-2.0**）
- **成熟度信号**：rosbag2 最后 push 2026-09-02，双线维护 0.33.3 (2026-05-12) / 0.26.11 (2026-06-03)；PlotJuggler star 6,138、`PlotJuggler 4 beta3` 于 2026-08-15 (evidence: [T02-S092, T02-S094])
- **关键工程事实**：**rosbag2 的默认存储格式已经是 MCAP**（取代早期的 sqlite3）。MCAP 是自描述的、可跨语言读、支持部分损坏文件恢复——这对现场事故录像很重要 (evidence: [T02-S093])
- **什么情况下不该用它**：
  1. 高带宽视频流全量录制 —— 直接录 bag 会打爆磁盘与 IO，实践是**降采样 + 关键帧 + 单独录压缩视频**
  2. 需要跨车队的长期数据仓库 —— bag 文件不是数据库，要上专门的数据平台
- **避坑**：**PlotJuggler 是 MPL-2.0**——比 GPL 宽松（文件级 copyleft，可以链接进闭源），但如果你改了它的源码分发，改动部分要开源
- **Decay risk**：low


## 二、场景特化层 — 选它意味着接受特定代价

### 12. Drake

- **One-liner**：把机器人当**数学问题**来做的工具箱——多体动力学 + 数学规划（LP/QP/SDP/SOS）+ 系统框图，接触建模是它的招牌。
- **维护方**：Toyota Research Institute + MIT（Russ Tedrake）｜**许可证**：BSD-3-Clause (evidence: [T02-S026])
- **成熟度**：star 4,165、最后 push 2026-09-02；**月度发版** v1.56.0 (2026-08-14) / v1.55.0 (2026-08-07) / v1.54.0 (2026-06-12)
- **典型场景**：(1) 需要**可验证**的接触模型（水弹性接触 hydroelastic，能给出接触面而非单点力）做精密装配；(2) 需要在同一框架里写轨迹优化 + 逆运动学 + 控制器综合；(3) 教学——Tedrake 的两门在线教材直接绑 Drake (evidence: [T05-S062, T05-S063])
- **代价**：学习曲线是本文件里最陡的一档；生态自成体系，与 ROS 2 集成要自己搭桥；**没有大规模并行 GPU 训练路径**
- **不该用它**：只想快速训一个 RL 策略；团队里没人愿意读 500 页教材
- **Decay risk**：low

### 13. Genesis

- **One-liner**：2024 年底出现的 Python-native 仿真平台，卖点是跨材料（刚体/软体/流体/布料）统一 + 极高吞吐。
- **维护方**：Genesis Embodied AI（多校联合）｜**许可证**：Apache-2.0 (evidence: [T02-S041])
- **成熟度**：star **29,856**（2026-09-02 查，是本文件里 star 最高的仿真器）；v1.3.3 (2026-08-13)，2026 年 7–8 月连发 1.3.0/1.3.1/1.3.2/1.3.3——**周级迭代**
- **吞吐口径的争议（必须写清）**：发布时宣称的「**4300 万 FPS**」是**特定场景 + RTX 4090 + 极简刚体设置**下的数字，与「你的实际训练任务能跑多快」不是一回事；社区复现时在含视觉观测、复杂接触的场景下差距很大。**引用这个数字前必须问：什么机器人、什么求解器、多少并行环境、有没有渲染** (evidence: [T02-S040])
- **典型场景**：需要软体/流体与刚体混合的研究；想要一个不绑 NVIDIA Omniverse 的 Python 栈
- **代价**：**sim-to-real 的证据链很短**——2024-12 才发布，公开的「用 Genesis 训出来、在真机上跑通」的案例仍稀少。star 数高 ≠ 生产采用
- **不该用它**：产品交付；任何需要「这个仿真结果可信」作为论据的场合
- **Decay risk**：high

### 14. ManiSkill 3 + SAPIEN

- **One-liner**：GPU 并行的**操作任务**仿真与基准，强在**视觉观测吞吐**（并行渲染），这正是 Isaac 之外的另一条路。
- **维护方**：UCSD Hao Su 组 / Hillbot Inc.｜**许可证**：ManiSkill Apache-2.0；SAPIEN Apache-2.0（版权页已含 Hillbot Inc.，即该组的公司化实体）(evidence: [T02-S042, T02-S043])
- **成熟度**：ManiSkill star 3,283，**v3.0.1 于 2026-04-21 正式脱离 beta**（此前 b23 系列跑了两年多）；SAPIEN star 829、最后 push 2026-07-18
- **典型场景**：需要同时要**并行 + 视觉**的操作策略训练；做跨算法的操作基准对比
- **代价**：绑 SAPIEN 渲染栈；**分数与 Isaac Lab / robosuite 完全不可比**（引擎、控制频率、成功判定都不同）(evidence: [T05-S055])
- **不该用它**：足式运动（生态在 Isaac 那边）；需要接触力保真度的装配研究
- **Decay risk**：medium

### 15. robosuite

- **One-liner**：MuJoCo 上一套干净、协议严格的操作环境集合，做算法消融的标准台面。RoboCasa 就建在它上面。
- **维护方**：ARISE Initiative（Stanford SVL + UT Austin RPL）｜**许可证**：MIT (evidence: [T02-S044])
- **成熟度**：star 2,586；v1.5.2 (2025-12-24)、v1.5.1 (2025-02-08)、最后 push 2026-07-11——**发版节奏放缓到年度级**
- **典型场景**：写论文要一个大家都认的消融环境；教学
- **代价**：单机为主，并行吞吐远不如 GPU 方案；环境偏"干净"，泛化结论外推要谨慎
- **不该用它**：判断一个方法能不能上真机
- **Decay risk**：medium

### 16. Webots

- **One-liner**：开箱即用模型最多的教育/竞赛仿真器，2018 年从商业软件转为开源。
- **维护方**：Cyberbotics｜**许可证**：Apache-2.0 (evidence: [T02-S047])
- **成熟度**：star 4,592、最后 push 2026-09-01；**发布形态是 nightly build**（2026-08-31 仍在出）
- **典型场景**：机器人课程；RoboCup 类竞赛；快速验证一个多机器人协作想法
- **代价**：工业交付里基本不用；物理引擎（ODE 系）不适合接触密集任务
- **不该用它**：任何要把仿真结果当 sim-to-real 依据的场合
- **Decay risk**：medium

### 17. CoppeliaSim（原 V-REP）

- **One-liner**：脚本化极强的工位级仿真器——传送带、PLC 逻辑、多机器人、视觉传感器能在一个场景里拼出来。
- **维护方**：Coppelia Robotics（瑞士）｜**许可证**：**商业软件**，教育版免费，商用需付费授权 (evidence: [T02-S048])
- **典型场景**：产线工位方案论证（给客户看节拍与干涉）；集成商做前期可行性
- **代价**：闭源 + 授权成本；社区规模远小于 Gazebo/Isaac；不适合作为学习算法的训练后端
- **不该用它**：需要大规模并行训练；需要把仿真器改到底层
- **Decay risk**：medium

### 18. PyBullet / Bullet3

- **One-liner**：2018–2022 年 RL 论文的默认物理引擎。**现在它主要是历史包袱**。
- **维护方**：Bullet 社区（Erwin Coumans 已转向其他项目）｜**许可证**：zlib（Extras 与第三方目录另有许可）(evidence: [T02-S045])
- **成熟度**：star 14,711，但**最后 push 是 2025-10-22**（2026-09-02 查）——距今约 10 个月，**维护实质停滞**
- **它的真实问题**：接触求解在刚性接触下容易抖动/穿模，摩擦模型简化，**大量 2019–2022 年的 sim-to-real 结论建立在它之上**，这些结论今天不能直接外推
- **什么时候还可以用**：复现老论文；教学演示；不需要接触保真度的运动学验证 (evidence: [T02-S046])
- **不该用它**：任何新项目的仿真基座；任何要拿仿真数字说服人的场合
- **Decay risk**：high（已在衰退，不是会衰退）

### 19. OMPL

- **One-liner**：采样式运动规划算法（RRT/RRT*/PRM/BIT*/KPIECE…）的权威实现库，MoveIt 的默认后端。
- **维护方**：Rice University Kavraki Lab｜**许可证**：**3-clause BSD**（Copyright 2010-2025 Rice University）(evidence: [T02-S017, T02-S018])
- **成熟度**：star 2,137；OMPL **2.0.2 (2026-08-14)**、2.0.1 (2026-06-19)——**2.0 是大版本，API 有变**
- **典型场景**：高维构型空间的无碰撞路径搜索；需要换算法做对比
- **代价**：**只管几何路径**——不管动力学、不管时间、不管力。规划完还要接 TOPP-RA 做时间参数化
- **不该用它**：需要考虑动力学可行性的足式/欠驱动系统（那是 Crocoddyl/OCS2/Drake 的活）
- **Decay risk**：low

### 20. Crocoddyl

- **One-liner**：足式与全身系统的 DDP/FDDP 类最优控制求解器，建在 Pinocchio 的解析导数上，能跑到 MPC 频率。
- **维护方**：LAAS-CNRS + University of Edinburgh｜**许可证**：BSD-3-Clause (evidence: [T02-S020])
- **成熟度**：star 1,296；v3.2.1 (2026-05-10)、v3.2.0 (2025-12-09)，最后 push 2026-09-01
- **典型场景**：四足/人形的接触序列已知时的全身轨迹优化；需要在几毫秒内解出来
- **代价**：需要真懂最优控制——代价函数与正则项调不好直接发散；接触序列通常要外部给
- **不该用它**：把它当"规划器"用（它是求解器，需要一个上层给接触模式）
- **Decay risk**：medium

### 21. OCS2

- **One-liner**：ETH 机器人系统实验室（ANYmal 血统）的最优控制工具箱，把足式 MPC 从论文做成了可复用的一套。
- **维护方**：ETH Zurich Robotic Systems Lab｜**许可证**：BSD-3-Clause (evidence: [T02-S021])
- **成熟度**：star 1,507、最后 push 2026-07-20——**比 Crocoddyl 慢**
- **典型场景**：四足 MPC 的工程起点；需要 SLQ/DDP + 约束处理的成套实现
- **代价**：编译重、文档薄、依赖多；很多示例仍带 ROS 1 时代的假设
- **不该用它**：只做机械臂；团队没有能读 C++ 模板重代码的人
- **Decay risk**：medium

### 22. TOPP-RA

- **One-liner**：把一条几何路径变成满足速度/加速度/力矩约束的**时间最优**轨迹。规划器与真机之间那一小段，缺了它机械臂就会抖或超限。
- **维护方**：Hung Pham（NTU）｜**许可证**：MIT (evidence: [T02-S022])
- **成熟度**：star 925；0.6.10 (2026-08-28)、0.6.9 (2026-07-28)——**仍在月度更新**
- **典型场景**：MoveIt 之外自己搭规划链路；需要在关节力矩约束下压节拍
- **代价**：只解决时间参数化，不是规划器；约束建模不准会出"看着能跑、真机报超速"的轨迹
- **Decay risk**：low

### 23. QP 求解器三选一：OSQP / ProxQP / qpOASES

- **One-liner**：WBC、MPC、导纳控制的内环最后都归结成一个二次规划。求解器选错，控制环就超时。
- **维护方 / 许可证**：OSQP（Apache-2.0，v1.0.0 于 2025-03-21——**十年才到 1.0**）；ProxQP / ProxSuite（INRIA Willow，BSD-2，v0.7.3 于 2026-05-11）；qpOASES（COIN-OR，**LGPL-2.1**）(evidence: [T02-S023, T02-S024, T02-S025])
- **怎么选（有实际分界）**：
  - **OSQP**：ADMM 一阶方法，问题规模大、精度要求不极端、需要热启动 → 首选，且许可证最干净
  - **ProxQP**：近端方法，**在病态/退化问题上比 OSQP 稳**，是 Pinocchio/INRIA 栈的原生搭配
  - **qpOASES**：在线主动集，小规模 MPC 上能给出高精度解且热启动极快；**但 LGPL-2.1，静态链接进闭源产品要走动态链接或谈授权**
- **不该做的事**：拿默认参数直接进 1 kHz 控制环——**必须实测最坏情况求解时间**，而不是平均时间
- **Decay risk**：low

### 24. Nav2

- **One-liner**：ROS 2 移动机器人导航栈——行为树调度 + 代价地图 + 规划器/控制器插件 + 恢复行为。
- **维护方**：Nav2 项目（Steve Macenski 等）｜**许可证**：Apache-2.0 (evidence: [T02-S131, T02-S132])
- **典型场景**：AMR/AGV、巡检机器人、服务机器人底盘；移动操作的"移动"那一半
- **代价**：面向 2D/2.5D 平面导航；参数极多，**调参是真实工作量**（代价地图膨胀半径、控制器前瞻、恢复策略）
- **不该用它**：足式在崎岖地形上的导航（需要高程图与足端规划）；室内高精度对接（要专门的视觉伺服）
- **合规提示**：AMR 类产品的安全要求走 **ISO 3691-4** 与 **ANSI/RIA R15.08**，与软件栈无关但决定你能不能卖 (evidence: [T06-S010, T06-S028])
- **Decay risk**：low

### 25. GTSAM

- **One-liner**：因子图优化的工业级后端——SLAM、多传感器融合、标定，凡是"把一堆约束拧成一个最优估计"的都能用它。
- **维护方**：Georgia Tech Borg Lab（Frank Dellaert）｜**许可证**：simplified BSD (evidence: [T02-S059])
- **成熟度**：star 3,663；Release 4.3a2 (2026-08-04)、4.2.2 (2026-06-30)，最后 push 2026-09-01
- **典型场景**：自研 VIO/LIO 后端；多相机-IMU-轮式里程计的联合标定与融合
- **代价**：要理解因子图、流形上的优化、噪声模型——**不是拿来即用的 SLAM 系统**
- **不该用它**：只想跑通一个建图 demo（用 RTAB-Map 或 Cartographer 更快）(evidence: [T02-S066, T02-S067])
- **Decay risk**：low

### 26. 视觉/视觉惯性 SLAM 三件套：ORB-SLAM3 / VINS-Fusion / OpenVINS

- **One-liner**：学术界公认的三个 VIO/SLAM 基线。**它们的共同点比技术差异更重要：全是 GPL-3.0。**
- **维护方 / 许可证 / 活跃度**：
  - ORB-SLAM3（Univ. Zaragoza，**GPL-3.0**，star 9,015，**最后 push 2024-07-24**）
  - VINS-Fusion（HKUST 沈劭劼组，**GPL-3.0**，star 4,693，**最后 push 2024-05-23**）
  - OpenVINS（University of Delaware RPNG，**GPL-3.0**，star 3,075，最后 push 2025-11-30——**三个里最活的**）
  (evidence: [T02-S056, T02-S057, T02-S058])
- **代价（这条是法务问题不是技术问题）**：**GPL-3.0 的传染性意味着把它们链接进闭源产品需要开源你的整个程序**。国内交付里这是最常被忽略、最晚被发现的雷。产品路线通常是：用它们做基线评估 → 自研或买商业 VIO（或用 BSD 的 GTSAM 自己搭后端）
- **不该用它**：任何要闭源分发的产品；需要长期维护的量产项目（三者都以研究代码形态存在）
- **Decay risk**：medium（作为基线 low；作为产品件 high）

### 27. Open3D / PCL

- **One-liner**：点云的读写、滤波、配准（ICP/GICP）、可视化与重建。
- **维护方 / 许可证**：Open3D（Intel ISL 起源，**MIT**）；PCL（社区，**BSD**）(evidence: [T02-S054, T02-S055])
- **成熟度（要看清）**：Open3D star 13,931、最后 push 2026-09-01，但**最近的正式版是 v0.19 (2025-01-10)**，之后只有 devel 包——正式发布节奏明显放缓；PCL star 11,106、最后 push 2026-08-29，最近正式版 1.15.1 (2025-08)——**以维护更新为主，不是活跃演进**
- **怎么选**：Python 侧原型与可视化 → Open3D；C++ 侧与 ROS 深度集成、需要老算法的完整实现 → PCL
- **不该用它**：需要深度学习点云算子（用 PyTorch3D / MinkowskiEngine 系）；需要实时大场景（用专门的 LIO 实现）
- **Decay risk**：medium（两者都进入稳态维护期，不是衰亡但也别期待新特性）

### 28. Kalibr / easy_handeye(2)

- **One-liner**：标定这件事只有两类工具——相机-IMU 时空标定（Kalibr）与手眼标定（easy_handeye）。**它们决定了你的绝对精度上限。**
- **维护方 / 许可证**：Kalibr（ETH ASL，**BSD**，star 5,696，**最后 push 2024-03-30**）；easy_handeye（TUM CAMP，star 1,174，最后 push 2025-11-30）；**ROS 2 用户要用 easy_handeye2**（独立维护）(evidence: [T02-S060, T02-S061, T02-S062])
- **典型场景**：eye-in-hand / eye-to-hand 外参求解；多相机 + IMU 的时间偏移标定
- **真实门槛（被严重低估）**：标定板质量、光照、运动激励充分性、温漂——**标定失败的原因 90% 在数据采集，不在算法**。一次合格的手眼标定通常要采 20–30 个姿态且覆盖足够的旋转空间；重投影误差（reprojection error）应看到亚像素级，看不到就是数据不合格 (evidence: [T02-S060, T06-S006])
- **不该用它**：以为标定一次就永久有效——**碰撞、拆装、温度变化后都要重标**，产线上要有定期复标 SOP
- **Decay risk**：medium（Kalibr 已两年多未更新，是明确的风险点）

### 29. FoundationPose / MegaPose / SAM 2

- **One-liner**：不训练专用模型也能拿到物体的 6D 位姿与实例掩码——2024 年以后抓取流水线的新默认前端。
- **许可证（这是选型的第一决策点，不是最后）**：
  - **FoundationPose：NVIDIA 源代码许可，明文限定「may be used or intended for use non-commercially… research or evaluation purposes only」——不能进商业产品** (evidence: [T02-S063])
  - **MegaPose**（INRIA Willow）：开源许可，商用需自行核对具体条款 (evidence: [T02-S064])
  - **SAM 2**（Meta AI）：**Apache-2.0，可商用** (evidence: [T02-S139, T02-S065])
- **成熟度**：FoundationPose star 3,531、最后 push 2026-04-29
- **典型场景**：新物体（无 CAD 或只有 CAD 无标注数据）的抓取位姿；杂乱堆叠场景的实例分割
- **代价**：推理开销大（通常要独立 GPU），**延迟直接吃进节拍**；对纹理缺失、透明、高反光物体仍然差
- **不该用它**：固定 SKU 的高节拍产线（专用模型或传统模板匹配又快又稳）；任何把 FoundationPose 写进商业方案的场合
- **Decay risk**：high

### 30. robomimic + Diffusion Policy

- **One-liner**：模仿学习的标准实现与消融基线。robomimic 回答"同样的数据换个算法能好多少"，Diffusion Policy 是 2023 年以后操作策略的默认结构。
- **维护方 / 许可证**：robomimic（ARISE Initiative，**MIT**，star 1,541，最后 push 2026-08-09）；Diffusion Policy（Columbia / Stanford / TRI，**MIT**）(evidence: [T02-S078, T02-S084])
- **典型场景**：拿到一批遥操作数据后，先用 robomimic 跑 BC/BC-RNN/Diffusion 的横向对比，再决定投入哪条线
- **代价**：论文级封装——数据管线、实验追踪、模型版本管理、真机回滚全要自己补
- **不该用它**：直接作为产品训练框架（多数团队 fork 后重写数据层）；力控任务（观测里没有力通道）
- **Decay risk**：medium

### 31. RL 训练库四选一：RSL-RL / skrl / Stable-Baselines3 / RLlib

- **怎么选（分界很清楚）**：
  - **RSL-RL**（ETH RSL + NVIDIA，star 2,937，最后 push 2026-08-31）：**极简、只做 GPU 上的 on-policy PPO**，是四足/人形运动策略的事实默认，因为它和 Isaac Lab 的向量化环境是一套血统。代价：功能少到近乎没有——没有 off-policy、没有分布式调度 (evidence: [T02-S080])
  - **skrl**（MIT，star 1,095，最后 push 2026-05-11）：统一封装 Isaac Lab / Isaac Gym / Gymnasium / PettingZoo 多个后端，适合要跨仿真器比较 (evidence: [T02-S081])
  - **Stable-Baselines3**（DLR-RM，MIT，star 13,755）：实现最可信、文档最好，但**面向单环境/中小规模**，不是给几千并行环境准备的 (evidence: [T02-S082])
  - **RLlib / Ray**（Apache-2.0，Ray star 43,684）：需要多机分布式、超参搜索、异构资源调度时才值得那份复杂度 (evidence: [T02-S083])
- **不该做的事**：为了"工程完备"上 RLlib 跑一个单机四足训练——启动与调试成本远超收益
- **Decay risk**：medium

### 32. 实时与总线链路：micro-ROS + PREEMPT_RT + SOEM/IgH + CANopen

- **One-liner**：从上位机到伺服的真实控制链路。这一层没有"框架"，只有一条条要自己证明的时序。
- **组成与许可证**：
  - **micro-ROS**（Apache-2.0，`micro_ros_setup` 6.1.0 / 2026-08-11）——在 MCU（FreeRTOS/Zephyr/裸机）上跑 ROS 2 客户端 (evidence: [T02-S008, T02-S009])
  - **PREEMPT_RT**——Linux 实时补丁，**主线化工作已基本完成**，但"打了补丁"不等于"实时"：还要隔核、关节能省电、设 CPU 亲和、避免页错误 (evidence: [T06-S072])
  - **SOEM**（OpenEtherCAT Society，**v2.0.0 / 2025-07-11**，是 1.4.0 之后时隔六年的大版本）——用户态 EtherCAT 主站，简单、易嵌入 (evidence: [T02-S010])
  - **IgH EtherCAT Master**（**GPLv2**）——内核态主站，抖动更好，**但 GPL 且要跟内核版本** (evidence: [T02-S011])
  - **CANopen / CiA 402**——ros_canopen（**LGPL-3.0**，最后 push 2025-04-14）与 ros2_canopen (evidence: [T02-S012, T02-S013, T06-S071])
- **口径提醒**：EtherCAT 常被宣传成"微秒级"，那是**协议层的周期能力**，不等于你的应用能在这个周期里稳定完成计算。真正要测的是**端到端抖动的最坏值（p99.9 / max）**，不是平均值 (evidence: [T06-S070])
- **不该做的事**：用 Xenomai 起新项目——双内核方案维护成本高、社区活跃度已明显落后于 PREEMPT_RT (evidence: [T02-S014])
- **Decay risk**：low（这一层十年不怎么变，是最保值的知识）

### 33. Isaac ROS

- **One-liner**：NVIDIA 把感知算子（AprilTag、立体深度、分割、位姿估计、nvblox 建图）做成 GPU 加速的 ROS 2 包，跑在 Jetson 与 x86+RTX 上。
- **维护方**：NVIDIA｜**许可证**：多数包 Apache-2.0，但**部分模型权重与组件另有 NVIDIA 条款**，商用前要逐包核对 (evidence: [T02-S134])
- **典型场景**：Jetson 上要把感知延迟压下去；需要零拷贝的 GPU 图像管线（NITROS）
- **代价**：**深度绑定 NVIDIA 硬件**；版本与 JetPack、Isaac Sim 三方对齐是持续的运维负担
- **不该用它**：非 NVIDIA 计算平台；需要长期锁定不变的软件基线
- **Decay risk**：medium

### 34. Foxglove

- **One-liner**：团队级的机器人数据可视化与协作平台——比 Rerun 更"平台"，比 RViz 更好用。
- **维护方**：Foxglove（美国公司）｜**许可证（重要变化）**：**Foxglove Studio 的开源版本已归档，产品转为商业闭源 + 免费额度**；开源的部分是 **MCAP 格式规范**，而不是查看器 (evidence: [T02-S091, T02-S093])
- **典型场景**：多人团队要共享一份现场数据并批注；需要把 bag 挂到云上给远程同事看
- **代价**：**按席位/用量收费**，且核心工具不再可自托管修改；对数据出境敏感的国内项目是硬门槛
- **不该用它**：数据不能出内网的国防/工业项目；个人调试（Rerun 更快且完全开源）
- **Decay risk**：medium

### 35. RealSense / ZED / Ouster / Livox（深度与激光传感器栈）

- **One-liner**：机器人感知的输入端。选型的第一问题不是精度，是**这条产品线三年后还在不在**。
- **关键事实（2026 年必须知道）**：
  - **RealSense 已从 Intel 独立成 RealSense AI**，GitHub 组织从 `IntelRealSense` 迁到 `realsenseai`，官网也换到 realsenseai.com。`librealsense` 仍在活跃更新（v2.58.4 beta / 2026-08-30）。历史上 Intel 曾在 2021 年宣布收缩 RealSense 业务、后又反复——**这条产品线的供应链稳定性有前科，长期项目要留替换方案** (evidence: [T02-S068, T02-S069])
  - **ZED（Stereolabs）**：纯双目 + 神经网络深度，室外强光下比结构光稳；SDK 闭源且**强绑 NVIDIA GPU**（zed-sdk MIT 但依赖闭源运行时）(evidence: [T02-S070])
  - **Ouster**：数字激光雷达，ROS 驱动官方维护；工业巡检与 AMR 常见 (evidence: [T02-S071])
  - **Livox**：非重复扫描模式，性价比高、国内供应链友好；**点云分布与传统机械式不同，很多现成 SLAM 算法要改** (evidence: [T02-S072])
- **不该做的事**：把三种原理（结构光 / ToF / 双目）的深度相机当成可互换件——它们在反光、透明、强光、近距下的失效模式完全不同 (evidence: [T02-S069, T02-S070, T02-S072])
- **Decay risk**：medium（硬件产品线变动是这一格的主要风险）


## 三、新兴层 — 12 个月内起势，标 experimental

> 这一层统一标 `stability: experimental`。判断标准：出现或起势 ≤ 12 个月，或**架构处于重写中**。**默认假设是「6 个月后接口不一样」**，所以任何用到它们的项目都必须 pin 版本 + 有退路。

### 36. MuJoCo Warp（MJWarp）

- **出现时间**：仓库建于 **2025-03-17**｜**维护方**：Google DeepMind｜**许可证**：Apache-2.0
- **成熟度**：star 1,432、最后 push 2026-09-02；版本号已与 MuJoCo 主线对齐（v3.12.0 / 2026-08-20、v3.11.0 / 2026-07-28）(evidence: [T02-S030])
- **为什么值得盯**：它是 DeepMind 把 MuJoCo 搬上 GPU 的**第二次尝试**（第一次是 MJX/JAX）。基于 NVIDIA Warp 内核，理论上覆盖度比 MJX 好。**如果它成，MJX 的地位会尴尬**——这两条线长期是重叠的
- **代价**：接口与功能覆盖仍在变；文档远薄于 MuJoCo 主线
- **不该用它**：任何要在未来 12 个月内交付的产品
- **Decay risk**：high

### 37. Newton（物理引擎）

- **出现时间**：2025 年公布，NVIDIA + Google DeepMind + Disney Research 联合｜**许可证**：Apache-2.0
- **成熟度**：star 5,576（2026-09-02 查）(evidence: [T02-S051, T02-S136])；底层依赖 NVIDIA Warp（star 7,066）(evidence: [T02-S050])
- **为什么值得盯**：它已经作为 **Isaac Lab 3.0 的可选物理后端**出现 (evidence: [T02-S033])。三家联手 + 进入 Isaac 主线，意味着未来两年「GPU 并行仿真的默认引擎是谁」这个问题可能被重新回答
- **代价**：还没有可引用的大规模 sim-to-real 成功案例；行为与 PhysX / MuJoCo 都不同，**已有的域随机化配方不能直接搬**
- **Decay risk**：high

### 38. Isaac Lab 3.0（beta）

- **出现时间**：3.0-beta 于 2026-03，beta2.patch1 于 **2026-07-02**（对应 Isaac Sim 6.0.1）(evidence: [T02-S033])
- **为什么值得盯**：这是一次**架构级重写**——多物理后端（PhysX / Newton）、可插拔渲染、kit-less 工作流。开发主线已切到 `develop` 分支，`main`（2.3.x）进入维护模式
- **代价（很实在）**：**2.x 的环境代码不保证平移到 3.0**。已经在 2.x 上训出策略的团队，升级 = 重新验证一遍 sim-to-real
- **建议**：新项目 pin 在 v2.3.x 稳定线上，直到 3.0 出正式版且有第三方复现报告；安装步骤与 Isaac Sim 版本的绑定关系以官方安装页为准 (evidence: [T02-S034])
- **Decay risk**：high

### 39. Genesis

- **出现时间**：2024-12 首发｜见上文场景特化层第 13 条的完整分析
- **早期采用者信号**：star 29,856（2026-09-02），远超所有其他仿真器——但**star 与生产采用在这一行严重脱钩**，这恰恰是需要警惕的信号
- **Decay risk**：high

### 40. openpi（π0 / π0.5）

- **出现时间**：仓库建于 **2024-10-21**｜**维护方**：Physical Intelligence｜**许可证**：Apache-2.0
- **成熟度**：star 13,588、最后 push 2026-08-24 (evidence: [T02-S075])
- **为什么值得盯**：它是**第一批把 VLA 模型权重 + 微调脚本以完全宽松许可证公开**的。在它之前，这一层要么闭源（RT-2），要么只有代码没有可用权重
- **代价**：
  1. **算力门槛真实存在**——微调需要多卡；推理要独立 GPU
  2. **默认假设你的本体接近它的训练分布**（桌面双臂 / 特定夹爪），换本体要重新做动作空间映射
  3. 公司驱动的开源，**路线随公司战略变**
- **不该用它**：足式运动控制；高精度力控装配；把它的 demo 成功率当作你的场景的预期
- **Decay risk**：high

### 41. Isaac GR00T N1.x

- **出现时间**：仓库建于 **2025-03-11**；N1.6 / N1.7 相关发布集中在 **2026-04**｜**许可证**：Apache-2.0
- **成熟度**：star 7,986、最后 push 2026-08-20 (evidence: [T02-S085])
- **为什么值得盯**：NVIDIA 在开源人形基础模型上的正面下注，配套的是合成数据生成管线（与 Isaac Sim/Lab 打通）
- **代价**：绑 NVIDIA 全栈；**「合成数据 + 少量真机」这条路线的独立第三方验证仍然稀薄**
- **Decay risk**：high

### 42. rmw_zenoh

- **出现时间**：2024 年 ROSCon 上正式介绍，此后进入 ROS 2 官方文档并被列为 **tier-1 中间件** (evidence: [T02-S133, T02-S141])
- **成熟度**：star 496——**star 低但重要性高**，因为它是 ROS 2 官方仓库下的组件，不是第三方项目
- **为什么值得盯**：DDS 的发现机制在**多机、跨网段、无线弱网、大规模节点**下问题很多。Zenoh 是十年来第一个被官方接纳的非 DDS 选项。另有 `zenoh-plugin-ros2dds` 走桥接路线，两者**不能互通**，要选一条 (evidence: [T02-S142])
- **代价**：生态工具（诊断、录制、第三方厂商驱动）仍默认 DDS；换了之后一些排错经验不适用
- **Decay risk**：medium

### 43. SO-100 / SO-101 + LeRobot 硬件生态

- **出现时间**：SO-100 于 2024 年，SO-101 于 2025 年｜**维护方**：The Robot Studio + Hugging Face 社区｜**许可证**：Apache-2.0（含 3D 打印件与 BOM）
- **成熟度**：`SO-ARM100` 仓库 star **7,270**（2026-09-02 查）(evidence: [T02-S086])
- **为什么值得盯**：它把「拥有一台能采数据的机械臂」的成本从几万美元压到**千元人民币级**（3D 打印件 + 舵机 + 一块控制板）。这不是技术突破，是**准入门槛的塌陷**——直接后果是 HF Hub 上社区数据集的爆发式增长 (evidence: [T05-S098, T02-S073])
- **代价（必须说清）**：
  - **舵机级精度与刚度**，没有力矩传感、没有可靠重复定位指标、负载极小
  - 采出来的数据**没有统一标定与相机位姿协议**，直接混训会引入大量噪声 (evidence: [T05-S053])
  - **它是学习工具与数据生产工具，不是产品原型平台**
- **Decay risk**：high（硬件迭代快，SO-101 之后还会有）

### 44. InternUtopia（原 GRUtopia）

- **出现时间**：2024 年以 GRUtopia 发布，2025 年随上海 AI Lab 的 InternRobotics 体系更名｜**许可证**：以仓库为准，本轨未逐条核对
- **成熟度**：star 1,286（2026-09-02 查）(evidence: [T02-S130])
- **为什么值得盯**：中国侧少数做**场景级**（城市/室内大场景，而非桌面）具身仿真的开源项目，且与国内的模型/数据体系绑定
- **代价**：更名本身就是信号——**项目归属与命名在两年内变过**，长期稳定性存疑；文档与英文社区支持弱于 Isaac/ManiSkill
- **Decay risk**：high


## 四、硬件本体：选型维度而不是清单

> 硬件不能写成清单——型号一年一换，清单一年就废。**能保值的是选型维度**。下面每一类先给维度，再给 2026-09 时点的代表型号与可核对的官方数字。
>
> **所有精度数字统一口径**：厂商给的是**重复定位精度（repeatability）**，测法通常引 ISO 9283 / GB/T 12642。**绝对定位精度（accuracy）厂商几乎从不公开**，实测常在 0.5–2 mm 量级 (evidence: [T06-S006, T06-S048, T06-S089])。

### 45. 通用选型维度（八条，按决策顺序）

1. **自由度与构型**：6 轴够不够？需要 7 轴的零空间（避障 / 保持工具姿态）吗？双臂还是单臂 + 变位机？
2. **负载与力矩余量**：**标称负载要减去夹爪、相机、线缆、工装的重量**，且力臂越长有效负载越低。实践里「10 kg 臂实际能搬 5 kg」是常态。
3. **重复定位精度 vs 你真正需要的精度**：见上文口径说明。**视觉引导 = 吃绝对精度**。
4. **是否可反驱（backdrivable）+ 有没有关节力矩传感**：这一条决定你能不能做真正的阻抗/导纳控制。Franka FR3 七轴全有力矩传感器是它在研究界流行的根本原因；多数工业臂不可反驱、只能靠外置六维力传感器做力控 (evidence: [T02-S110, T02-S113])
5. **接口开放度（最容易踩坑的一条）**：
   - 有没有**开放的实时接口**（1 kHz 力矩/位置流）？还是只有「发个位姿等它走完」的高层 API？
   - 有没有官方 ROS 2 驱动？UR 与 Franka 都有官方维护的 ROS 2 驱动，这直接省掉数周工作 (evidence: [T02-S137, T02-S138])
   - **SDK 是否分级**：宇树等厂商的底层 DDS 接口与高层 SDK 是分开的，能拿到哪一层直接决定你能做什么 (evidence: [T02-S097, T02-S098])
6. **安全等级与认证**：协作场景要看 **ISO 10218-1/-2:2025**（2025 年大改版，原 ISO/TS 15066 的协作内容被并入）与 **ISO 13849-1:2023 的 PL 等级**；AMR 走 **ISO 3691-4 / R15.08** (evidence: [T06-S002, T06-S003, T06-S026, T06-S008, T06-S010])。AUBO 官方标注其产品符合 **EN ISO 13849-1:2015 (PL=d, CAT 3)** 并具备 CE / NRTL / KCs / CR 认证 (evidence: [T02-S105])——**这类标注要逐型号核对，不能按品牌一概而论**
7. **售后与备件（国内交付的真实决定项）**：换一个关节模组要等几天？有没有本地工程师？**这一条经常比参数更决定项目成败**
8. **单价区间**：见下文各类的具体数字与来源

### 46. 协作臂（cobot）

| 型号 | 负载 | 臂展 | **重复定位精度** | 力矩传感 | 关键接口 |
|---|---|---|---|---|---|
| Franka Research 3 | 3 kg | 855 mm | **±0.1 mm** | **7 轴全有** | 1 kHz 低层力矩接口，官方 franka_ros2 (evidence: [T02-S110, T02-S138]) |
| AUBO iS7 / i5 | 7 kg / 5 kg | 886.5 mm | **±0.02 mm** | 无（碰撞检测 10 级） | EN ISO 13849-1 PL=d CAT 3 (evidence: [T02-S105]) |
| AUBO iS35 | 35 kg | 2100 mm | **±0.05 mm** | 无 | 同上 (evidence: [T02-S105]) |
| UR e 系列 | 3–30 kg | 500–1300 mm | 厂商按型号标 repeatability | 无（可外挂 F/T） | 官方 ROS 2 驱动 (evidence: [T02-S109, T02-S137]) |
| 节卡 JAKA / 越疆 Dobot CR / 珞石 ROKAE xMate | 3–30 kg | 按型号 | 官方页按型号标 | ROKAE xMate 主打柔性/力控 | (evidence: [T02-S104, T02-S107, T02-S108]) |

- **选型分界**：
  - **研究 / 需要真力控** → Franka FR3（力矩传感 + 1 kHz 接口，代价是**只有 3 kg 负载**且是研究定位产品）
  - **产线上要精度与稳定** → AUBO / UR / JAKA 这类高重复精度但不可反驱的臂 + **外置六维力传感器**（ATI 系）做力控 (evidence: [T02-S113])
  - **国内交付** → 国产臂在**价格、交期、售后响应**上优势明显，且不受出口管制影响；代价是**海外文档与社区生态弱**，遇到疑难要靠厂商 FAE 而不是搜索
- **不该做的事**：拿「±0.02 mm」去承诺一个视觉引导装配的精度指标

### 47. 工业臂（发那科 / ABB / 库卡 / 安川 / 埃斯顿 / 埃夫特 / 新松）

- **维度差异**：工业臂的核心不是算法友好度，而是**节拍、刚性、寿命、防护等级、以及一整套已被验证的工艺包**（焊接、喷涂、码垛）
- **接口现实**：四大家的控制器是**闭源实时系统**，对外通常只给以太网/现场总线的位姿指令与 IO。**你拿不到 1 kHz 力矩接口**，所以「在工业臂上做学习型力控」这件事在多数情况下不成立——除非用厂商的专用选件或换控制器
- **国产侧**：埃斯顿（自研伺服 + 本体）、埃夫特、新松是主要玩家 (evidence: [T02-S122, T02-S123])；**埃斯顿官网在本轨的检测中从本机不可达（重定向循环），其参数未从一手确认，此处不给具体数字**
- **不该做的事**：为了「能跑 ROS」而在工业产线上选研究型臂——寿命、防护、售后全不达标

### 48. 人形

| 型号 | 官方公开数据 | 来源 |
|---|---|---|
| Unitree G1 | **23 DOF**（EDU 版 23–43 DOF）、整机约 **35 kg**、折叠尺寸 1320×450×200 mm、膝关节峰值力矩 **90 N·m**（EDU 版 **120 N·m**）、13 串锂电 9000 mAh、续航约 **2 小时**、**售价 US$13.5K**（不含税与运费；EDU 版询价） | (evidence: [T02-S095]) |
| Unitree H1 / 智元远征 / 傅利叶 GRx / 优必选 Walker / 星动纪元 / 逐际动力 | 各家官网有产品页，**多数不公开完整关节参数与价格** | (evidence: [T02-S100, T02-S128, T02-S129, T02-S126, T02-S125, T02-S127]) |
| Figure / 1X | **不公开销售、不公开完整规格**，只有官方视频与博客 | — |

- **诚实边界**：**人形这一格的参数透明度是全行业最低的**。除宇树公开挂价外，多数厂商的负载、连续工作时间、重复定位精度、MTBF 都**未公开**。任何声称「某人形负载 X kg、精度 Y mm」的说法，先问出处
- **开发接口**：宇树提供 `unitree_sdk2`（BSD-3，DDS 底层）、`unitree_ros2` 桥接、以及官方 RL 训练与 sim2real 部署示例 `unitree_rl_gym`（star 3,527，2026-09-02 查）——**这套开放度是它成为国际开源栈默认目标本体的直接原因** (evidence: [T02-S097, T02-S098, T02-S099, T05-S051])
- **国内开源公版**：**OpenLoong / 青龙**（上海国地共建人形创新中心，`openloong-dyn-control` star 359）与**智元 AgiBot X1**（`agibot_x1_train` star 1,698 + 开源硬件图纸）是两条可以照着做的公开路线 (evidence: [T02-S102, T02-S103, T02-S101, T02-S140, T05-S050])
- **不该做的事**：把「人形本体买回来」当成项目的起点——**买回来之后要解决的是标定、安全围栏、数据采集流程、以及谁来修**

### 49. 四足

- **Unitree Go2 / B2**：Go2 是消费级到教育级的价格带，B2 面向工业巡检；官方产品页给规格分层（不同版本的算力与接口不同）(evidence: [T02-S096])
- **ANYbotics ANYmal**：工业巡检定位，主打 IP 防护、自主充电、与工厂系统集成；**价格与生态是企业级**，不对个人销售 (evidence: [T02-S116])
- **Boston Dynamics Spot**：SDK 文档公开且质量高，但**开放的是应用层 API，不是关节力矩层**——你能写巡检任务，不能替换它的运动控制器 (evidence: [T02-S117, T02-S118])
- **选型分界**：做**运动控制研究** → 宇树（便宜 + 底层可控）；做**工业巡检交付** → ANYmal / Spot（认证、防护、售后成体系）；**别指望用研究平台去交付巡检项目**

### 50. 夹爪与灵巧手

- **两指自适应夹爪**：Robotiq 2F-85 / 2F-140 是研究与轻工业的默认件（很多数据集就是拿它采的，例如 DROID 的 18 台 Franka 全配 2F-85）(evidence: [T02-S111, T05-S033])；SCHUNK 覆盖工业侧的气动/电动夹爪与快换 (evidence: [T02-S112])
- **灵巧手**：Shadow Dexterous Hand 是研究界的高自由度标杆（**价格在数万至十万美元量级**，是研究预算而非产品预算）(evidence: [T02-S114])；国产侧因时（Inspire）等把多指手压到了显著更低的价格带 (evidence: [T02-S115])
- **最被低估的一条工程事实**：**在真实项目里，夹爪与工装（fixture）的成本远低于算法投入，但对成功率的影响常常更大**。一个为零件形状定制的夹爪或一个简单的定位工装，能把「需要毫米级视觉伺服」的问题变成「重复定位精度就够了」的问题。**先改机械，再改算法**，是这一行的老工程师最常给的建议

### 51. 力/力矩传感器

- **六维力传感器**：ATI 是工业与研究的基准品牌，产品线覆盖不同量程与过载保护 (evidence: [T02-S113])；国内有宇立（SRI）等替代，**本轨未能从本机访问到其官网，参数未一手确认**
- **选型维度**：量程（**要按最坏冲击算，不是按静态负载**）、过载保护倍数、串扰、温漂、采样率与接口（EtherCAT / CAN / 模拟）、**是否需要过安全认证**
- **关节内力矩传感 vs 腕部外置**：关节力矩（Franka 式）能做全身柔顺与碰撞检测；腕部六维力精度更高但**只能感知末端**，机器人自身与环境的碰撞感知不到

### 52. 关节模组、减速器与伺服（国产供应链的关键格）

- **谐波减速器**：Harmonic Drive（日本，行业基准，规格页给背隙/传动精度口径）与国产**绿的谐波** (evidence: [T02-S119, T02-S121])
- **RV / 摆线减速器**：Nabtesco 是重载工业臂的主流选择 (evidence: [T02-S120])
- **一体化关节模组**：零差云控（ZeroErr）等把「电机 + 减速器 + 编码器 + 驱动器 + 通信」打包，**降低了自研本体的门槛**，是这两年人形创业公司大量采用的路径 (evidence: [T02-S124])
- **伺服与控制器**：汇川（Inovance）是国产伺服/驱动的主要供应商之一 (evidence: [T02-S106])
- **选型维度**：额定与峰值力矩、**背隙（回差）**、传动精度、允许径向/轴向载荷、寿命曲线（L10）、编码器分辨率与是否**双编码器**（输出端也有编码器才能真正闭环补偿柔性）、通信协议（EtherCAT/CANopen 的 CiA 402）(evidence: [T06-S071])
- **不该做的事**：只看额定力矩不看**背隙与刚度**——人形的落地冲击与机械臂的高频往复对减速器的要求完全不同

### 53. 遥操作数据采集硬件

| 方案 | 形态 | 成本量级 | 代价 |
|---|---|---|---|
| **ALOHA / Mobile ALOHA** | 主从双臂（leader-follower），带移动底盘版本 | 官方公开了完整硬件清单与 BOM | 采集质量高但**要两套臂**；空间与预算门槛 (evidence: [T02-S087, T02-S088]) |
| **GELLO** | 低成本关节映射主手（3D 打印 + 编码器） | 千元人民币级 | 只提供关节映射，**没有力反馈**；精度受编码器与打印件限制 (evidence: [T02-S089]) |
| **SO-100 / SO-101** | 整套低成本臂（既是主手也是从臂） | 千元人民币级 | 舵机级精度，**不能作为产品原型** (evidence: [T02-S086]) |
| **VR 手柄（Quest 系）** | 末端位姿映射 | 已有设备即可 | **末端映射会丢失冗余臂的构型信息**；DROID 就是这条路线 (evidence: [T05-S033]) |
| **动捕手套 / 外骨骼** | 手部关节直采 | 数万元起 | 标定复杂、**人手到机器人手的形态差**是根本困难 |
| **越疆 X-Trainer** | 商业化的双臂遥操作采集设备 | 厂商询价 | 国内可采购的成品方案 (evidence: [T02-S107]) |

- **口径提醒**：采集方式直接决定数据里有什么。**VR 手柄采的数据没有关节冗余信息，主从臂采的数据有；两者都没有力**——所以「用这批数据训力控」从一开始就不成立 (evidence: [T02-S087, T05-S033])


## 五、选型决策树

> 用法：从根节点往下走，每层只回答一个问题。**节点 8 个**。每个叶子给「推荐 / 不推荐 / 代价」，不给「都可以」。

### 根节点：这件事的终点是论文，还是一台要交给别人用的机器？

这是本行最大的分水岭，比「机械臂还是足式」更前置。**两条路的工具栈只有约 40% 重合**。

---

### 节点 1 — 研究复现 / 算法迭代

**推荐主栈**：MuJoCo（单机快迭代）+ robosuite 或 ManiSkill（标准环境）+ robomimic / Diffusion Policy（基线）+ Rerun（看数据）+ LeRobot（如果做真机模仿学习）
**不推荐**：Isaac Sim（启动开销 > 迭代收益）、Drake（学习曲线换不来论文产出速度）、ROS 2（除非要上真机）
**代价**：这套栈里的成功率数字**不能外推到真机**——这正是它便宜的原因 (evidence: [T05-S055, T02-S028, T02-S044, T02-S078])

#### 节点 1a — 但你要做的是足式 / 全身运动控制
→ **换栈**：Isaac Lab（v2.3.x 稳定线）+ RSL-RL + 域随机化 + 真机部署脚本。这条路线已经有大量公开的 sim-to-real 成功案例，是**目前唯一被反复验证的足式训练路径** (evidence: [T02-S033, T02-S080, T02-S099])
→ **不要**用 MuJoCo 单机训四足然后期待直接上真机——并行规模不够，域随机化覆盖不足
→ **注意 2026 年的断层**：Isaac Lab 3.0 换了物理后端，**pin 在 2.3.x 上直到出现第三方复现报告** (evidence: [T02-S033, T02-S051])

---

### 节点 2 — 产品交付 / 要给客户用

#### 节点 2a — 机械臂操作，且**没有**接触力控需求（取放、上下料、视觉分拣）
→ **推荐**：厂商本体 + 厂商控制器 + ROS 2 只做上位机 + MoveIt 2 仅用于换型与避障 + 相机 + 手眼标定 SOP
→ **真正的工作量在**：标定与复标流程、异常恢复、节拍优化、工装设计
→ **不推荐**：把规划器放进节拍关键路径（采样式规划每次路径不同，工艺工程师不接受）(evidence: [T02-S015, T02-S061])
→ **省钱的顺序**：先想能不能用**工装**把问题变简单，再想算法 (evidence: [T02-S111])

#### 节点 2b — 机械臂操作，**有**接触力控需求（装配、打磨、插拔、擦拭）
→ **两条互斥的路**：
  - **路 A：本体自带关节力矩传感** → Franka FR3 类（7 轴力矩 + 1 kHz 接口）。代价：**负载只有 3 kg**，且是研究定位产品，产线寿命与售后要自己评估 (evidence: [T02-S110])
  - **路 B：工业臂 + 腕部六维力传感器** → 精度更高、负载更大、能进产线；代价：**只感知末端**，机器人身体与环境碰撞感知不到，且要自己写导纳/阻抗控制环 (evidence: [T02-S113])
→ **仿真侧**：**别用 MuJoCo 的接触结果去论证装配可行性**——软约束接触会系统性低估刚性冲击。要么用 Drake 的水弹性接触，要么直接上真机做 (evidence: [T02-S029, T02-S027])
→ **控制环**：ros2_control + PREEMPT_RT + EtherCAT/CANopen；QP 用 OSQP 或 ProxQP，**必须实测最坏情况求解时间** (evidence: [T02-S004, T02-S023, T02-S024, T06-S072])

#### 节点 2c — 足式移动（巡检、勘察）
→ **交付级**：ANYmal / Spot——认证、IP 防护、自主充电、售后成体系；代价是**只开放应用层 API**，运动控制器不可替换 (evidence: [T02-S116, T02-S118])
→ **研究/低成本**：宇树 Go2 / B2 + `unitree_sdk2` 底层接口；代价是**你要自己承担可靠性与安全** (evidence: [T02-S096, T02-S097])
→ **导航**：崎岖地形不要直接套 Nav2 的 2D 代价地图，需要高程图 + 足端可通行性 (evidence: [T02-S131])

#### 节点 2d — 移动操作（底盘 + 臂）
→ **这是最难的一格**，因为误差是**串联累积**的：底盘定位误差（厘米级）+ 臂的绝对精度误差（毫米级）
→ **推荐做法**：**不要指望一次到位**——底盘粗定位 + 到位后用视觉做**局部闭环**（视觉伺服或重新标定），把底盘误差从误差链里摘出去
→ **栈**：Nav2（移动）+ MoveIt 2（操作）+ 一套统一的 TF 与时间同步（PTP / 硬件触发）(evidence: [T02-S132, T02-S015, T06-S010])

---

### 节点 3 — 数据从哪来？（决定你的学习栈）

#### 节点 3a — 遥操作真机采集
→ **栈**：ALOHA / GELLO / SO-101 / VR 手柄 → LeRobot 数据格式 → robomimic / Diffusion Policy / openpi 微调 (evidence: [T02-S087, T02-S089, T02-S086, T02-S073, T02-S075])
→ **代价**：**人力是主要成本**，且采集协议（相机位姿、标定、任务定义）的一致性决定数据能不能用。DROID 用 18 台完全相同的 Franka + 统一 ZED 相机配置，正是为了消除这个变量 (evidence: [T05-S033])
→ **先问一句**：你的任务需要力吗？**需要的话，主流遥操作方案采不到力**，这条路从一开始就不通

#### 节点 3b — 仿真生成
→ **操作任务**：ManiSkill 3 / robosuite / RoboCasa；**长程家务与物体状态变化**：OmniGibson / BEHAVIOR-1K；**足式**：Isaac Lab (evidence: [T02-S049, T05-S043])
→ **代价**：sim-to-real 差距在接触密集任务上仍然巨大；**仿真涨 10 个点不能推出真机更好**，这是本行最常见的过度解读 (evidence: [T05-S055])

#### 节点 3c — 混合（公开数据集预训练 + 自采后训练）
→ **先查许可证**：Open X-Embodiment 是 **CC BY 4.0（可商用）**；**AgiBot World 是 CC BY-NC-SA 4.0（不可商用 + 传染）** (evidence: [T05-S035, T05-S034])
→ **格式**：跨数据集混训的事实标准是 **RLDS**（Google Research），OXE 就是统一到这个格式发布的 (evidence: [T02-S079, T05-S035])
→ **代价**：OXE 的本体分布极度偏斜（Franka Panda / WidowX 桌面单臂占压倒性比例），**移动操作、人形、力控样本稀少**——如果你的本体不在分布里，预训练的收益要重新评估 (evidence: [T05-S035])

---

### 节点 4 — 必须过安全认证吗？

→ **是（要卖给工厂 / 要有人在旁边）**：从第一天就按 **ISO 12100 风险评估 → ISO 10218-1/-2:2025（2025 大改版）→ ISO 13849-1:2023 的 PL 等级**来设计，选本体时逐型号核对认证而不是按品牌 (evidence: [T06-S007, T06-S002, T06-S003, T06-S008, T06-S026])
→ **AMR / 移动机器人**：走 **ISO 3691-4:2023** 与 **ANSI/RIA R15.08** (evidence: [T06-S010, T06-S028])
→ **代价**：安全相关的部分**不能用「学习出来的策略」直接承担**——安全功能要走独立的、可认证的通道（STO、安全 IO、安全 PLC）。你的神经网络在功能安全体系里目前拿不到 PL d/e (evidence: [T06-S008, T06-S018])
→ **否（实验室 / 内部演示）**：以上全部可以后置，但**不要在方案书里承诺一个你没做过认证的等级**

---

### 节点 5 — 是否国内交付？（供应链与合规是不同的问题）

→ **是**：
  - **本体与零部件**：国产协作臂（节卡 / 遨博 / 越疆 / 珞石）+ 国产减速器（绿的谐波）+ 国产伺服（汇川）+ 国产一体化关节（零差云控）——**交期与售后是决定性优势** (evidence: [T02-S104, T02-S105, T02-S107, T02-S108, T02-S121, T02-S106, T02-S124])
  - **数据与模型**：AgiBot World（注意 **NC 许可**）、RoboMIND、OpenLoong 公版机 (evidence: [T05-S034, T05-S038, T05-S050])
  - **合规**：数据不能出内网时，**Foxglove 这类云平台直接出局**，用 Rerun + rosbag2 自建 (evidence: [T02-S091, T02-S090])
  - **算力**：Isaac 全栈强绑 NVIDIA，**要评估显卡供应与替代路径**
→ **否**：上面这些约束大部分不存在，但**国产本体的海外文档与社区支持弱**是反向代价


## 六、避坑清单

> 12 条。每条的格式是：**错在哪 → 后果是什么 → 正确做法**。

1. **❌ 用重复定位精度冒充绝对定位精度**
   → 「这台臂精度 0.02 mm」是本行第一号外行破绽。**ISO 9283 把两者严格分开**：重复性是多次实到位姿的离散度，准确度是指令位姿与实到均值之差，后者通常差一到两个数量级。
   → 后果：视觉引导装配的方案按 0.02 mm 报价，现场做出来是毫米级偏差，整个工艺窗口不成立。
   → 正确：只要有「相机告诉机器人去哪」，就按**绝对精度**做预算，并把机器人标定 + 手眼标定 + 定期复标写进 SOP (evidence: [T06-S006, T06-S089, T02-S060])

2. **❌ 以为 ROS 2 自带实时性**
   → ROS 2 让你**能够**构建实时系统，但默认发行版跑在通用 Linux 上，抖动毫秒级正常。
   → 后果：1 kHz 力控环写在 ROS 2 节点里，现场偶发抖动、力超调、撞件。
   → 正确：实时环放 PREEMPT_RT 隔核进程或 MCU，用 EtherCAT / CANopen 下行；ROS 2 只当上位机。**并且要测最坏抖动（max / p99.9），不是平均** (evidence: [T06-S072, T06-S070, T02-S008])

3. **❌ 拿 PyBullet 的结果当 sim-to-real 依据**
   → Bullet3 主仓最后 push 是 **2025-10-22**，维护实质停滞；它的接触求解在刚性接触下抖动/穿模，摩擦模型简化。
   → 后果：2019–2022 年建立在它之上的一批 sim-to-real 结论今天不能直接外推，而新手仍在照着老教程复现。
   → 正确：新项目用 MuJoCo（学术）或 Isaac Lab（并行）；需要接触保真度就用 Drake 或直接上真机 (evidence: [T02-S045, T02-S028, T02-S027])

4. **❌ 把仿真里的成功率当真机预期**
   → 「仿真涨 10 个点」和「真机更好」之间没有可靠的传递关系，接触密集任务尤其如此。而且**不同仿真平台的分数互相不可比**（引擎、控制频率、成功判定都不同）。
   → 后果：立项时按仿真成功率承诺交付指标，真机上差几十个点。
   → 正确：仿真只用来做**相对比较与消融**；任何对外承诺的数字必须来自真机，且要写清分母（多少次试验、什么初始分布、算不算人工干预）(evidence: [T05-S055, T05-S041])

5. **❌ 用 GPL-3.0 的 SLAM 实现做闭源产品**
   → ORB-SLAM3、VINS-Fusion、OpenVINS **全是 GPL-3.0**。链接进闭源程序会触发传染。
   → 后果：产品都交付了才发现法务问题，返工成本极高——这是国内交付里最晚被发现的雷之一。
   → 正确：它们只用于基线评估；产品线用 BSD 的 GTSAM 自建后端，或买商业 VIO (evidence: [T02-S056, T02-S057, T02-S058, T02-S059])

6. **❌ 用 NC（非商用）许可的数据集或模型做商业产品**
   → **AgiBot World 是 CC BY-NC-SA 4.0**——不可商用，且衍生物要同样开放。**FoundationPose 的许可证明文写着「non-commercially… research or evaluation purposes only」**。
   → 后果：模型权重是「用不能商用的数据训的」，整个产品的知识产权链是脏的。
   → 正确：训练前先过一遍数据与模型的许可证清单；商用路线优先 CC BY 4.0 的 OXE、Apache-2.0 的 SAM 2 (evidence: [T05-S034, T02-S063, T05-S035, T02-S139])

7. **❌ 照着老教程起在已经死掉的东西上**
   → 四个高频例子：**Gazebo Classic**（已停止支持）、**Isaac Gym Preview / IsaacGymEnvs**（已被 Isaac Lab 取代）、**Kilted Kaiju**（2026-12 EOL）、**PyBullet**（维护停滞）。
   → 后果：环境装不上、没人能答疑、半年后要整体重写。
   → 正确：起项目前先查**三件事**——最后一次 commit、最近一个 release、以及官方有没有 EOL 公告 (evidence: [T02-S039, T02-S036, T02-S001, T02-S045])

8. **❌ 忽略夹爪与工装比算法便宜**
   → 在真实项目里，一个为零件定制的夹爪或一个简单的定位工装，能把「需要毫米级视觉伺服」变成「重复定位精度就够了」。
   → 后果：把六个月投进感知与策略，最后被一个两周做出来的工装解决。
   → 正确：**先改机械，再改算法**。方案评审时强制回答一句「这个问题能不能用工装消掉？」(evidence: [T02-S111, T02-S112])

9. **❌ 把「star 数高」当成「可以用在生产上」**
   → Genesis star 29,856（本文件里仿真器第一），但 2024-12 才发布、公开的 sim-to-real 案例稀少；反过来 **rmw_zenoh 只有 496 star 却是 ROS 2 官方 tier-1 中间件**；ros2_control 只有 990 star 却是每台真机都要过的一层。
   → 后果：选型会上用 star 数说服人，交付时发现没人踩过你要踩的坑。
   → 正确：看**最后一次 release 的日期、issue 的响应速度、有没有第三方生产案例**，star 数最多算注意力信号 (evidence: [T02-S041, T02-S133, T02-S004])

10. **❌ 把 MJX / MuJoCo Warp 当成「MuJoCo 的 GPU 版，功能一样」**
    → **MJX 的功能是 MuJoCo 的子集**，官方专门列了差异表——不支持全部约束类型、传感器与碰撞几何组合。MuJoCo Warp 是另一条并行路线，两者长期重叠。
    → 后果：模型直接搬过去跑不动，或者能跑但行为不同，调了两周才发现是引擎差异。
    → 正确：迁移前先对着官方差异表核一遍模型用到的特性 (evidence: [T02-S031, T02-S030])

11. **❌ 用「协作机器人」这个词代替风险评估**
    → 买了协作臂不等于可以拆掉围栏。**是否安全取决于应用（速度、负载、末端形状、接触部位），不取决于机器人型号**。ISO 10218:2025 大改版后，原 ISO/TS 15066 的协作内容被并入正文。
    → 后果：现场审核过不了，或者出了伤人事故没有可辩护的文档链。
    → 正确：按 ISO 12100 做应用级风险评估，力/压强限值按具体接触部位查表，安全功能走独立可认证通道（STO / 安全 IO），**不要让神经网络承担安全功能** (evidence: [T06-S007, T06-S002, T06-S026, T06-S008])

12. **❌ 报「采了 X 万条轨迹」而不报口径**
    → 不同数据集的「一条轨迹」不是同一个东西。DROID 平均约 16.6 秒/条，AgiBot World Beta 平均约 10.7 秒/条；BridgeData V2 的 60,096 条里有 9,731 条是策略 rollout 不是人类演示；RoboMIND 的 10.7 万条里约 28% 是仿真。
    → 后果：按轨迹数横向比较数据集规模，得出完全错误的结论。
    → 正确：看到轨迹数先问三件事——**平均多长、谁采的、真机还是仿真** (evidence: [T05-S033, T05-S034, T05-S036, T05-S038])


## 七、Phase 2 接口

### 三层清单（一句话理由）

**必备（11）**
| 工具 | 一句话理由 |
|---|---|
| ROS 2 | 不是最好的技术，是唯一能让别人接手你项目的底座 |
| ros2_control | 只要你驱动真机，这一层绕不过去 |
| MuJoCo（+MJX/MJWarp） | 学术接触仿真的事实标准，Apache-2.0 是它爆发的直接原因 |
| Isaac Sim + Isaac Lab | 足式与大规模并行 RL 目前唯一被反复验证的路径 |
| Gazebo（Jetty） | 系统级仿真（传感器、多机、世界）的默认件，LTS 到 2031 |
| MoveIt 2 | 机械臂规划的集成层；产线上只在换型与避障工位用 |
| Pinocchio | 所有现代控制/优化库的地基，你可能没直接用但一定在依赖 |
| OpenCV | 标定与图像处理的地板；2026 年是 5.0/4.x 双线并行 |
| LeRobot | 把数据格式的碎片化收敛掉了，是模仿学习的入口 |
| Rerun | 调机器人 80% 时间在对齐数据流，它就是干这个的 |
| rosbag2 + MCAP + PlotJuggler | 出了事故只有这三样能救你 |

**场景特化（24）**：Drake、Genesis、ManiSkill 3+SAPIEN、robosuite、Webots、CoppeliaSim、PyBullet（仅复现）、OMPL、Crocoddyl、OCS2、TOPP-RA、QP 三选一（OSQP/ProxQP/qpOASES）、Nav2、GTSAM、SLAM 三件套（ORB-SLAM3/VINS-Fusion/OpenVINS）、Open3D/PCL、Kalibr/easy_handeye2、FoundationPose/MegaPose/SAM 2、robomimic+Diffusion Policy、RL 库四选一（RSL-RL/skrl/SB3/RLlib）、实时与总线链路（micro-ROS/PREEMPT_RT/SOEM/IgH/CANopen）、Isaac ROS、Foxglove、传感器栈（RealSense/ZED/Ouster/Livox）

**新兴（9，`stability: experimental`）**：MuJoCo Warp、Newton、Isaac Lab 3.0 beta、Genesis、openpi、Isaac GR00T N1.x、rmw_zenoh、SO-101+LeRobot 硬件生态、InternUtopia

### 选型决策树摘要（8 节点）

1. **根**：终点是论文还是交付？（两条路的工具栈只约 40% 重合）
2. **研究复现** → MuJoCo + robosuite/ManiSkill + robomimic；**足式研究** → Isaac Lab 2.3.x + RSL-RL
3. **交付·机械臂无力控** → 厂商本体 + ROS 2 只当上位机；工作量在标定与异常恢复，不在规划器
4. **交付·机械臂有力控** → 路 A 关节力矩本体（FR3，3 kg 上限）／路 B 工业臂 + 腕部六维力（只感知末端）
5. **交付·足式** → ANYmal/Spot（认证成体系，只开放应用层）／宇树（底层可控，可靠性自负）
6. **交付·移动操作** → 误差串联累积；底盘粗定位 + 到位后视觉局部闭环，别指望一次到位
7. **数据来源** → 遥操作（采不到力）／仿真（分数不可外推）／混合（先查许可证：OXE 可商用，AgiBot World 不可）
8. **合规两问** → 要不要过安全认证（ISO 12100 → 10218:2025 → 13849-1 PL）；是不是国内交付（供应链 + 数据不出内网）

### 避坑清单（12 条，见正文第六节）

重复定位 vs 绝对精度混淆／以为 ROS 2 自带实时／拿 PyBullet 当 sim-to-real 依据／把仿真成功率当真机预期／GPL-3.0 SLAM 进闭源产品／NC 许可数据训商用模型／起在已死的东西上（Gazebo Classic、Isaac Gym、Kilted、PyBullet）／忽略夹爪与工装比算法便宜／把 star 数当生产可用性／把 MJX 当 MuJoCo 的等价 GPU 版／用「协作机器人」代替风险评估／报轨迹数不报口径

### 近 12 个月工具栈的真实变化（带日期）

| 日期 | 变化 | 影响 |
|---|---|---|
| 2025-07-11 | **SOEM v2.0.0** 发布，距上一版 1.4.0（2019-07）六年 | 用户态 EtherCAT 主站重新有人维护 |
| 2025-09 | **Gazebo Jetty** 发布，LTS 至 2031-05 | 新项目的 Gazebo 版本选择答案变了 (evidence: [T02-S037]) |
| 2025-10-22 | **Bullet3 最后一次 push** | PyBullet 事实上进入停滞，老教程失效 (evidence: [T02-S045]) |
| 2025 年内 | **RealSense 从 Intel 独立**，GitHub 组织迁至 `realsenseai` | 传感器供应链的长期稳定性要重新评估 (evidence: [T02-S068, T02-S069]) |
| 2025 年内 | **Zenoh 进入 ROS 2 tier-1 中间件** | DDS 十年垄断被打破，多机/弱网场景有了官方选项 (evidence: [T02-S141]) |
| 2025-03-17 | **MuJoCo Warp** 仓库创建 | DeepMind 的 GPU 第二条路线，MJX 地位存疑 (evidence: [T02-S030]) |
| 2026-03-09 → 2026-08-03 | **LeRobot 从 v0.5.0 到 v0.6.1**，半年三个次版本 | 接口仍在破坏性变化，产品化必须 fork 冻结 (evidence: [T02-S073]) |
| 2026-03 / 2026-07-02 | **Isaac Lab 3.0-beta / beta2.patch1**，引入 Newton 后端与 kit-less 工作流 | 架构级重写，2.x 环境代码不保证平移 (evidence: [T02-S033]) |
| 2026-04-13 / 2026-07-07 | **Pinocchio 4.0.0 / 4.1.0** | 大版本 API 变化，下游控制库要跟 (evidence: [T02-S019]) |
| 2026-04-21 | **ManiSkill v3.0.1 正式脱离 beta**（b23 系列跑了两年多） | GPU 并行操作基准有了稳定版 (evidence: [T02-S042]) |
| 2026-05-22 | **ROS 2 Lyrical Luth 发布**，新 LTS 至 2031-05 | 新项目的发行版答案变了；**Kilted 2026-12 EOL** (evidence: [T02-S001]) |
| 2026-06-26 | **OpenCV 5.0.0 发布**，与 4.14.0（2026-07-19）双线并行 | 破坏性变更；机器人栈下游仍以 4.x 为准，别急着上 (evidence: [T02-S052, T02-S053]) |
| 2026-08-14 | **OMPL 2.0.2**（2.0 是大版本） | MoveIt 默认规划后端的 API 有变 (evidence: [T02-S017]) |
| 2026-08-20 | **MuJoCo 3.12.0**（月度发布节奏，含大网格碰撞检测 2 倍加速） | 单机接触仿真仍在快速改进 (evidence: [T02-S028]) |
| 2026-09-01 | **Rerun 0.37.0**（周级发布） | 可视化层迭代极快，pin 版本 (evidence: [T02-S090]) |

### 衰减速度分层（Phase 0C 刷新节奏直接用）

**一年后大概率还在、且基本没变（≥ 24 个月，刷新周期 12 个月）**
ROS 2 的核心概念与 DDS/QoS 模型、ros2_control 的架构、EtherCAT / CANopen / PREEMPT_RT 这一层、Pinocchio、OMPL、GTSAM、OSQP、Drake、MoveIt 2、OpenCV、rosbag2/MCAP、ISO 精度与安全标准的口径。
→ **这一层是最保值的知识**：十年前学的 EtherCAT 今天照样用。

**12–24 个月会有一次显著变化（刷新周期 6 个月）**
Isaac Sim / Isaac Lab 的接口、LeRobot 的 API、Rerun 的 API、Nav2 的插件体系、Open3D/PCL 的维护状态、Foxglove 的商业条款、传感器产品线（RealSense/ZED/Livox）、国产本体的型号与价格。

**半年就可能换（刷新周期 3 个月，且默认标 experimental）**
MuJoCo Warp、Newton、Isaac Lab 3.0、Genesis、openpi、Isaac GR00T、InternUtopia、SO-10x 硬件世代、以及**所有 VLA 模型的具体型号与成功率数字**。
→ **写进 skill 时必须带日期，且不要把这一层的任何数字当作基线**。

### 反复出现 ≥ 3 source 都强调的「工具选型原则」（候选 playbook 规则）

1. **先问许可证再问性能**——GPL-3.0 的 SLAM、NC 的数据集与模型，会在交付末期变成不可逆的成本 (出现于: T02-S056/S057/S058, T02-S063, T05-S034)
2. **仿真只用于相对比较，绝不用于对外承诺**——跨平台分数不可比，接触密集任务的差距尤其大 (出现于: T05-S055, T02-S029, T02-S045)
3. **先改机械，再改算法**——工装与夹爪能把毫米级问题降级成重复定位精度问题 (出现于: T02-S111, T02-S112, T02-S105)
4. **任何数字都要带口径**——精度要说是重复性还是准确度；吞吐要说引擎/步长/并行数；轨迹数要说平均时长与真机比例 (出现于: T06-S006, T05-S033, T05-S034, T02-S040)
5. **起项目前查三件事**：最后一次 commit、最近一个 release、有没有 EOL 公告 (出现于: T02-S045, T02-S039, T02-S001, T02-S036)
6. **实时性不是框架给的，是你自己证明的**——测最坏抖动而不是平均 (出现于: T06-S072, T06-S070, T02-S010)

### 显著的工具流派分裂（候选「智识谱系」条目）

1. **「模型驱动」vs「数据驱动」**
   - 模型派：Drake / Pinocchio / Crocoddyl / OCS2 / MPC + WBC。主张先把动力学与约束写清楚，再优化；可验证、可解释、样本效率高。代表人物与 Track 01 关联：Russ Tedrake（Drake + 两门在线教材）(evidence: [T05-S062, T05-S063])
   - 数据派：LeRobot / openpi / Diffusion Policy / GR00T。主张用规模化数据吃掉建模困难。
   - **分裂点不是意识形态，是任务形态**：接触与几何可建模（足式支撑相、已知零件装配）→ 模型派赢；任务多样、物体开放、难以枚举（家庭杂物整理）→ 数据派赢。
2. **「厚平台」vs「薄库」**
   - 厚平台：Isaac Sim/Lab、Omniverse、CoppeliaSim——一站式但绑生态、版本迁移痛
   - 薄库：MuJoCo、Pinocchio、OSQP、Rerun——各管一段、自己拼、迁移成本低
   - 这一行的资深人普遍偏薄库，**理由是「三年内平台一定会改架构，而库不会」**——Isaac Gym→Orbit→Isaac Lab→Isaac Lab 3.0 这条改名史是最直接的证据 (evidence: [T02-S036, T02-S033])
3. **「开源可自托管」vs「云平台」**
   - Rerun（Apache-2.0，全开源）vs Foxglove（Studio 已闭源，转商业平台）。在国内交付里这不是偏好问题，是**数据能不能出内网**的硬约束 (evidence: [T02-S090, T02-S091])

### 新兴工具信号

- 当前活跃 / 上升的新工具数：**9**（新兴层）
- **出现 → 主流的速度估计**：本行约 **18–30 个月**。锚点：MuJoCo 开源（2021-10）→ 成为论文默认约 18 个月；Isaac Gym（2021）→ Isaac Lab 成为足式默认约 30 个月；LeRobot（仓库建于 2024-01-26）→ 成为模仿学习默认入口约 18 个月 (evidence: [T02-S028, T02-S033, T02-S073])
- **反向信号**：Octo（最后 push 2024-07-31）与 OpenVLA（最后 push 2025-03-23）都曾是热门 VLA 开源实现，**如今均已停更**——这一层的半衰期比其他层都短 (evidence: [T02-S076, T02-S077])

### 冷僻 / 信号薄弱标注（Phase 2.8 诚实边界直接用）

- **不冷僻**：必备层 11 个 ✅、场景特化 20 个 ✅、新兴 9 个 ✅、source 142 条 ✅
- **但有四处真实薄弱，必须写进诚实边界**：
  1. **人形本体的参数透明度是全行业最低的**。除宇树 G1 公开挂价（US$13.5K）与部分关节力矩外，智元、傅利叶、优必选、星动纪元、逐际动力、Figure、1X 的负载、连续工作时间、重复定位精度、MTBF **全部未公开**。本文件对这一格只能写「有产品页」，不能写参数。
  2. **三家国产厂商官网从本机不可达**：**埃斯顿**（重定向循环）、**大族机器人**、**宇立 SRI 力传感器**。这三家的参数本轨**未从一手确认**，正文中已明确标注为「未公开 / 未确认」而不是引用二手数字。
  3. **成本区间的一手来源稀薄**。除宇树 G1 的官方标价外，协作臂、灵巧手、六维力传感器的价格区间几乎没有厂商公开标价（全部「联系销售」）。本文件给出的量级判断（如 Shadow Hand 数万至十万美元）是**范围性表述而非可引用的一手价格**。
  4. **仿真吞吐数字普遍不可比且缺测试条件**。Genesis 的「4300 万 FPS」是本行最典型的例子——本轨保留了这个数字但同时标注了它的口径问题，Phase 2 引用时必须连口径一起带上。
- **surrogate 比例**：manifest 中 `surrogate_primary` 主要来自厂商产品页与标准机构页。**厂商页在「参数」这一维度是一手的，但在「好不好用」这一维度是利益相关方**——从本轨提炼任何「某厂商方案更优」的判断时，必须要求至少一个非厂商来源交叉印证。

### 不进任何层的候选（21 个，供 Phase 1.5 复核）

**已死或维护停滞**：Isaac Gym Preview / IsaacGymEnvs（官方弃用）、Gazebo Classic（停止支持）、Octo（2024-07 起停更）、OpenVLA（2025-03 起停更）、Cartographer（2024-01 起停更）、Xenomai（社区活跃度落后 PREEMPT_RT）、Foxglove Studio 开源版（已归档）。
**与本行业范围外或过于外围**：openpilot（乘用车 ADAS，范围外）、ArduPilot / PX4（无人机自驾，与地面机器人栈重合少）、johnny-five / gobot（IoT 玩具级）、NiceGUI（通用 Web UI）、EasySpider（与机器人无关，仅因 topic 标签混入 seed）、Wechaty（同前）、text-to-cad（CAD agent，另一条线）。
**是清单不是工具**：awesome-robotics、Embodied-AI-Guide、cs-video-courses、awesome-multimodal-ml、ai-deadlines（已由 Track 05 收录为信息源）。
**证据不足**：若干国产仿真与数据平台只有发布公告、无可核对的仓库活跃度或许可证条款。

