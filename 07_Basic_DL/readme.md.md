# Deep Learning & CNN Mastery Checklists

> A complete, phase-by-phase learning roadmap covering Deep Learning fundamentals and Convolutional Neural Networks — from math foundations to research-level understanding.

---

## Table of Contents

1. [Deep Learning (DL)](#1-deep-learning-dl)
2. [Convolutional Neural Networks (CNN)](#2-convolutional-neural-networks-cnn)

---

# 1. Deep Learning (DL)

*From Beginner → Master → Research-Level Understanding*

---

## Phase 0: Mathematical Foundations

### Linear Algebra

- [ ] Scalars, Vectors, Matrices, Tensors
- [ ] Matrix Operations (add, subtract, scale)
- [ ] Dot Product
- [ ] Matrix Multiplication
- [ ] Transpose
- [ ] Inverse
- [ ] Rank
- [ ] Eigenvalues & Eigenvectors
- [ ] Singular Value Decomposition (SVD)

**Deep Dive**
- [ ] Why tensors are the language of deep learning
- [ ] Memory representation of matrices
- [ ] Sparse vs dense matrices
- [ ] GPU matrix operations

---

### Calculus

- [ ] Functions & Limits
- [ ] Derivatives & Partial Derivatives
- [ ] Chain Rule
- [ ] Gradients
- [ ] Jacobian
- [ ] Hessian

**Deep Dive**
- [ ] Why gradient descent works
- [ ] Optimization landscapes
- [ ] Saddle points
- [ ] Vanishing & exploding gradients

---

### Probability & Statistics

- [ ] Mean, Median, Variance, Standard Deviation
- [ ] Probability Distributions
- [ ] Conditional Probability
- [ ] Bayes Theorem
- [ ] Expectation

**Deep Dive**
- [ ] Maximum Likelihood Estimation (MLE)
- [ ] Entropy
- [ ] Cross Entropy
- [ ] KL Divergence

---

### Information Theory (Added)

- [ ] Information content of an event
- [ ] Mutual information
- [ ] Why cross-entropy is used as a loss
- [ ] Connection between entropy and model uncertainty

---

## Phase 1: Machine Learning Foundations

### Understanding ML

- [ ] What is Machine Learning?
- [ ] AI vs ML vs DL
- [ ] Supervised / Unsupervised / Reinforcement Learning

### Data Preparation

- [ ] Train / Validation / Test Split
- [ ] Data Cleaning
- [ ] Missing Values & Outlier Handling

### Feature Engineering

- [ ] Feature Scaling
- [ ] Normalization & Standardization
- [ ] Encoding Categorical Variables

### Classical Models

- [ ] Linear Regression / Logistic Regression
- [ ] KNN / Decision Trees / Random Forest
- [ ] SVM / Naive Bayes

### Understand Limitations of Classical ML

- [ ] Feature engineering burden
- [ ] Scalability issues
- [ ] Why Deep Learning emerged

---

## Phase 2: Neural Network Fundamentals

### Biological Inspiration

- [ ] Human neuron → Artificial neuron
- [ ] Inputs, Weights, Bias, Output

### Perceptron

- [ ] Single neuron model
- [ ] Linear classification
- [ ] Limitations

**Deep Dive**
- [ ] XOR problem
- [ ] Why single-layer networks fail
- [ ] Universal approximation theorem

### Multi-Layer Neural Networks

- [ ] Input Layer / Hidden Layer / Output Layer
- [ ] Parameters: Weights & Biases
- [ ] Activations

### Understand

- [ ] Depth vs width of a network
- [ ] Why depth matters more than width (in practice)

---

## Phase 3: Forward Propagation

### Understand Flow

- [ ] Input → Hidden Layer → Output
- [ ] Prediction generation

### Mathematics

- [ ] Weighted sum
- [ ] Matrix multiplication
- [ ] Activation application

### Deep Dive

- [ ] Tensor dimensions at each layer
- [ ] Batch processing
- [ ] Vectorization vs loops

---

## Phase 4: Activation Functions

### Core Activations

- [ ] Sigmoid
- [ ] Tanh
- [ ] ReLU
- [ ] Leaky ReLU
- [ ] ELU
- [ ] GELU
- [ ] Softmax
- [ ] Swish (Added)
- [ ] Mish (Added)

### Deep Dive

- [ ] Saturation problem
- [ ] Dead neuron problem (dying ReLU)
- [ ] Why ReLU dominates
- [ ] When to use Sigmoid vs Softmax vs ReLU
- [ ] Output layer activation choice by task

---

## Phase 5: Loss Functions

### Regression Losses

- [ ] MSE (Mean Squared Error)
- [ ] MAE (Mean Absolute Error)
- [ ] Huber Loss

### Classification Losses

- [ ] Binary Cross Entropy
- [ ] Categorical Cross Entropy
- [ ] Focal Loss (Added — handles class imbalance)

### Deep Dive

- [ ] Why loss functions exist
- [ ] Optimization objective
- [ ] Probabilistic interpretation of cross entropy
- [ ] Choosing the right loss for your task

---

## Phase 6: Backpropagation

### Core Concepts

- [ ] Error computation
- [ ] Gradient calculation via chain rule
- [ ] Weight updates

### Deep Dive

- [ ] Computational graph
- [ ] Automatic differentiation (Autograd)
- [ ] Reverse mode differentiation
- [ ] Gradient accumulation
- [ ] Numerical gradient checking

---

## Phase 7: Optimization

### Gradient Descent Variants

- [ ] Batch Gradient Descent
- [ ] Stochastic Gradient Descent (SGD)
- [ ] Mini-Batch Gradient Descent

### Advanced Optimizers

- [ ] Momentum
- [ ] RMSProp
- [ ] Adam
- [ ] AdamW
- [ ] Nadam
- [ ] Lion (Added — modern optimizer)

### Learning Rate Techniques

- [ ] Learning Rate Scheduling
- [ ] Step Decay / Cosine Annealing
- [ ] Warmup (Added)
- [ ] Cyclical Learning Rates (Added)

### Deep Dive

- [ ] Convergence behavior
- [ ] Local minima vs saddle points
- [ ] Why Adam is the default choice
- [ ] Weight decay vs L2 regularization

---

## Phase 8: Training Neural Networks

### Training Pipeline

- [ ] Epoch / Batch / Iteration
- [ ] Training loop structure

### Monitoring

- [ ] Training loss & Validation loss curves
- [ ] Accuracy tracking
- [ ] Gradient norms (Added)

### Common Problems

- [ ] Underfitting → solutions: more capacity, more data
- [ ] Overfitting → solutions: regularization, dropout, augmentation

### Regularization Techniques

- [ ] L1 / L2 Regularization
- [ ] Dropout
- [ ] Batch Normalization (Added)
- [ ] Layer Normalization (Added)
- [ ] Early Stopping
- [ ] Data Augmentation
- [ ] Label Smoothing (Added)

### Weight Initialization (Added)

- [ ] Random initialization
- [ ] Xavier / Glorot initialization
- [ ] He initialization
- [ ] Why initialization matters

---

## Phase 9: Deep Learning Frameworks

### NumPy Foundation

- [ ] Tensor operations
- [ ] Broadcasting
- [ ] Vectorization

### PyTorch

- [ ] Tensor basics
- [ ] Autograd
- [ ] nn.Module
- [ ] DataLoader & Dataset
- [ ] Custom training loops
- [ ] torch.compile (Added)

### TensorFlow / Keras

- [ ] Tensors
- [ ] Keras Sequential & Functional API
- [ ] Model API
- [ ] TF Data pipeline (Added)

### Understand

- [ ] PyTorch vs TensorFlow tradeoffs
- [ ] When to use each framework

---

## Phase 10: Computer Vision

### CNN Fundamentals

- [ ] Convolution
- [ ] Filters / Kernels
- [ ] Feature Maps
- [ ] Pooling

### CNN Architectures

- [ ] LeNet / AlexNet / VGG
- [ ] ResNet / DenseNet
- [ ] EfficientNet / ConvNeXt (Added)
- [ ] MobileNet (Added — edge deployment)

### Applications

- [ ] Image Classification
- [ ] Object Detection (YOLO, Faster R-CNN)
- [ ] Semantic Segmentation (U-Net, DeepLab)
- [ ] Instance Segmentation (Mask R-CNN)
- [ ] Image Generation (Added)

---

## Phase 11: Natural Language Processing

### Foundations

- [ ] Text preprocessing
- [ ] Tokenization (word, subword, BPE)
- [ ] Embeddings (Word2Vec, GloVe, FastText)

### Sequence Models

- [ ] RNN
- [ ] LSTM
- [ ] GRU
- [ ] Vanishing gradient in RNNs

### Transformers

- [ ] Attention mechanism
- [ ] Self-attention
- [ ] Multi-head attention
- [ ] Positional encoding
- [ ] Encoder / Decoder architecture

### Large Language Models

- [ ] GPT architecture (decoder-only)
- [ ] BERT architecture (encoder-only)
- [ ] T5 (encoder-decoder)
- [ ] Fine-tuning strategies
- [ ] Prompt engineering
- [ ] RAG basics

---

## Phase 12: Generative AI

### Autoencoders

- [ ] Encoder / Decoder / Latent space
- [ ] Denoising autoencoders (Added)

### Variational Autoencoders (VAE)

- [ ] VAE architecture
- [ ] Latent distributions
- [ ] Reparameterization trick (Added)

### GANs

- [ ] Generator / Discriminator
- [ ] Adversarial training
- [ ] Mode collapse problem (Added)
- [ ] DCGAN / StyleGAN overview (Added)

### Diffusion Models

- [ ] Forward noise process
- [ ] Reverse denoising
- [ ] DDPM
- [ ] Stable Diffusion concepts
- [ ] DDIM sampling (Added)

### Flow-Based Models (Added)

- [ ] Normalizing flows concept
- [ ] When to use vs VAE vs GAN

---

## Phase 13: Scaling Deep Learning

### Hardware

- [ ] CPU vs GPU vs TPU
- [ ] When to use each

### Distributed Training

- [ ] Data parallelism
- [ ] Model parallelism
- [ ] Tensor parallelism (Added)
- [ ] Pipeline parallelism (Added)
- [ ] ZeRO optimization (Added — DeepSpeed)

### Model Optimization

- [ ] Mixed precision training (FP16/BF16)
- [ ] Quantization (INT8, INT4)
- [ ] Pruning
- [ ] Knowledge distillation (Added)
- [ ] Flash Attention (Added)

---

## Phase 14: Deep Learning Internals

### Tensor Internals

- [ ] Tensor memory layout
- [ ] Strides
- [ ] Views vs Copies
- [ ] Contiguous vs non-contiguous tensors (Added)

### Autograd Internals

- [ ] Computation graph construction
- [ ] Backward graph
- [ ] Gradient accumulation
- [ ] Detaching from graph

### GPU Internals

- [ ] CUDA basics
- [ ] GPU memory hierarchy (HBM, SRAM, registers)
- [ ] Kernel execution model
- [ ] Memory bandwidth bottleneck (Added)

---

## Phase 15: MLOps for Deep Learning

### Experiment Management

- [ ] Experiment tracking (MLflow, Weights & Biases)
- [ ] Model versioning (DVC)
- [ ] Hyperparameter search (Optuna, Ray Tune)

### Deployment

- [ ] ONNX export
- [ ] TorchScript
- [ ] TensorRT
- [ ] Serving (FastAPI, Triton Inference Server)

### Infrastructure

- [ ] Docker
- [ ] Kubernetes
- [ ] Cloud GPU providers (AWS, GCP, Lambda Labs)

### Monitoring

- [ ] Data drift detection (Added)
- [ ] Model performance tracking (Added)
- [ ] Alerting on degradation (Added)

---

## Phase 16: Research-Level Deep Learning

### Landmark Papers to Read

- [ ] AlexNet (2012)
- [ ] ResNet (2015)
- [ ] Attention Is All You Need (2017)
- [ ] BERT (2018)
- [ ] GPT-2 / GPT-3
- [ ] DALL-E / Stable Diffusion
- [ ] LoRA (2021) — efficient fine-tuning

### Research Skills

- [ ] How to read a paper efficiently
- [ ] Reproducing results
- [ ] Implementing papers from scratch
- [ ] Writing experiment logs

### Open Source Contributions

- [ ] PyTorch internals
- [ ] Hugging Face ecosystem
- [ ] Contributing to open-source DL projects

---

## Projects

### Beginner

- [ ] ANN from scratch with NumPy
- [ ] MNIST digit classifier
- [ ] Binary classification on tabular data

### Intermediate

- [ ] CNN image classifier (CIFAR-10)
- [ ] Sentiment analysis with LSTM
- [ ] Text classification with BERT

### Advanced

- [ ] Fine-tune an LLM (LoRA)
- [ ] Build a VAE from scratch
- [ ] Object detection with YOLO

### Expert

- [ ] Train a GAN from scratch
- [ ] Build a Transformer from scratch
- [ ] Reproduce a research paper
- [ ] Build a production ML pipeline

---

## Final Mastery

**Theory**
- [ ] Explain deep learning from first principles
- [ ] Derive backpropagation manually
- [ ] Explain optimization mathematically
- [ ] Explain the bias-variance tradeoff in deep networks

**Practical**
- [ ] Build ANN from scratch using NumPy
- [ ] Build CNN from scratch
- [ ] Train Transformer models
- [ ] Deploy production models

**Internals**
- [ ] Explain autograd internals
- [ ] Explain tensor memory layout
- [ ] Explain CUDA execution model

**Research**
- [ ] Read and implement papers
- [ ] Contribute to DL frameworks
- [ ] Design novel architectures

---

## True Master Level

- [ ] Teach DL from first principles
- [ ] Build models from scratch
- [ ] Debug training failures systematically
- [ ] Optimize large-scale models
- [ ] Read framework source code
- [ ] Reproduce research papers
- [ ] Contribute to DL ecosystems
- [ ] Design new architectures
- [ ] Lead AI projects end-to-end
- [ ] Mentor other engineers

---

# 2. Convolutional Neural Networks (CNN)

*From Beginner → Master → Research-Level Understanding*

---

## Phase 0: Prerequisites

### Linear Algebra

- [ ] Vectors & Matrices
- [ ] Matrix Multiplication
- [ ] Tensor basics & Tensor Dimensions

### Calculus

- [ ] Derivatives & Partial Derivatives
- [ ] Chain Rule
- [ ] Gradients

### Probability & Statistics

- [ ] Mean, Variance
- [ ] Probability Distributions

### Deep Learning Basics (Added)

- [ ] What is a neural network?
- [ ] Forward propagation
- [ ] Backpropagation intuition
- [ ] Loss functions

---

## Phase 1: Why CNNs Exist

### Problem with Fully Connected Networks on Images

- [ ] Why traditional neural networks struggle with images
- [ ] Curse of dimensionality
- [ ] Parameter explosion

**Example**
- [ ] Calculate parameters required for FC network on a 224×224 image
- [ ] Understand memory and compute requirements

### Image Fundamentals

- [ ] Pixels & Resolution
- [ ] RGB channels & Grayscale images
- [ ] Image tensors (H × W × C)

**Deep Dive**
- [ ] Image as matrix vs tensor
- [ ] Channel-first (NCHW) vs channel-last (NHWC) formats
- [ ] How images are loaded into memory

### Key CNN Properties (Added)

- [ ] Local connectivity
- [ ] Weight sharing
- [ ] Translational equivariance
- [ ] Translational invariance (via pooling)

---

## Phase 2: Convolution Fundamentals

### Understanding Convolution

- [ ] What is a convolution?
- [ ] Why convolution works for images
- [ ] Sliding window concept

### Filters / Kernels

- [ ] Kernel concept & dimensions
- [ ] Learnable filters

**Manual Practice**
- [ ] Apply 3×3 kernel manually on a small matrix
- [ ] Compute output feature map by hand
- [ ] Understand weight sharing across positions

### Feature Maps

- [ ] Feature extraction
- [ ] Activation maps
- [ ] Local pattern detection

### Deep Dive

- [ ] Mathematical convolution vs cross-correlation
- [ ] Why DL libraries use cross-correlation
- [ ] Dilated convolution (Added)
- [ ] Depthwise separable convolution (Added — used in MobileNet)
- [ ] Transposed convolution / deconvolution (Added — used in segmentation)

---

## Phase 3: CNN Building Blocks

### Convolution Layer

- [ ] Input tensor
- [ ] Number of filters
- [ ] Kernel size
- [ ] Stride
- [ ] Padding (valid vs same)

**Output Shape Formula**
- [ ] Output = ⌊(Input + 2P − K) / S⌋ + 1
- [ ] Derive manually for different configurations

### Batch Normalization (Added)

- [ ] Why BatchNorm is used after convolutions
- [ ] Training vs inference behavior
- [ ] Layer Norm vs Batch Norm

### Activation Functions

- [ ] ReLU (dominant choice)
- [ ] Leaky ReLU
- [ ] GELU (used in modern architectures)

### Pooling Layers

**Max Pooling**
- [ ] Concept & output size calculation
- [ ] Keeps dominant feature

**Average Pooling**
- [ ] Concept & applications

**Global Average Pooling (GAP)**
- [ ] Replaces flatten + FC in modern architectures
- [ ] Why modern architectures prefer GAP

---

## Phase 4: CNN Architecture Flow

### Full Pipeline

Input Image → Convolution → BatchNorm → Activation → Pooling → (Repeat) → GAP → Fully Connected → Output

### Build First CNN

- [ ] MNIST digit classifier
- [ ] CIFAR-10 classifier
- [ ] Visualize predictions and errors

---

## Phase 5: CNN Training

### Dataset Handling

- [ ] Train / Validation / Test Split
- [ ] Batch loading with DataLoader
- [ ] Dataset class in PyTorch / TensorFlow

### Loss Functions

- [ ] Cross Entropy Loss (multi-class)
- [ ] Binary Cross Entropy (binary)
- [ ] Focal Loss (class imbalance)

### Optimization

- [ ] SGD with Momentum
- [ ] Adam / AdamW

### Learning Rate Techniques

- [ ] Step Decay
- [ ] Cosine Annealing
- [ ] Warmup (Added)

### Metrics

- [ ] Accuracy / Precision / Recall / F1 Score
- [ ] Top-5 Accuracy (Added — ImageNet metric)
- [ ] Confusion Matrix

---

## Phase 6: Understanding What CNNs Learn

### Visualizations

- [ ] Feature maps at each layer
- [ ] Activation maps
- [ ] Filter visualizations
- [ ] Grad-CAM (Added — visualize which regions influence prediction)
- [ ] Saliency Maps (Added)

### Layer-by-Layer Understanding

**Early Layers**
- [ ] Edges, corners, colors, textures

**Middle Layers**
- [ ] Shapes, patterns, object parts

**Deep Layers**
- [ ] Semantic features, high-level concepts

---

## Phase 7: Regularization

### Prevent Overfitting

- [ ] Dropout (spatial dropout for CNNs)
- [ ] Weight Decay (L2)
- [ ] Batch Normalization
- [ ] Early Stopping

### Data Augmentation

- [ ] Rotation / Flipping / Cropping / Scaling
- [ ] Color Jitter
- [ ] Cutout / CutMix / MixUp (Added — strong regularizers)
- [ ] AutoAugment (Added — learned augmentation policies)
- [ ] Test Time Augmentation (Added — TTA)

---

## Phase 8: Classic CNN Architectures

### LeNet (1998)

- [ ] Architecture overview
- [ ] Historical importance (first practical CNN)

### AlexNet (2012)

- [ ] Introduced ReLU at scale
- [ ] GPU training breakthrough
- [ ] Dropout for regularization

### VGG (2014)

- [ ] Deep stacks of 3×3 convolutions
- [ ] Simplicity and depth as design principles

### GoogLeNet / Inception (2014)

- [ ] Inception module
- [ ] 1×1 convolutions for dimensionality reduction

### ResNet (2015)

- [ ] Residual connections / skip connections
- [ ] Vanishing gradient solution
- [ ] Identity mapping

### DenseNet (2017)

- [ ] Dense connectivity (every layer connected to all subsequent)
- [ ] Feature reuse

### EfficientNet (2019)

- [ ] Compound scaling (width, depth, resolution together)
- [ ] NAS-designed baseline

### ConvNeXt (2022)

- [ ] CNN redesigned with Transformer design choices
- [ ] Competitive with ViT

### MobileNet (Added)

- [ ] Depthwise separable convolutions
- [ ] Designed for edge/mobile deployment

---

## Phase 9: CNN Internals

### Parameter Counting

- [ ] Count weights in a conv layer: K × K × C_in × C_out
- [ ] Count biases
- [ ] Count FC layer parameters

### Computational Cost

- [ ] FLOPs per layer
- [ ] MAC (Multiply-Accumulate) operations
- [ ] Total model FLOPs

### Memory Usage

- [ ] Activation memory during forward pass
- [ ] Weight memory
- [ ] Gradient memory during training

### Deep Dive

- [ ] Why CNNs are efficient vs FC networks
- [ ] Weight sharing benefits
- [ ] Sparse connectivity
- [ ] Receptive field concept (Added)
- [ ] Effective receptive field (Added)

---

## Phase 10: Backpropagation Through CNNs

### Gradient Flow

- [ ] Forward pass
- [ ] Loss computation
- [ ] Backward pass through each layer

### Convolution Backpropagation

- [ ] Kernel gradients (dL/dW)
- [ ] Input gradients (dL/dX)
- [ ] Weight updates

### Pooling Backpropagation

- [ ] Max Pooling: gradient flows to max position only
- [ ] Average Pooling: gradient distributed evenly

### Understand

- [ ] How gradients flow through skip connections
- [ ] Why ResNets train more stably

---

## Phase 11: CNN Implementation

### NumPy (From Scratch)

- [ ] Implement 2D convolution manually
- [ ] Implement max/average pooling manually
- [ ] Implement full forward pass

### Build CNN From Scratch (PyTorch)

- [ ] Custom Convolution layer
- [ ] Custom Pooling layer
- [ ] Custom Dense layer
- [ ] Full backward pass / backpropagation

---

## Phase 12: Transfer Learning

### Concepts

- [ ] Pretrained models (ImageNet weights)
- [ ] Feature extraction (freeze backbone, train head)
- [ ] Fine-tuning (unfreeze some or all layers)
- [ ] Domain adaptation (Added)

### Popular Pretrained Backbones

- [ ] ResNet family
- [ ] EfficientNet family
- [ ] ConvNeXt
- [ ] MobileNet (for edge)

### Understand

- [ ] When to fine-tune vs train from scratch
- [ ] How much data do you need for each strategy
- [ ] Learning rate differences for head vs backbone (Added)

---

## Phase 13: Object Detection

### Fundamentals

- [ ] Bounding boxes (x, y, w, h)
- [ ] IoU (Intersection over Union)
- [ ] NMS (Non-Maximum Suppression) (Added)
- [ ] mAP (mean Average Precision) (Added)

### Two-Stage Detectors

- [ ] R-CNN
- [ ] Fast R-CNN
- [ ] Faster R-CNN
- [ ] Region Proposal Networks (RPN) (Added)

### One-Stage Detectors

- [ ] YOLO (v1 → v8)
- [ ] SSD
- [ ] RetinaNet (Added — Focal Loss)
- [ ] FCOS (Added — anchor-free)

---

## Phase 14: Image Segmentation

### Semantic Segmentation

- [ ] Pixel-level classification
- [ ] Fully Convolutional Network (FCN)

### Instance Segmentation

- [ ] Object-wise segmentation

### Panoptic Segmentation (Added)

- [ ] Combines semantic + instance

### Architectures

- [ ] U-Net (skip connections for localization)
- [ ] Mask R-CNN
- [ ] DeepLab (Added — atrous convolutions)
- [ ] SegFormer (Added — transformer-based)

---

## Phase 15: Advanced CNN Topics

### Attention in CNNs

- [ ] SE Blocks (Squeeze-and-Excitation)
- [ ] CBAM (Convolutional Block Attention Module)
- [ ] Non-local Networks (Added)

### Vision Transformers (ViT)

- [ ] Why CNN limitations led to ViTs
- [ ] Patch embeddings
- [ ] Self-attention for vision
- [ ] Position embeddings

### Hybrid Architectures (Added)

- [ ] ConvNeXt (CNN with Transformer design)
- [ ] CvT (Convolutions in ViT)
- [ ] Swin Transformer (local window attention)

### CNN vs ViT

- [ ] Performance comparison on benchmarks
- [ ] Scaling behavior (ViT needs more data)
- [ ] Inductive biases: locality vs global attention
- [ ] Data efficiency: CNN wins on small data

---

## Phase 16: Production CNN Systems

### Deployment Formats

- [ ] ONNX (framework-agnostic)
- [ ] TorchScript (PyTorch)
- [ ] TensorRT (NVIDIA GPU optimized)
- [ ] CoreML (Added — Apple devices)
- [ ] TFLite (Added — mobile)

### Model Optimization

- [ ] Quantization (FP32 → INT8 / INT4)
- [ ] Pruning (structured & unstructured)
- [ ] Knowledge Distillation
- [ ] Layer fusion (Added)

### Serving

- [ ] FastAPI inference server
- [ ] Triton Inference Server (Added)
- [ ] Batching strategies (Added)

---

## Phase 17: GPU & CNN Internals

### CUDA Fundamentals

- [ ] CUDA cores & thread hierarchy
- [ ] GPU memory hierarchy (HBM, L2, shared memory, registers)
- [ ] Kernel execution model

### Deep Learning Libraries

- [ ] cuDNN (optimized conv kernels)
- [ ] Kernel fusion
- [ ] Winograd algorithm for convolutions (Added)

### Tensor Layouts

- [ ] NCHW (PyTorch default)
- [ ] NHWC (TensorFlow default, faster on some hardware)

### Performance Optimization

- [ ] Batch sizing
- [ ] Mixed precision training (FP16/BF16)
- [ ] Memory-efficient backpropagation (gradient checkpointing) (Added)

---

## Phase 18: Research-Level CNN Knowledge

### Landmark Papers

| Year | Paper |
|------|-------|
| 1998 | LeNet |
| 2012 | AlexNet |
| 2014 | VGG |
| 2014 | GoogLeNet / Inception |
| 2015 | ResNet |
| 2017 | DenseNet |
| 2019 | EfficientNet |
| 2020 | ViT (Vision Transformer) |
| 2022 | ConvNeXt |

### Research Skills

- [ ] Read CNN papers efficiently
- [ ] Reproduce architectures from scratch
- [ ] Implement from paper pseudocode
- [ ] Write clear experiment logs
- [ ] Ablation studies (Added)

---

## Projects

### Beginner

- [ ] MNIST digit classifier
- [ ] CIFAR-10 image classifier

### Intermediate

- [ ] Cat vs Dog classifier
- [ ] Fashion image classifier
- [ ] Transfer learning with ResNet

### Advanced

- [ ] Face mask detector
- [ ] Traffic sign classifier
- [ ] Medical image classifier (X-Ray, skin lesion)
- [ ] Real-time object detection (YOLO)

### Expert

- [ ] YOLO implementation from scratch
- [ ] U-Net implementation from scratch
- [ ] ResNet from scratch with full training
- [ ] CNN framework from scratch (NumPy only)
- [ ] Reproduce a CNN paper end-to-end (Added)

---

## Final Mastery

**Theory**
- [ ] Explain CNNs from first principles
- [ ] Derive convolution output shape formula
- [ ] Derive CNN backpropagation manually
- [ ] Explain why ResNets solve vanishing gradients

**Practical**
- [ ] Build CNN from scratch (NumPy + PyTorch)
- [ ] Train on custom datasets end-to-end
- [ ] Fine-tune pretrained models
- [ ] Deploy CNN to production

**Internals**
- [ ] Explain weight sharing & sparse connectivity
- [ ] Explain receptive field calculation
- [ ] Explain GPU acceleration for convolutions

**Expert**
- [ ] Implement ResNet manually
- [ ] Optimize CNN inference for edge devices
- [ ] Read CNN framework source code

---

## True Master Level

- [ ] Teach CNNs from first principles
- [ ] Build a CNN library from scratch
- [ ] Implement modern architectures (ConvNeXt, EfficientNet)
- [ ] Reproduce research papers end-to-end
- [ ] Optimize models for production and edge
- [ ] Contribute to computer vision frameworks
- [ ] Design new vision architectures
- [ ] Lead computer vision projects end-to-end
