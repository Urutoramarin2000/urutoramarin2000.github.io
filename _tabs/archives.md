---
layout: archives
icon: fas fa-archive
order: 2
---
### 人形机器人强化学习控制与部署
针对人形机器人在复杂环境中的运动控制问题，搭建isaacgym仿真器环境，使用强化学习算法在仿真器中进行走路policy训练，提升其稳定性和适应性。


**我的贡献**：
- 负责算法调优与仿真实验。基于Isaacgym仿真环境，使用PPO算法进行训练。
- 根据实机硬件情况，添加域随机化。
- 参与硬件部署与调试。
- 添加了速度预测网络Estimator，DreamWaQ（基于VAE的地形隐Encoder），RMA（基于Teacher-Student的特权观测Encoder）的实现与测试。
- 添加web-visualizer，在没有gui的情况下可视化训练。

**成果**：
- 成功完成sim2real，在直线电机（isaacgym只支持旋转电机）机器人平台上实现了强化学习原地踏步。

**项目链接**：[humanoid-RL](https://github.com/Urutoramarin2000/humanoid-rl)


### 双轮足强化学习控制与部署（从人形项目修改而来）
针对双轮足机器人在复杂环境中的运动控制问题，搭建isaacgym仿真器环境，使用强化学习算法在仿真器中进行运动policy训练，提升其稳定性和适应性。

**我的贡献**：
- 与人型项目相同

**成果**：
- 成功完成sim2real，在大质量双轮足机器人平台上部署了强化学习运动控制，实现坑洼路面稳定通过。

**项目链接**：[Wheeled-RL](https://github.com/Urutoramarin2000/wheeled_rl)

### 基于Quest3的机械臂VR无线遥操作与训练数据采集
基于Vuer，使用Quest3，添加了机械臂与机器人的1:1映射，使用pybullet求解ik，实现了机械臂的VR远程控制。完成了机械臂的训练数据采集pipeline。

**我的贡献**：
- 在vr环境中接入realsense相机画面
- 在vr环境中添加机器人模型，对齐遥操空间与真实空间
- 设计遥操作控制逻辑，防止机械臂危险行为
- 完成数据采集pipeline，解决数据同步问题



**项目链接**：[Quest3_teleop_record](https://github.com/Urutoramarin2000/quest3_teleop_record)


### 基于扩散模型与 3D 高斯的文本-3D 模型生成（毕业设计）：
基于 transformer 的 3d 高斯生成模型，结合 SDS 的形状优化与扩散模型的texture 优化来完成基于文本 - 高质量3D模型的生成。

**成果**：
- 结合基于tranfromer的快速3D模型生成与基于SDS的模型精细优化，完成告快速高质量3D模型生成。