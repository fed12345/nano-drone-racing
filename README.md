# Autonomous Racing Framework for Nano Drones

In this repository, we introduce an initial framework for a cutting-edge software platform designed to enable autonomous racing capabilities in nano drones. By integrating neural networks optimized for real-time processing on resource-constrained hardware, this framework addresses the unique challenges of autonomous drone racing in a highly efficient manner. 

[Paper](files/Modular_Neural_Network_Navigatiom.pdf)

## Key Components

- **Lightweight Convolutional Neural Network (CNN)**: A streamlined CNN, based on the Gatenet architecture, has been adapted to minimize computational demand. This network is successfully deployed on a GAP8 processor, achieving a processing rate of 16Hz. The CNN provides data on gate size and location, which serves as input for the positioning algorithm.

[Vision Net](https://github.com/fed12345/visionnet): Repository for training and deployment of this vision network


- **Reinforcement Learning-based Guidance and Control**: A second neural network, trained through reinforcement learning, handles the drone’s guidance and control functions. This network runs at an impressive rate of 167Hz on an STM32F405 processor, outputting attitude rates and thrust values for an attitude rate PID controller.
  
[Control Net](https://github.com/fed12345/controlnet): Repository for training and deployment of the control network

## Findings and Insights

Our findings demonstrate that state-of-the-art neural networks for autonomous drone racing can be effectively deployed on nano drones, even with limited processing power. However, the study also highlights specific limitations, such as the perception network’s sensitivity to bright areas (e.g., white pixels), which can impact performance when intense light sources are present. These insights emphasize the importance of comprehensive dataset composition and diverse training scenarios to enhance neural network robustness and reliability for autonomous nano drone racing.


