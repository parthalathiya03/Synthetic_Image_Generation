# Synthetic_Image_Generation
Generate synthetic images using Stable Diffusion, perform basic image preprocessing, and set up a minimal Flux-based neural network to process an image (via a forward pass).


# Synthetic Image Generation, Preprocessing, and Flux Forward Pass

This project demonstrates a complete pipeline for generating synthetic images using Stable Diffusion, preprocessing those images, and running them through a simple Flux neural network model in Julia.

## Project Structure

```
project/
├── image_generation.py      # Python script for Stable Diffusion image generation
├── image_preprocessing.py   # Python script for image preprocessing
├── flux_forward_pass.jl     # Julia script for Flux model forward pass
├── images/                 # Directory for generated images
│   └── raw/                # Raw generated images
│   └── processed/          # Preprocessed images
└── README.md               # Project documentation (this file)
```

## Setup Instructions

### Option 1: Local Setup

#### Python Environment Setup (for image generation and preprocessing)

1. Create a new conda environment:
```bash
conda create -n image-gen python=3.8
conda activate image-gen
```

2. Install required packages:
```bash
pip install torch diffusers==0.15.0 transformers accelerate pillow matplotlib numpy
```

#### Julia Environment Setup (for Flux model)

1. Install Julia 1.9 or later from [julialang.org](https://julialang.org/downloads/)

2. Install required packages:
```julia
using Pkg
Pkg.add(["Flux", "Metalhead", "Images", "NPZ", "JSON", "Random", "Statistics", "BSON"])
```

### Option 2: Google Colab Setup

1. Create a new Google Colab notebook
2. Install Python dependencies:
```
!pip install diffusers==0.15.0 transformers accelerate pillow matplotlib numpy
```
