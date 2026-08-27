---
permalink: /publications/
title: "Publications"
excerpt: "My Publications"
author_profile: true
---


# 📝 Publications

<style>
  .paper-title {
    position: relative;
    cursor: pointer;
  }
  
  .abstract-tooltip {
    display: none;
    position: absolute;
    top: 100%;
    left: 0;
    width: 100%;
    background-color: #f9f9f9;
    border: 1px solid #ddd;
    padding: 10px;
    border-radius: 5px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.2);
    z-index: 100;
    margin-top: 5px;
    font-weight: normal;
    font-size: 14px;
    color: #333;
    line-height: 1.4;
    text-align: left;
  }
  
  .paper-title:hover .abstract-tooltip {
    display: block;
  }
</style>


<div class="paper-item" style="display: flex; align-items: flex-start; margin-bottom: 20px;">
  <!-- 左侧图片 -->
  <div class="paper-image" style="flex: 0 0 24%; max-width: 24%; margin-right: 20px;">
    <div class="badge">
      RA-L 2026
    </div>
    <a href="/images/paper_cover/RAL2026.png" target="_blank">
      <img src="/images/paper_cover/RAL2026.png" alt="Paper Cover" style="width: 100%; height: auto; border-radius: 8px;">
    </a>
  </div>
  <!-- 右侧文字内容 -->
  <div class="paper-content" style="flex: 1;">
    <h3 class="paper-title" style="margin: 0 0 10px; color:rgb(18, 74, 134);">
        Homotopy-Aware Corridor Generation without Predefined Reference Paths
        <div class="abstract-tooltip">
          <b><em>Abstract:</em></b> Generating safe corridors is essential for collision-free robotic motion planning, yet most existing methods rely on predefined reference paths, which bias corridor geometry and implicitly limit the homotopy classes that can be explored. We propose a reference-path-free corridor generation framework on graphs of convex sets (GCS) that constructs corridors directly as sequences of convex sets, allowing corridor structure to emerge from the free-space representation rather than from a guiding path. To reason about similarity among corridors, we extend visibility-based deformation from paths to convex-set sequences, enabling the fusion of topologically redundant corridors while preserving distinct alternatives. To overcome the limited adaptability of existing GCS methods based on static global decompositions, we further develop an adaptive multi-scale GCS, in which a sampling-based fine-scale graph supports localized updates and a visibility-based coarse-scale graph enables compact global exploration. The two levels maintain topological consistency, allowing incremental updates without full graph reconstruction under environmental uncertainty. Numerical experiments characterize GCS construction, corridor generation, homotopy-aware exploration, and local updates, showing efficient graph construction, stable trajectory-level performance, and shorter-duration homotopy-aware trajectories than existing baselines. Hardware experiments on ground and aerial robots, including deployment with onboard localization, further validate the framework under translated and previously unknown obstacles.
        </div>
    </h3>
    <p style="margin: 0 0 5px;"> <u>Haoze Dong</u>, Minghan Li, Meng Guo, Zhongkui Li</p>
    <div style="margin-top: 10px;">
      <a href="https://ieeexplore.ieee.org/document/11652891" target="_blank" style="display: inline-block; padding: 2px 0px;  width: 60px; text-align: center; background-color:rgb(164, 37, 22); color: white; text-decoration: none; border-radius: 5px; margin-right: 10px;">PDF</a>
      <a href="https://github.com/HauserDong/path-free-gcs-corridors" target="_blank" style="display: inline-block; padding: 2px 0px;  width: 60px; text-align: center; background-color:rgb(11, 11, 11); color: white; text-decoration: none; border-radius: 5px; margin-right: 10px;">Code</a>
      <a href="https://youtu.be/6j3_F9xE-zM" target="_blank" style="display: inline-block; padding: 2px 0px;  width: 60px; text-align: center; background-color:rgb(216, 53, 61); color: white; text-decoration: none; border-radius: 5px;">Video</a>
    </div>
  </div>
</div>


