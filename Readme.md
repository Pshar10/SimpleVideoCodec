# Simple Video Codec

This repository provides a simple video codec implementation using various video compression techniques, including color transformation, chroma downsampling, block-based Discrete Cosine Transform (DCT) with block sampling, and motion compensation.

## Overview

This codec aims to achieve efficient video compression by leveraging:
- **Color Transformation**: Converts RGB to YCbCr format, separating luminance and chrominance channels.
- **Chroma Downsampling**: Reduces color data to save space while maintaining visual quality.
- **Block-Based DCT**: Applies DCT on 8x8 blocks and selectively keeps coefficients.
- **Motion Compensation**: Uses a nearest-neighbor approach for detecting and encoding motion.

The codec follows a Group of Pictures (GoP) structure, consisting of Intra (I) frames and Predicted (P) frames.
## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Pshar10/SimpleVideoCodec.git
   cd SimpleVideoCodec
   ```

2. **Install Dependencies**:
   Use `pip` to install the required packages.
   ```bash
   pip install -r requirements.txt
   ```

3. **Prepare Video File**:
   - Place your input video as `videorec.mp4` in the main directory or modify paths in the notebook.

## Usage

### Encoding and Decoding Workflow

1. Run the Jupyter notebook `Simple_Video_Codec.ipynb` to encode and decode a video file.
2. The codec will:
   - **Encode** the video and save it as `encoded.pickle`.
   - **Decode** the compressed data and generate the video `decoded.mp4`.

### Performance Metrics

The notebook provides:
- **Compression Ratio**: Logarithmic ratio of decoded to encoded size.
- **SSIM (Structural Similarity Index)**: Quantitative measure of video quality.
- **Overall Performance**: Based on compression ratio and SSIM.

## Key Functions

- **encoder**: Compresses the video using color transformation, downsampling, DCT, and motion compensation.
- **decoder**: Reconstructs the video from the encoded data.
