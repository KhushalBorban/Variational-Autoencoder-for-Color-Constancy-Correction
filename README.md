# Variational-Autoencoder-for-Color-Constancy-Correction

Variational Autoencoder for Color Constancy Correction
This project implements a Variational Autoencoder (VAE) for correcting color distortions in images captured under varied illumination. The model learns robust latent representations that enable illumination-invariant image reconstruction, effectively restoring natural colors.

📌 Features

Variational Autoencoder Architecture: Encoder-decoder network with latent space regularization.
Color Constancy Correction: Restores original scene colors despite lighting variations.
Robust Evaluation: Image quality validated using PSNR and SSIM metrics.
Dataset: Optimized and tested on the CUBE+ dataset, a challenging benchmark for color constancy.
High Performance: Achieved 35.06 dB PSNR and 0.9739 SSIM at 500 training epochs.

🛠️ Methods & Workflow

Data Preprocessing
  Input: Raw images from CUBE+ dataset with varied lighting conditions.
  Normalization and resizing for efficient training.
Model Design
  Encoder: CNN layers compressing input into latent space.
  Latent Space: Mean & variance parameterization for VAE sampling.
  Decoder: CNN layers reconstructing illumination-corrected images.
Loss Function
  Reconstruction Loss (MSE for pixel fidelity).
  KL Divergence (regularizes latent space).
  Combined to train stable, robust VAE.
Training & Optimization
  Framework: PyTorch
  Optimizer: Adam
  Epochs: 500
  Batch normalization & dropout for regularization.

  📊 Results

  Quantitative Performance:
  PSNR: 35.06 dB
  SSIM: 0.9739
  Qualitative Results:
  Clear restoration of original colors across diverse lighting conditions.

  🎯 Applications

  Photography & Videography: Lighting-agnostic color correction.
  Computer Vision Preprocessing: Improved input consistency for downstream tasks.
  Autonomous Systems: Robust perception in varying illumination.

📖 References

  CUBE+ Dataset for Color Constancy
  Kingma, D.P., & Welling, M. (2013). Auto-Encoding Variational Bayes. arXiv:1312.6114
