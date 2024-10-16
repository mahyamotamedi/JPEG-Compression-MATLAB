# JPEG Compression and Decompression in MATLAB

## Overview
This project implements the JPEG compression algorithm in MATLAB, based on the example from Chapter 8 of the book **Digital Image Processing, Fourth Edition** by Rafael C. Gonzalez and Richard E. Woods. The goal is to simulate JPEG compression and decompression on an input image, with a user interface to display both the original and compressed images.

## Project Description
The project is divided into two main parts:
1. **JPEG Compression**: The input image is compressed using the JPEG algorithm, with quality parameters and compression rates taken into account.
2. **JPEG Decompression**: The compressed image is decompressed to reconstruct the original image as closely as possible, based on the compression settings.

## Methods
The JPEG algorithm follows these main steps:
1. **Color Space Conversion**: Converts the image from RGB to YCbCr color space.
2. **Discrete Cosine Transform (DCT)**: Applies DCT to each 8x8 block of the image to transform spatial data into frequency data.
3. **Quantization**: Compresses the data by reducing the precision of the less important frequencies.
4. **Encoding**: Uses Huffman encoding to further compress the quantized data.
5. **Decompression**: Applies the inverse of each step (i.e., inverse DCT, dequantization, and decoding) to reconstruct the image.

## User Interface
The project includes a user interface with the following features:
- **Image Display**: Allows users to load an input image and display both the original and compressed versions.
- **Quality Settings**: Users can adjust the quality parameter, which influences the compression rate and image quality.
- **Compression Rate Display**: The interface shows the compression ratio based on the selected quality settings.

## Results
The user can observe the trade-off between image quality and compression rate by adjusting the quality parameter. The compressed image can be viewed alongside the original to visually assess the differences caused by compression.

## Book Reference
- **Book Title**: Digital Image Processing, Fourth Edition  
- **Authors**: Rafael C. Gonzalez, Richard E. Woods  
- **Chapter 8**: JPEG Compression

## Conclusion
This project demonstrates how the JPEG compression algorithm works and allows users to interact with various quality and compression settings through a MATLAB-based user interface.

## Course
- **Course Title**: Digital Image Processing
