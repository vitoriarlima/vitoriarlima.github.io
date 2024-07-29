---
title: "Project 2: Curriculum Learning applied in RL simulation complexity to lighten and speed up an agent's training time."
excerpt: "Work done under the supervision of Professor Daniel Bruder and Professor Robert Wood at the Harvard's Microrobotics Lab."
collection: portfolio
category: ai
permalink: /portfolio/ai-project-2

---

### Curriculum Complexity: A Framework for Computationally Efficient Reinforcement Learning Control of Soft Robotic Agents

<!-- <div style="text-align: center;">
    <figure style="display: inline-block;">
        <img src="/files/curr_compl.png" alt="Curr" style="width: 500px; height: 500px;" />
        <figcaption>Figure 1: In Blue is the training with Curriculum Learning per simulation complexity. In Red is a training with the most 'complex' simulation throughout the entire training process. As seen from the graphs on the right, the training done with Curriculum Complexity are successfully completed in almost <strong>half</strong> of the training time and compute.</figcaption>
    </figure>
</div> -->


<!-- <div style="text-align: center;">
    <figure>
        <img src="/files/curr_compl.png" alt="Curr" style="width: 500px; height: 500px;" />
        <figcaption>Figure 1: In Blue is the training with Curriculum Learning per simulation complexity. In Red is a training with the most 'complex' simulation throughout the entire training process. As seen from the graphs on the right, the training done with Curriculum Complexity are successfully completed in almost <strong>half</strong> of the training time and compute.</figcaption>
    </figure>
</div> -->

<div style="text-align: center;">
    <figure>
        <img src="/files/curr_compl.png" alt="Curr" width="100"  />
        <figcaption>Figure 1: In Blue is the training with Curriculum Learning per simulation complexity. In Red is a training with the most 'complex' simulation throughout the entire training process. As seen from the graphs on the right, the training done with Curriculum Complexity are successfully completed in almost <strong>half</strong> of the training time and compute. </figcaption>
    </figure>
</div>

<!-- <div style="text-align: center;">
    <figure>
        <img src="/files/curr_compl.png" alt="Curr"  height="100" />
        <figcaption>Figure 1: In Blue is the training with Curriculum Learning per simulation complexity. In Red is a training with the most 'complex' simulation throughout the entire training process. As seen from the graphs on the right, the training done with Curriculum Complexity are successfully completed in almost <strong>half</strong> of the training time and compute. </figcaption>
    </figure>
</div> -->

## Overview

This project presents a framework for reducing the computational expense associated with controlling soft robotic agents using reinforcement learning. While there has been significant research on controlling rigid robotic arms, the control of soft robots, particularly through machine learning methods, remains an underexplored area. This thesis proposes an online reinforcement learning approach aimed at effectively controlling soft robots while minimizing computational costs.

### Key Objectives

1. **Reduce Computational Expense**: Develop methods to lower the computational burden for controlling soft robots with infinite degrees of freedom (DOF).
2. **Curriculum Learning**: Leverage curriculum learning to train reinforcement learning policies on low-fidelity systems and gradually increase fidelity.
3. **Framework Development**: Create a framework, Complexity Curriculum, to train soft robotic agents efficiently using SoMoGym environments.

### Methodology

- **SoMoGym Environments**: Utilize the SoMoGym toolkit to simulate and train controllers for soft robots in environments like Planar Reaching and Block Pushing.
- **Curriculum Learning**: Apply curriculum learning by training agents on tasks of increasing complexity, represented by the number of segments per actuator in the soft robot simulation.
- **PPO Algorithm**: Implement Proximal Policy Optimization (PPO) to train the reinforcement learning policies, balancing exploration and exploitation to optimize learning.

### Experiments

#### Baseline Experiments

1. **Planar Reaching**: Trained agents with 2, 5, 10, and 20 segments per actuator to observe the impact of discretization on training time and learned behaviors.
2. **Block Pushing**: Conducted similar experiments with 2, 5, 10, and 20 segments per actuator, noting the differences in training duration and performance.

<div style="text-align: center;">
    <figure>
        <img src="/files/without_curr_compl.png" alt="Curr2" width="200" />
        <figcaption>Figure 2: The more complexity is added, the more the agent is able to learn the physics of movement and the more rewards are achieved in the RL training Process. But this comes at the expense of time compute, see how the Red Line (most complex simulation) takes almost 4x as the least complex simulation to complete. </figcaption> 
    </figure>
</div>



#### Curriculum Complexity

1. **Planar Reaching**: Implemented curriculum learning over 2, 4, 5, 8, 10, and 15 segments per actuator, demonstrating faster convergence and higher rewards compared to static high-fidelity training.
2. **Block Pushing**: Applied curriculum learning to train agents from 2 to 10 segments per actuator, achieving efficient training despite higher variance due to interaction with the environment.

### Findings

- **Training Efficiency**: Curriculum learning significantly reduced training time while maintaining high fidelity in learned behaviors.
- **Performance Improvement**: Agents trained using curriculum learning achieved comparable or better performance than those trained directly on high-fidelity simulations.

### Conclusion

This framework demonstrates the potential of curriculum learning in enhancing the efficiency and effectiveness of reinforcement learning for soft robotic control. By gradually increasing task complexity, the computational burden is reduced, paving the way for more advanced and practical applications of soft robotics in various fields.

### Repository and Resources

To read the full analysis, you can download the [PDF file](/files/Vitoria___Master_Thesis.pdf).


