# Marine Snow Removal Benchmarking Dataset

Welcome to the repository for **Marine Snow Removal Benchmarking Dataset** (**MSRB Dataset** in short).

<img src="img/174710351_orig.png" width=30%><img src="img/174710351_task1.png" width=30%><img src="img/174710351_task2.png" width=30%>

*An example from Marine Snow Removal Benchmarking Dataset. Left: Original underwater image. Middle: Synthesized image for Task 1, small-sized marine snow artifacts. Right: Synthesized image for Task 2, various-sized marine snow artifacts.*

Marine snow is one of the main degradation sources of underwater images that are caused by small particles, e.g., organic matter and sand, between the underwater scene and photosensors. We mathematically model two typical types of marine snow from the observations of real underwater images. The modeled artifacts are synthesized with underwater images to construct large-scale pairs of ground-truth and degraded images to calculate objective qualities for marine snow removal and to train a deep neural network.

## References
If you use MSRB Dataset in your paper, please cite the following paper.

[1] bluhbluhbluh

## Dataset Descriptions
MSRB Dataset has two sub-datasets:
- **MSR Task 1**: Removal of small-sized marine snow artifacts.
- **MSR Task 2**: Removal of various-sized marine snow artifacts.

Each sub-dataset corresponding to a MSR Task contains 2,300 training image pairs and 400 test image pairs, all having a pixel resolution of 384 x 384. An image pair contains one original underwater image and one image containing synthesized marine snow artifacts. Each synthesized image contains 100-600 marine snow particles.

All original images are collected from [flickr](https://www.flickr.com/) under a Creative Commons Attribution-NonCommercial-ShareAlike 2.0 Generic (CC BY-NC-SA 2.0) License.

### MSR Task 1
In Task 1, the maximum width/height of the artifacts is restricted to 6 pixels, which correspond to roughly 1.6% of the image width/height.

### MSR Task 2
The synthesized images for Task 2 have small- and large-sized marine snow artifacts. For large-sized artifacts, we set the largest width/height of marine snow to 32 pixels, which corresponds to 8.3% compared to the image width. Furthermore, the probabilities of small- and large-sized artifacts are set to 0.7 and 0.3, respectively.

## Downloading MSRB Dataset
You can download MSRB Dataset from this repository. The file is zipped. After unzipping, you can find MSRB1 and MSRB2 directories which correspond to the Tasks 1 and 2, respectively. There are training and test directories under MSRB1 and MSRB2.

## Examples from MSRB Dataset
The images below are examples from the test data of MSRB Dataset.

## MSR Benchmarking Results
The following tables are the current state-of-the-art results for marine snow removal. The average PSNRs/SSIMs are computed over the test datasets. If you would like to update the results, [please let us know](<mailto:ytnk@cc.tuat.ac.jp>)!

### MSR Task 1
|Method   | PSNR  | SSIM  |
|---|---|---|
|Median filter (kernel size 3x3)   |  28.55 | 0.846  |
|Median filter (kernel size 5x5)   |  25.98 | 0.711  |
|Adaptive median filter (kernel size 3x3)   | 29.88  | 0.910  |
|Adaptive median filter (kernel size 5x5)   | 28.08  | 0.861  |
|U-Net   | **36.82**  | **0.978**  |
|Synthesized image   | 32.20  | 0.945  |


### MSR Task 2
|Method   | PSNR  | SSIM  |
|---|---|---|
|Median filter (kernel size 3x3)   |22.81   | 0.770  |
|Median filter (kernel size 5x5)   |21.93   | 0.645  |
|Adaptive median filter (kernel size 3x3)   | 23.35  | 0.842  |
|Adaptive median filter (kernel size 5x5)   | 22.83  | 0.794  |
|U-Net   | **30.95**  | **0.932**  |
|Synthesized image   | 23.83  | 0.876  |

### Restoration Results

## Copyright
Copyright (c) 2020 Yuya Sato, Takumi Ueda, and Yuichi Tanaka.

We would like to thank all users on flickr who made original underwater images available under the CC BY-NC-SA 2.0 license. Credits of all the images in MSRB Dataset are available in this repository through xxxx. Please let us know if you have any questions and comments on this dataset.