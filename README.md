# 🌌 VoidGrad

![C++](https://img.shields.io/badge/C++-17%2B-blue.svg?style=flat-square&logo=c%2B%2B)
![Build](https://img.shields.io/badge/build-CMake-green.svg?style=flat-square)
![License](https://img.shields.io/badge/License-All%20Rights%20Reserved-red.svg?style=flat-square)

**A bare-metal, no-framework C++ auto-differentiation engine and Reinforcement Learning environment built entirely from scratch.**

---

## 📖 About
**VoidGrad** is an educational and architectural exploration of artificial intelligence at the systems level. It purposefully steps away from heavy Python frameworks like PyTorch and TensorFlow, diving straight into the "void" of raw C++ memory management, manual pointer manipulation, and raw mathematical calculus.

This project implements a foundational auto-grad engine, dynamic computational graphs, and neural network abstractions, ultimately culminating in a custom Reinforcement Learning agent capable of mastering terminal-based environments.

## ✨ Features
* **Bare-Metal Tensor Core:** Custom scalar and matrix classes with overloaded C++ operators for natural equation building.
* **Dynamic Auto-Differentiation:** A ground-up computational graph that tracks mathematical operations and applies the Chain Rule for exact gradient computation (`backward()`).
* **Zero Dependencies:** No external math libraries (e.g., Eigen, BLAS) or ML frameworks. Everything from matrix multiplication to auto-grad logic is handwritten.
* **Neural Network Abstractions:** High-level APIs for `Neuron`, `LinearLayer`, `MLP`, Activation Functions (ReLU, Sigmoid), and Loss Functions (MSE).
* **Reinforcement Learning:** Includes a custom Deep Q-Learning implementation and a terminal-based testing environment.

---

## 🗺️ Project Roadmap
This repository is structured into four sequential phases of development:

1. **Phase 1: The Tensor & Math Foundation**
   - Core mathematical structures and operator overloading.
2. **Phase 2: The Auto-Grad Engine**
   - Forward pass evaluation, dynamic computational graph generation, and topological sorting for the backward pass.
3. **Phase 3: Neural Network Wrapping**
   - Encapsulating the engine into trainable Multi-Layer Perceptrons.
4. **Phase 4: The RL Environment**
   - Terminal-based agent training via Q-Learning using VoidGrad MLPs.

---

## 🛠️ Build Instructions

### Prerequisites
* A C++17 compatible compiler (GCC, Clang, or MSVC)
* CMake (3.10+)

### Compiling from Source
```bash
# Clone the repository
git clone [https://github.com/yourusername/VoidGrad.git](https://github.com/yourusername/VoidGrad.git)
cd VoidGrad

# Create a build directory
mkdir build && cd build

# Generate build files and compile
cmake ..
make
