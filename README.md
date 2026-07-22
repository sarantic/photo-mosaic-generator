# Photo Mosaic Generator

A Python project that generates photo mosaics by reconstructing a target image using thousands of smaller images selected according to color similarity. The project demonstrates image processing, color analysis, and algorithmic matching techniques.

## Project Overview

Photo mosaics recreate an image by replacing small regions with photographs that closely match the original colors. This project processes a collection of tile images, computes average RGB values, and selects the closest matching tile for every region of the target image to generate a complete mosaic.

## Features

- Image loading and preprocessing
- RGB color extraction
- Average color computation
- Tile image matching
- Mosaic image generation
- Support for custom image collections
- Image resizing and preprocessing utilities

## Technologies

- Python
- pandas
- NumPy
- Pillow (PIL)
- Jupyter Notebook

## Repository Structure

```text
.
├── notebooks/
│   ├── photo_mosaic_generator.ipynb
│   └── image_preprocessing.ipynb
├── src/
│   ├── DISCOVERY.py
│   └── instagram.py
├── images/
├── README.md
├── .gitignore
└── requirements.txt
```

## Inputs

The mosaic generator uses:

- Target image
- Tile image library
- Average RGB color values
- Tile dimensions

## Objective

Generate a photo mosaic by replacing regions of a target image with visually similar tile images based on average color similarity.

## Future Improvements

- Compare alternative color distance metrics (Lab color space, CIEDE2000)
- Parallelize tile matching for improved performance
- Prevent duplicate tile usage
- Build a graphical user interface
- Support variable tile sizes and higher-resolution mosaics
