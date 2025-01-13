# Multiscale Image Compression with Attention-Enhanced Discrete Cosine Transform Models

This repository contains the code, report, and presentation for the B.Tech Project "Multiscale Image Compression with Attention-Enhanced Discrete Cosine Transform Models". The project focuses on designing an efficient and effective deep learning-based image compression framework that achieves superior rate-distortion (R-D) performance with lower complexity.

## Project Structure
- **BTP Report.pdf**: The final project report detailing the problem statement, methodology, implementation, results, and conclusions.
- **BTP_B21CS055_B21AI026.pptx**: The presentation summarizing the project's key points, including an overview of the model, dataset, and performance comparison with traditional methods.
- **btp-submission-final.ipynb**: The Jupyter Notebook containing the implementation of the proposed model, including training, visualization, and evaluation.

## Abstract
Deep learning has revolutionized image compression, enabling better R-D performance compared to traditional methods like JPEG and JPEG2000. This project introduces a framework with the following innovations:

- **Multi-Frequency Channel Attention (MFCA)**: Enhances the model's ability to focus on important features by analyzing frequency components using the Discrete Cosine Transform (DCT).
- **Pyramid Multi-Convolution Network (PMCN)**: Captures multi-scale features for efficient compression and quality reconstruction.
- **Perceptual Quality Enhancement (PQF)**: Reduces quantization errors and improves visual quality.

The model is trained and evaluated on the Kodak dataset, achieving state-of-the-art results in terms of PSNR and SSIM with reduced complexity.

## Dataset
The Kodak dataset is used, containing 24 high-quality images at 768x512 resolution. Data preprocessing includes resizing to 384x384 and applying data augmentation (random flipping and cropping).

## Model Overview
- **Encoder**: Extracts a compact feature representation using MFCA and PMCN modules.
- **Quantization and Entropy Coding**: Compresses features for storage and transmission.
- **Decoder**: Reconstructs the image from compressed features using upsampling, PMCN blocks, and skip connections.
- **Loss Function**: Combines reconstruction, perceptual, rate, and quantization losses to optimize compression and quality.

## Results
- Achieves better PSNR and SSIM compared to JPEG and JPEG2000 at similar bit rates.
- Provides real-time suitability with lower encoding and decoding times.
- Visualizations demonstrate high-quality reconstruction and efficient bit allocation.

## Contributors
- **Kovidh Pothireddy** (B21AI026)
- **Oppangi Poojita** (B21CS055)
- **Supervisor: Prof. Binod Kumar**
