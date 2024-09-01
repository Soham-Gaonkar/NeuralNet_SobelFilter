# What the Hack: Neural Network Image Filtering

Welcome to the repository for my submission to the "What the Hack" hackathon! This project focuses on developing and training neural networks to apply classical image processing filters, specifically the Sobel, Laplacian, and Prewitt filters.

## Repository Structure

- **`optimisednnsobel.ipynb`**: This Jupyter notebook contains the code for a neural network specifically designed to learn and apply the Sobel filter to images. It includes data preprocessing, model architecture, training, and evaluation steps.

- **`nn-multiplefilters.ipynb`**: This Jupyter notebook extends the approach by training a neural network to apply multiple image filters, including Sobel, Laplacian, and Prewitt filters. The notebook also features visualization techniques to compare and analyze the representations learned by different layers of the CNN.

## Project Overview

### Dataset Preparation
- Original and Sobel-filtered image pairs were generated using a standard image processing library.
- These pairs serve as the training dataset, where the model learns to predict the Sobel-filtered image from the original input.

### Model Development
- A neural network architecture was designed to take original images as input and output Sobel-filtered images.
- For the `nn-multiplefilters.ipynb`, the model was extended to handle multiple filters.

### Training and Evaluation
- The models were trained on the prepared datasets and evaluated on a separate test set to measure their performance in replicating the classical image filters.

## How to Run

1. Clone the repository.
2. Install the required dependencies from `requirements.txt`.
3. Open the Jupyter notebooks in your environment.
4. Run the cells sequentially to train the models and visualize the results.

## Additional Details 

For more in-depth explanations and performance metrics, please refer to `DETAILS.md`.

Refer `BONUS.md` for explanation of the bonus part.

## Conclusion

This project demonstrates how neural networks can learn and replicate classical image processing filters. It extends beyond the basic Sobel filter to include multiple filters, providing a comprehensive approach to neural network-based image processing.

