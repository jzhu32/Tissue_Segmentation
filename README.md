# Comparative Study: Spatial Transcriptomics and Computational Pathology

> **A Comparative Study of Spatial Transcriptomics and Cell-Type Segmentation in Histopathology**

## 📋 Project Overview

This project conducts a comprehensive comparison between computational pathology and spatial transcriptomics approaches for tissue characterization, with a focus on cell-type identification and mapping in histopathology samples. The study is divided into two complementary parts:

### Part 1: Cell Type Segmentation with SegPath
Development and optimization of deep learning models for cell-type segmentation in H&E-stained histopathology images, using immunofluorescence-based annotations from the SegPath dataset.

### Part 2: Integration with Spatial Transcriptomics
Comparison of morphology-based cell type predictions (using CellViT++) with spatial transcriptomics data, exploring the complementary information provided by both modalities.

### [View Presentation Slides](https://medcornell-my.sharepoint.com/:p:/r/personal/diz4009_med_cornell_edu/Documents/Presentations/ML_Imaging.pptx?d=wdb7b29bf15d8462cb555327a2e2b76bc&csf=1&web=1&e=jfczKE)

## 🌟 Key Features

- **Automated Architecture Discovery**: Systematic exploration of model architectures and hyperparameters using Optuna
- **Multi-Modal Integration**: Novel approach combining spatial transcriptomics with computational pathology
- **Optimized Cell-Type Segmentation**: Specialized models for epithelial, smooth muscle, lymphocyte, and myeloid cells
- **Advanced Training Pipeline**: Sophisticated data augmentation, ensemble modeling, and specialized loss functions

## 🏗️ Project Structure

```
.
├── SegPath/                    # Cell type segmentation models
│   └── src/                    # Source code for SegPath implementation
│       ├── 01_segmentation_sample.ipynb          # Preprocessing and mask filtering
│       ├── Train_Segmentation.ipynb              # Initial training implementation 
│       ├── Train_Segmentation_v2.ipynb           # Improved training pipeline
│       └── Train_Segmentation_v2_Optuna.ipynb    # Hyperparameter optimization
│
├── CellViT/                    # CellViT++ implementation
│   ├── src/                    # Source code
│   │   └── CellVIT.ipynb       # CellViT++ implementation notebook
│   ├── qupath/                 # QuPath project files
│   └── results_svs/            # GeoJSON results from CellViT analysis
│
└── Resources/                  # Research papers and documentation
    ├── SegPath.pdf             # SegPath paper
    └── CellViT.pdf             # CellViT paper
```

## 📓 Notebooks

### SegPath Implementation

1. **Preprocessing and Filtering**: 
   - [01_segmentation_sample.ipynb](SegPath/src/01_segmentation_sample.ipynb)
   - [Open in Google Colab](https://colab.research.google.com/drive/PLACEHOLDER_LINK)

2. **Initial Training Implementation**: 
   - [Train_Segmentation.ipynb](SegPath/src/Train_Segmentation.ipynb)
   - [Open in Google Colab](https://colab.research.google.com/drive/17KVaIeWIElx43Xj8OZkKZm8CwpMBMA9Y?usp=sharing)

3. **Improved Training Pipeline**: 
   - [Train_Segmentation_v2.ipynb](SegPath/src/Train_Segmentation_v2.ipynb)
   - [Open in Google Colab](https://colab.research.google.com/drive/1iczYDh8oOn3sK-tsCAO-qSerK7USWCBk?usp=sharing)

4. **Hyperparameter Optimization with Optuna**: 
   - [Train_Segmentation_v2_Optuna.ipynb](SegPath/src/Train_Segmentation_v2_Optuna.ipynb)
   - [Open in Google Colab](https://colab.research.google.com/drive/1IL207-HHmhvFMLws6fYaJkszxHS9O7n_?usp=sharing)

### CellViT Implementation

1. **CellViT Analysis Pipeline**: 
   - [CellVIT.ipynb](CellViT/src/CellVIT.ipynb)
   - [Open in Google Colab](https://colab.research.google.com/drive/1oId5T6ZvFMgIlfxKXr9oFxcCjwSIKHnV?usp=sharing)

## 📚 External Resources

- [SegPath Documentation](https://dakomura.github.io/SegPath/)
- [SegPath Paper](https://www.sciencedirect.com/science/article/pii/S2666389923000193) - "Restaining-based annotation for cancer histology segmentation to overcome annotation-related limitations among pathologists"
- [CellViT++ GitHub Repository](https://github.com/TIO-IKIM/CellViT-plus-plus/blob/main/README.md#examples)
- [CellViT Paper](https://www.sciencedirect.com/science/article/pii/S1361841524000689) - "CellViT++: Multi-level cell detection and classification in whole-slide images with vision transformers"

## 🚀 Setup and Usage

### Running the Code

- Use the provided Google Colab links for an environment with GPU support
- Each notebook contains detailed instructions on setup and execution

## 📋 Results

Segmentation results and GeoJSON outputs from CellViT analysis are available in the `CellViT/results_svs/` directory. For detailed model outputs, checkpoints, and raw data, please contact [diz4009@med.cornell.edu](mailto:diz4009@med.cornell.edu).

## 🔜 Future Work

- Direct correlation between segmentation results and spatial transcriptomics data
- Development of integrated predictive models
- Validation across multiple cancer types and datasets
- Exploration of attention mechanisms for improved feature localization

## 📬 Contact

For questions, data access, or collaboration opportunities:

- **Email**: [diz4009@med.cornell.edu](mailto:diz4009@med.cornell.edu)
- **GitHub Issues**: Feel free to open an issue in this repository
