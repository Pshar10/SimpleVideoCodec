# Simple Video Codec Project

This repository contains a basic implementation of a video codec, developed to demonstrate video compression and decompression techniques. The project includes modules for encoding, decoding, and processing video files using custom algorithms and standard compression techniques.

## Project Structure

```
SimpleVideoCodec/
├── data/                   # Directory for storing video files for encoding/decoding
├── notebooks/              # Jupyter notebooks for video processing exploration
├── src/                    # Source code for codec implementation
│   ├── encoder/            # Video encoding scripts and algorithms
│   ├── decoder/            # Video decoding scripts and algorithms
│   ├── utils/              # Utility functions for video manipulation
├── requirements.txt        # Python dependencies
├── README.md               # Project description and usage guide
└── main.py                 # Main script to run the codec
```

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

3. **Prepare Video Files**:
   - Place your input video files in the `data/` directory or use the provided utility scripts in `src/utils/` to load and preprocess videos.

## Usage

### Encoding a Video
To encode a video file, run:
```bash
python main.py --encode path/to/video.mp4
```

### Decoding a Video
To decode an encoded video file, use:
```bash
python main.py --decode path/to/encoded_file
```

### Jupyter Notebooks
The `notebooks/` directory contains interactive notebooks for experimenting with encoding and decoding parameters, analyzing compression ratios, and visualizing results.

## Key Modules

- **Encoder**: Modules for compressing video files using various encoding schemes.
- **Decoder**: Modules for decompressing and reconstructing video files.
- **Utilities**: Helper functions for video handling, format conversion, and frame manipulation.

## Contributing
Contributions are welcome! Feel free to open issues or submit pull requests to improve the codec or add new features.

