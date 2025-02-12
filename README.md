
# 3D Point Cloud Generation using TransGAN

## Overview
This project presents the first-ever implementation of TransGAN for 3D Point Cloud Generation, pushing the boundaries of transformer-based generative models into 3D space. The goal is to generate high-fidelity 3D point clouds with improved structural accuracy and scalability.

## Directory Structure
```
Trans-GAN-main
├── Point_Sample_From_Mesh
│   ├── meshtopc.py
│   ├── meshtopc.pyc
│   ├── modelnet_mesh_to_pointcloud.py
│   └── view_pointcloud.py
├── data
│   └── ModelNet10
│       ├── bathtub
│       │   ├── train
│       │   └── test
│       └── ... other classes
└── TransGAN_PointCloud_Notebook.ipynb
```

## Dataset Preparation
1. **Download ModelNet10 Dataset:**  
   Download the ModelNet10 dataset and place it in the `data/ModelNet10` directory.

2. **Convert Mesh Files to Point Cloud (.npy format):**  
   Use the scripts in the `Point_Sample_From_Mesh` folder to convert the dataset:
   ```bash
   python Point_Sample_From_Mesh/modelnet_mesh_to_pointcloud.py
   ```
   This will generate `.npy` files for point cloud data, required for training the model.

## Usage
Simply open the Jupyter Notebook and run the cells in sequence:

```bash
jupyter notebook TransGAN_PointCloud_Notebook.ipynb
```

## Key Features
- First-of-its-kind application of TransGAN in 3D point cloud generation.
- Transformer-based architecture for enhanced performance on complex 3D data.
- Focused on structural accuracy and efficient model refinement.

## Current Status
- The model currently generates **rough structures** of 3D point clouds.
- Work is in progress to improve the quality, accuracy, and finer details of the generated outputs.

## Work in Progress
- Ongoing improvements in model refinement and performance optimization.
- Experimenting with different hyperparameters and architectural adjustments.
- Future integration of more robust datasets and evaluation metrics.
