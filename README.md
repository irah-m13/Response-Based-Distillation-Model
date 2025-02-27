# Response-Based Knowledge Distillation on CIFAR-10

This project demonstrates **response-based knowledge distillation** using PyTorch on the CIFAR-10 dataset. It involves training a larger **teacher model** and then distilling its knowledge to a smaller **student model**, which learns from the teacher's softened output probabilities. This technique is useful for compressing models while retaining much of their accuracy, making them suitable for deployment on resource-constrained devices.

---

## Project Overview

- **Teacher Model**: A convolutional neural network (CNN) trained on CIFAR-10.
- **Student Model**: A smaller CNN that learns from the teacher's softened outputs via knowledge distillation.
- **Dataset**: CIFAR-10, downloaded from an S3 bucket and extracted locally.

---

## Prerequisites

The CIFAR-10 dataset - From Kaggle

To run this project, you need the following software and libraries:

- Python 3.x
- PyTorch
- torchvision
- boto3 (for downloading the dataset from S3)
- pandas
- PIL (Pillow)
- py7zr (for extracting .7z files)

You can install the required libraries using pip:

```bash
pip install torch torchvision boto3 pandas pillow py7zr
