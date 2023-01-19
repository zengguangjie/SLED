# SLED
Unsupervised Skin Lesion Segmentation via Structural Entropy Minimization on Multi-Scale Superpixel Graphs

# Installation
Install the required packages listed in the file ```requirement.txt```. The code has been tested on Python 3.10.6.

# Usage
In the root directory of this project:
```
python main.py [-h] [--dataset DATASET]
               [--slic_compactness COMPACTNESS]
               [--self_tuning_k SELF_TUNING_K] [--centroid_thresh CENTROID_THRESH]
               [--outlier_detection OUTLIER_DETECTION] [--contamination CONTAMINATION]
```

example: ```python main.py --dataset PH2```
```
optional arguments:
  -h                    show this help message and exit
  --dataset DATASET     name of dataset (default: PH2)
  --slic_compactness SLIC_COMPACTNESS    
                        compactness of SLIC superpixel algorithm (default: 10)
  --self_tuning_k SELF_TUNING_K          
                        K for self tuning scaling parameters in graph construction (default: 30)
  --centroid_thresh CENTROID_THRESH      
                        r for centroid thresh in graph construction (default:0.3)
  --outlier_detection OUTLIER_DETECTION  
                        outlier detection method in multi-scale mechanism (default: IFOREST)
  --contamination CONTAMINATION          
                        contamination for outlier detection methods (default: 0.1)
  ```