<div class="paper-item" style="display: flex; align-items: flex-start; margin-bottom: 20px;">
  <!-- 左侧图片 -->
  <div class="paper-image" style="flex: 0 0 24%; max-width: 24%; margin-right: 20px;">
    <div class="badge">
      IROS 2025
    </div>
    <a href="/images/paper_cover/iros2025.jpg" target="_blank">
      <img src="/images/paper_cover/iros2025.jpg" alt="Paper Cover" style="width: 100%; height: auto; border-radius: 8px;">
    </a>
  </div>
  <!-- 右侧文字内容 -->
  <div class="paper-content" style="flex: 1;">
    <h3 class="paper-title" style="margin: 0 0 10px; color:rgb(18, 74, 134);">
        Homotopy-aware Multi-agent Navigation via Distributed Model Predictive Control
        <div class="abstract-tooltip">
          <b><em>Abstract:</em></b> Multi-agent trajectory planning requires ensuring both safety and efficiency, yet deadlocks remain a significant challenge, especially in obstacle-dense environments. Such deadlocks frequently occur when multiple agents attempt to traverse the same long and narrow corridor simultaneously. To address this, we propose a novel distributed trajectory planning framework that bridges the gap between global path and local trajectory cooperation. At the global level, a homotopy-aware optimal path planning algorithm is proposed, which fully leverages the topological structure of the environment. A reference path is chosen from distinct homotopy classes by considering both its spatial and temporal properties, leading to improved coordination among agents globally. At the local level, a model predictive control-based trajectory optimization method is used to generate dynamically feasible and collision-free trajectories. Additionally, an online replanning strategy ensures its adaptability to dynamic environments. Simulations and experiments validate the effectiveness of our approach in mitigating deadlocks. Ablation studies demonstrate that by incorporating time-aware homotopic properties into the underlying global paths, our method can significantly reduce deadlocks and improve the average success rate from 4%-13% to over 90% in randomly generated dense scenarios.
        </div>
    </h3>
    <p style="margin: 0 0 5px;"> <u>Haoze Dong</u>, Meng Guo, Chengyi He, Zhongkui Li</p>
    <div style="margin-top: 10px;">
      <a href="https://ieeexplore.ieee.org/document/11246185" target="_blank" style="display: inline-block; padding: 2px 0px;  width: 60px; text-align: center; background-color:rgb(164, 37, 22); color: white; text-decoration: none; border-radius: 5px; margin-right: 10px;">PDF</a>
      <a href="https://github.com/HauserDong/HomoMPC" target="_blank" style="display: inline-block; padding: 2px 0px;  width: 60px; text-align: center; background-color:rgb(11, 11, 11); color: white; text-decoration: none; border-radius: 5px; margin-right: 10px;">Code</a>
      <a href="https://www.youtube.com/watch?v=9HCiO9QTpgw" target="_blank" style="display: inline-block; padding: 2px 0px;  width: 60px; text-align: center; background-color:rgb(216, 53, 61); color: white; text-decoration: none; border-radius: 5px;">Video</a>
    </div>
  </div>
</div>


<div class="paper-item" style="display: flex; align-items: flex-start; margin-bottom: 20px;">
  <!-- 左侧图片 -->
  <div class="paper-image" style="flex: 0 0 24%; max-width: 24%; margin-right: 20px;">
    <div class="badge">
      IROS 2024
    </div>
    <a href="/images/paper_cover/IROS2024.png" target="_blank">
      <img src="/images/paper_cover/IROS2024.png" alt="Paper Cover" style="width: 100%; height: auto; border-radius: 8px;">
    </a>
  </div>
  <!-- 右侧文字内容 -->
  <div class="paper-content" style="flex: 1;">
    <h3 class="paper-title" style="margin: 0 0 10px; color:rgb(18, 74, 134);">
        Asynchronous Spatial-Temporal Allocation for Trajectory Planning of Heterogeneous Multi-Agent Systems
        <div class="abstract-tooltip">
          <b><em>Abstract:</em></b> To plan the trajectories of a large-scale heterogeneous swarm, sequentially or synchronously distributed methods usually become intractable due to the lack of global clock synchronization. To this end, we provide a novel asynchronous spatial-temporal allocation method. Specifically, between a pair of agents, the allocation is proposed to determine their corresponding derivable time-stamped space and can be updated in an asynchronous way, by inserting a waiting duration between two consecutive replanning steps. It is theoretically shown that the inter-agent collision is avoided and the allocation ensures timely updates. Comprehensive simulations and comparisons with state-of-the-art baselines validate the effectiveness of the proposed method and illustrate its improvement in completion time and moving distance. Finally, hardware experiments are carried out, where 8 heterogeneous unmanned ground vehicles with onboard computation navigate in cluttered scenarios with high agility.
        </div>
    </h3>
    <p style="margin: 0 0 5px;"> Yuda Chen, <u>Haoze Dong</u>, Zhongkui Li</p>
    <div style="margin-top: 10px;">
      <a href="https://ieeexplore.ieee.org/document/10801393" target="_blank" style="display: inline-block; padding: 2px 0px;  width: 60px; text-align: center; background-color:rgb(164, 37, 22); color: white; text-decoration: none; border-radius: 5px; margin-right: 10px;">PDF</a>
      <a href="https://github.com/CYDXYYJ/ASAP" target="_blank" style="display: inline-block; padding: 2px 0px;  width: 60px; text-align: center; background-color:rgb(11, 11, 11); color: white; text-decoration: none; border-radius: 5px; margin-right: 10px;">Code</a>
      <a href="https://youtu.be/au3fhqbySOE" target="_blank" style="display: inline-block; padding: 2px 0px;  width: 60px; text-align: center; background-color:rgb(216, 53, 61); color: white; text-decoration: none; border-radius: 5px;">Video</a>
    </div>
  </div>
