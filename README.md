# Marine Snow Removal Benchmarking Dataset
Welcome to the repository for Marine Snow Removal Benchmarking Dataset (MSRB Dataset in short).

Marine snow is one of the main degradation sources of underwater images that are caused by small particles, e.g., organic matter and sand, between the underwater scene and photosensors. We mathematically model two typical types of marine snow from the observations of real underwater images. The modeled artifacts are synthesized with underwater images to construct large-scale pairs of ground-truth and degraded images to calculate objective qualities for marine snow removal and to train a deep neural network.

## References
If you use the MSRB Dataset, please refer to the following paper.

## Dataset Descriptions
MSRB Dataset has two sub-datasets:
- MSR Task 1: Removal of small-sized marine snow artifacts.
- MSR Task 2: Removal of various-sized marine snow artifacts.

Each sub-dataset corresponding to a MSR Task contains 2,300 training image pairs and 400 test image pairs, all having a pixel resolution of 384 x 384. An image pair contains one original underwater image and one image containing synthesized marine snow artifacts. Each synthesized image contains 100--600 marine snow particles.

All original images are collected from [flickr](https://www.flickr.com/) under a Creative Commons Attribution-NonCommercial-ShareAlike 2.0 Generic (CC BY-NC-SA 2.0) License.

### MSR Task 1
In Task 1, the maximum width/height of the artifacts is restricted to 6 pixels, which correspond to roughly 1.6% of the image width/height.

## MSR Task 2
The synthesized images for Task 2 have small- and large-sized marine snow artifacts. For large-sized artifacts, we set the largest width/height of marine snow to 32 pixels, which corresponds to 8.3% compared to the image width. Furthermore, the probabilities of small- and large-sized artifacts are set to 0.7 and 0.3, respectively.

## Downloading MSRB Dataset


## Examples from MSRB Dataset


## MSR Benchmarking Results
