# BrainVAE

This project demonstrates a Variational Autoencoder (VAE) implementation in PyTorch designed to understand and recreate medical images.

## Project Goal

The objective was to train a VAE on brain CT scan images from the [DeepStroke dataset](https://www.kaggle.com/datasets/huseyincavus/deepstroke). The goal was enabling the AI model to learn a smooth, organized "map" (hidden space) of the data in order to explore changes between different brain slice images.

## Implementation Process

1. **Data Loading:** The complete [DeepStroke dataset](https://www.kaggle.com/datasets/huseyincavus/deepstroke) containing normal and abnormal brain CT scans was loaded.
2. **Training Configuration:** A custom VAE underwent training across multiple GPUs, with model and data batch sizes optimized for maximum hardware utilization.
3. **Space Interpolation:** The trained model generated smooth, multi-step transitions between different real scans, demonstrating the learned hidden space structure.

## Results Achieved

The VAE learned a smooth representation of the training data. The hidden space enables realistic anatomical transitions between images, demonstrating deeper "knowledge" of the data beyond simple generation.

## License

This project is licensed under the MIT License. See the **LICENSE** file for details.
