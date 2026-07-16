# Proyecto-de-Investigacion
Modelo de Deep Learning para la personalización automática de prótesis pasivas impresas en 3D a partir de imágenes medicas
# 3D Prosthesis Research Repository

This repository contains source code and dataset files for a 3D prosthesis research project.
The code includes dataset preprocessing, U-Net training, STL generation, and academic figure creation.

## Key Files

- `generate_academic_figures.py`: Generates high-resolution English figures from the dataset.
- `source_images/`: Original healthy and amputated medical images.
- `PREPROCESADAS/`: Preprocessed images ready for model use.
- `unet_model.py`: U-Net model definition.
- `train_unet.py`, `train_unet_split.py`: Training scripts for segmentation.
- `organize_medical_dataset.py`: Dataset organization utilities.
- `visualize_dataset.py`: Dataset visualization utilities.

## Setup

1. Create or activate your Python environment.
2. Install dependencies:

```bash
python -m pip install -r requirements.txt
```

## Generate High-Quality English Figures

Run:

```bash
python generate_academic_figures.py --output-folder figures --project-root . --dpi 300
```

This will create a `figures/` folder with 8 publication-ready PNG images.

## Notes

- The dataset is already available in `source_images/sano`, `source_images/amputado`, and `PREPROCESADAS`.
- The `.gitignore` file excludes the local Python environment and temporary build artifacts.
