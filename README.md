# <center>Deep Learning Project</center>

<center>
Master in Data Science and Advanced Analytics <br>
NOVA Information Management School
</center>

** **

<center>
David Vieira
Jan-Louis Schneider <br>
Emir Kamiloglu <br>
Marta Boavida <br>
Sofia Gomes <br>
</center>

** **

## Animal Family Classification 

Deep learning project to classify images into **animal families** using a highly imbalanced dataset:
**11,983 images** across **202 classes**.  
Built a robust training pipeline with **outlier filtering (CLIP)**, **data augmentation**, and **transfer learning**.

### Highlights
- Challenging setup: 202 classes with severe class imbalance.
- Preprocessing pipeline:
  - dataset inspection + cleaning
  - outlier detection/removal using **CLIP**
  - class-balancing augmentation with **Albumentations**
- Model benchmarking in **PyTorch**:
  - custom CNN baselines
  - transfer learning with **ResNet50** and **VGG16**
- Best model: **ResNet50**
  - **Macro F1:** 45.78%
  - **Accuracy:** 48.98%
  - **Top-3 accuracy:** 68%

### Repository contents
This repository is notebook-driven. Recommended execution order:

1. `01_EDA.ipynb` — dataset exploration, class distribution, initial insights  
2. `02_preprocessing.ipynb` — cleaning + CLIP-based outlier filtering + augmentation setup  
3. `03_models.ipynb` — model training/benchmarking (CNN baselines + ResNet50/VGG16)  
4. `04_results_and_visualizations.ipynb` — evaluation, metrics, and result plots  

Additional:
- `preprocessing_testing.ipynb` — auxiliary experiments / preprocessing checks

### Data
The dataset was provided in an academic context and may not be included in this repository.
To reproduce results, place the dataset in a local folder and update the paths referenced in the notebooks.