</div>


<div class="paper-item" style="display: flex; align-items: flex-start; margin-bottom: 20px;">
  <!-- 左侧图片 -->
  <div class="paper-image" style="flex: 0 0 24%; max-width: 24%; margin-right: 20px;">
    <div class="badge">
      航空学报 2023
    </div>
    <a href="/images/paper_cover/hangkongxuebao2023.png" target="_blank">
      <img src="/images/paper_cover/hangkongxuebao2023.png" alt="Paper Cover" style="width: 100%; height: auto; border-radius: 8px;">
    </a>
  </div>
  <!-- 右侧文字内容 -->
  <div class="paper-content" style="flex: 1;">
    <h3 class="paper-title" style="margin: 0 0 10px; color:rgb(18, 74, 134);">
        障碍物空间下分布式轨迹规划的死锁破解
        <div class="abstract-tooltip">
          <b><em>摘要:</em></b> 基于优化的分布式轨迹规划方法因具有较强的可解释性和可扩展性而备受关注，但由于缺少中心节点和全局优先级，容易诱发集群运动陷入死锁，即若干机器人互相阻隔而无法到达终点的情形。现有的障碍物空间下死锁解决方案大多是启发式的，缺乏理论支撑。为此，本文针对可行域为半空间交集这一基础情形，通过构建多机器人轨迹规划的模型预测控制（MPC）问题，得到了死锁发生的必要条件，并指出该条件可以理解为机器人所受来自自身目标的吸引力、来自其他机器人的斥力和来自障碍物约束面的斥力三者的受力平衡。在此基础上，提出了一种死锁破解策略，并证明其在一定条件下可避免发生稳定的死锁现象。最后，通过密集空间下的随机对比仿真验证了算法的有效性。
        </div>
    </h3>
    <p style="margin: 0 0 10px; font-size: 14px; color:rgba(100, 100, 100, 0.7);">
       Deadlock Resolution of Distributed Trajectory Planning in Obstacle Space (Chinese)
    </p>
    <p style="margin: 0 0 5px;"> <u>董豪泽</u>, 陈昱达, 刘丹, 李忠奎</p>
    <p style="margin: 0 0 10px; font-size: 14px; color:rgba(100, 100, 100, 0.7);">
      <u>Haoze Dong</u>, Yuda Chen, Dan Liu, Zhongkui Li
    </p>
    <p style="margin: 0 0 10px; font-size: 12px; color: rgb(151, 41, 0); font-weight: bold;">
      The conference version received the Best Paper Award at CCSICC 2023 🏆
    </p>
    <div style="margin-top: 10px;">
      <a href="https://hkxb.buaa.edu.cn/CN/10.7527/S1000-6893.2023.29771" target="_blank" style="display: inline-block; padding: 2px 0px;  width: 60px; text-align: center; background-color:rgb(164, 37, 22); color: white; text-decoration: none; border-radius: 5px; margin-right: 10px;">PDF</a>
    </div>
  </div>
</div>