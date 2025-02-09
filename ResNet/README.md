# ResNet Implementation

This repository contains an implementation of the ResNet (Residual Network) architecture using PyTorch. ResNet is a popular deep learning model known for its ability to train very deep networks by using residual connections.

## Overview

ResNet was introduced in the paper "Deep Residual Learning for Image Recognition" by Kaiming He et al. It addresses the problem of vanishing gradients in deep networks by introducing shortcut connections, or residuals, that allow gradients to flow through the network more easily.

### Key Features of ResNet:

- **Residual Blocks**: Each block contains a series of convolutional layers with a shortcut connection that bypasses one or more layers.
- **Identity Mapping**: The shortcut connection helps in learning identity mappings, which makes it easier to optimize very deep networks.
- **Deep Architectures**: ResNet can be scaled to hundreds or even thousands of layers.

## Implementation Details

This implementation includes:

- A `Block` class that defines the basic building block of ResNet.
- A `ResNet` class that constructs the full network using multiple blocks.
- A `ResNet50` function that creates a 50-layer ResNet model.

### Code Structure

- **Block**: Implements a single residual block with three convolutional layers.
- **ResNet**: Constructs the full ResNet architecture by stacking multiple blocks.
- **ResNet50**: A specific configuration of ResNet with 50 layers.