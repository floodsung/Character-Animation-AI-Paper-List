# Character-Animation-AI-Paper-List
https://zhuanlan.zhihu.com/p/509528335

1 前言
角色动画Character Animation 的AI研究主要分成两块：物理动画Physics-based Animation AI 和运动学动画Kinematic-based Animation AI。物理动画AI角色需要受到虚拟世界的物理环境限制，控制方法和 控制机器人差不多，都是使用PD控制器来控制，而运动学动画AI的角色不受物理约束 ，我们可以直接赋值角色骨骼的位置，这和传统动画的控制方式是一样的。物理动画AI等价于让角色自己动，能够让角色在虚拟世界真正“活”起来，而运动学动画AI则是角色像提线木偶，是被动的动，所以物理动画AI具有明显的优越性，更具未来感，当然难度也会更大。

下面列举物理动画AI的相关研究。

2 物理动画Physics-based Animation AI
2.1 人型Humanoid
人型物理动画AI的研究往往需要兼顾拟人和任务完成，即在物理环境下完成要求任务的同时整个动作系列看起来和人真实的行为差不多。所以，这一块的研究往往将模仿学习和强化学习结合在一起。强化学习是为了在物理环境交互下完成任务，模仿学习则为了拟人。

以下按主要作者及团队分类，有些工作作者之间有合作。

2.1.1 Xue Bin (Jason) Peng

[1] ASE: Large-Scale Reusable Adversarial Skill Embeddings for Physically Simulated Characters [Siggraph 2022]

Project page


[2] AMP: Adversarial Motion Priors for Stylized Physics-Based Character Control [Siggraph 2021]

Project Page


[3] MCP: Learning Composable Hierarchical Control with Multiplicative Compositional Policies [Neurips 2019]

Project Page


[4] SFV: Reinforcement Learning of Physical Skills from Videos [Siggraph Asia 2018]

Project Page


[5] DeepMimic: Example-Guided Deep Reinforcement Learning of Physics-Based Character Skills [Siggraph 2018]

Project Page


2.1.2 Michiel van de Panne home page

[1] Discovering Diverse Athletic Jumping Strategies [Siggraph 2021]

Project Page


[2] ALLSTEPS: Curriculum-driven Learning of Stepping Stone Skills [SCA 2020]

Project Page


[3] Fast and Flexible Multilegged Locomotion Using Learned Centroidal Dynamics [Siggraph 2020]

Project Page


2.1.3 NVIDIA Toronto Artificial Intelligence Lab

[1] UniCon: Universal Neural Controller For Physics-based Character Motion [Siggraph 2020]


[2] Physics-based Human Motion Estimation and Synthesis from Videos [ICCV 2021]


2.1.4 Jehee Lee https://mrl.snu.ac.kr/~jehee/

[1] Human Dynamics from Monocular Video with Dynamic Camera Movements [SIGGRAPH Asia 2021]Link


[2] Learning a family of motor skills from a single motion clip [SIGGRAPH 2021] Link


[3] Learning Time-Critical Responses for Interactive Character Control [SIGGRAPH 2021] Link


[4] Learning Predict-and-Simulate Policies From Unorganized Human Motion Data [SIGGRAPH Asia 2019].Link


2.1.5 Daniel Holden /Ubisoft

[1] SuperTrack – Motion Tracking for Physically Simulated Characters using Supervised Learning [Siggraph 2021]


[2] DReCon: Data-Driven responsive Control of Physics-Based Characters[Siggraph Asia 2019]


2.1.6 DeepMind

[1] Imitate and Repurpose:Learning Reusable Robot Movement Skills From Human and Animal Behaviors


2.1.7 Karen Liu

[1]Learning to Manipulate Amorphous Materials[Siggraph 2020]


[2] Learning To Dress: Synthesizing Human Dressing Motion via Deep Reinforcement Learning [Siggraph Asia 2018]


2.1.8 Jessica K. Hodgins

[1] Control Strategies for Physically Simulated Characters Performing Two-player Competitive Sports [Siggraph 2021]


[2] Learning Basketball Dribbling Skills Using Trajectory Optimization and Deep Reinforcement Learning [Siggraph 2018]


2.2 多足Legged Robot
多足角色和机器人更紧密相关，特别很多多足sim2real的工作，在real就是机器人控制，在sim就是物理动画，因此我们这里列举多足机器人的相关工作。

2.2.1 ETH Anymal Team

[1] Advanced Skills through Multiple Adversarial Motion Priors in Reinforcement Learning


[2] Rudin N, Hoeller D, Reist P, et al. Learning to walk in minutes using massively parallel deep reinforcement learning[C]//Conference on Robot Learning. PMLR, 2022: 91-100


[3] Miki T, Lee J, Hwangbo J, et al. Learning robust perceptive locomotion for quadrupedal robots in the wild[J]. Science Robotics, 2022, 7(62): eabk2822.


[4] Lee J, Hwangbo J, Wellhausen L, et al. Learning quadrupedal locomotion over challenging terrain[J]. Science robotics, 2020, 5(47): eabc5986.


[5] Hwangbo J, Lee J, Dosovitskiy A, et al. Learning agile and dynamic motor skills for legged robots[J]. Science Robotics, 2019, 4(26): eaau5872.


[6] Robust Recovery Controller for a Quadrupedal Robot using Deep Reinforcement Learning


2.2.2 Cassie

[1] Xie Z, Berseth G, Clary P, et al. Feedback control for cassie with deep reinforcement learning[C]//2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, 2018: 1241-1246. [PDF] arxiv.org


[2] Xie Z, Clary P, Dao J, et al. Learning locomotion skills for cassie: Iterative design and sim-to-real[C]//Conference on Robot Learning. PMLR, 2020: 317-329


[3] Li Z, Cheng X, Peng X B, et al. Reinforcement learning for robust parameterized locomotion control of bipedal robots[C]//2021 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2021: 2811-2817


[4] Cassie Learning Dodging Skills: A Hierarchical Reinforcement Learning Based Approach


[5] Sim-to-Real Learning of All Common Bipedal Gaits via Periodic Reward Composition


2.2.3 Other Legged Robot Related

[1] Towards Real Robot Learning in the Wild: A Case Study in Bipedal Locomotion


[2] Learning Agile Robotic Locomotion Skills by Imitating Animals Paper


[3] Legged Robots that Keep on Learning: Fine-Tuning Locomotion Policies in the Real World Paper


[4] Model-based Motion Imitation for Agile, Diverse and Generalizable Quadupedal Locomotion


[5] Imitate and Repurpose:Learning Reusable Robot Movement Skills From Human and Animal Behaviors


[6] RMA: rapid motor adaptation for legged robots


[7] Concurrent Training of a Control Policy and a State Estimator for Dynamic and Robust Legged Locomotion



[8] Adversarial Motion Priors Make Good Substitutes for Complex Reward Functions


[9] Minimizing Energy Consumption Leads to the Emergence of Gaits in Legged Robots


[10] Rapid Locomotion via Reinforcement Learning


2.2.4 Others

[1] Transition Motion Tensor: A Data-Driven Approach for Versatile and Controllable Agents in Physically Simulated Environments [Siggraph Asia 2021 Technical Communications]


[2] CARL: Controllable Agent with Reinforcement Learning for Quadruped Locomotion [Siggraph 2020]

