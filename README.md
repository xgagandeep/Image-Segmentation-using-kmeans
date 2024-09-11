

# Image Segmentation using KMeans

**Repository:** [xgagandeep/Image-Segmentation-using-Kmeans](https://github.com/xgagandeep/Image-Segmentation-using-Kmeans)  
**Date:** 2020  
**Language:** Python  
**Libraries:** NumPy, OpenCV, Matplotlib, Scikit-learn

## Description

This project demonstrates image segmentation using the KMeans clustering algorithm. The notebook performs color-based segmentation on an image by clustering pixel colors and then reconstructing the image based on the dominant colors identified by KMeans.

## Features

- **Image Loading:** Reads and preprocesses the image.
- **Pixel Flattening:** Reshapes the image into a 2D array where each row represents a pixel's RGB values.
- **KMeans Clustering:** Applies KMeans to segment the image into a specified number of color clusters.
- **Color Visualization:** Displays the dominant colors identified by KMeans.
- **Image Reconstruction:** Reconstructs and visualizes the segmented image based on the dominant colors.

## Files

- **`Image Segmentation.ipynb`:** Jupyter Notebook containing the implementation of image segmentation using KMeans.

## Installation

To run this project, you need Python and the required libraries installed. Follow these steps:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/xgagandeep/Image-Segmentation-using-Kmeans.git
   ```

2. **Navigate to the project directory:**

   ```bash
   cd Image-Segmentation-using-Kmeans
   ```

3. **Install the required libraries:**

   ```bash
   pip install numpy opencv-python matplotlib scikit-learn
   ```

4. **Run the Jupyter Notebook:**

   ```bash
   jupyter notebook Image\ Segmentation.ipynb
   ```

## Usage

1. **Image Reading:** The image is loaded and converted to RGB format for processing.
2. **Pixel Flattening:** The image is reshaped into a 2D array of RGB values.
3. **KMeans Clustering:**
   - Define the number of dominant colors (clusters).
   - Apply KMeans clustering to the pixel data.
   - Retrieve cluster centers (dominant colors).
4. **Color Visualization:** Display the dominant colors as color swatches.
5. **Image Reconstruction:**
   - Assign each pixel to the nearest cluster center.
   - Reconstruct the image using the dominant colors.
   - Display the segmented image.

## Functions

- **`cv2.imread(path)`**: Reads the image from the specified path.
- **`cv2.cvtColor(img, cv2.COLOR_BGR2RGB)`**: Converts the image from BGR to RGB format.
- **`reshape((-1, 3))`**: Flattens the image into a 2D array of RGB values.
- **`KMeans(n_clusters)`**: Applies KMeans clustering to the pixel data.
- **`plt.imshow(image)`**: Displays images and color swatches.

## Example

The notebook demonstrates segmentation on a sample image. You can modify the `dominant_colors` variable to change the number of clusters for segmentation and visualize how different numbers of colors affect the segmentation results.

## Contribution

Feel free to contribute to this project by submitting issues or pull requests. For any questions or feedback, please open an issue on the GitHub repository.
