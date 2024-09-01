# Explanation of Bonus Part

Welcome to the `nn_multiplefilters.ipynb` notebook, a part of my submission for the "What the Hack" hackathon. This notebook demonstrates a comprehensive approach to applying multiple classical image filters using neural networks. It builds on the foundation of individual filter models to create a unified framework for edge detection and image enhancement.

## Notebook Overview

### Imports and Initial Setup
- Essential libraries such as TensorFlow, OpenCV, NumPy, and scikit-image are imported.
- Mixed precision training is enabled to boost performance.

### Filter Functions
- **Sobel Filter**: Applied to compute gradient magnitude in x and y directions.
- **Laplacian Filter**: Computes the Laplacian of the image to highlight areas of rapid intensity change.
- **Prewitt Filter**: Computes gradients using Prewitt operators for edge detection.

### Data Loading and Processing
- Images are loaded from a specified dataset path.
- Each image is processed using Sobel, Laplacian, and Prewitt filters.
- Images and their filtered counterparts are normalized and split into training, validation, and test sets.

### Model Definition
- The `create_improved_filter_model` function defines a CNN architecture designed to handle multiple filter types.
- The model includes downsampling, upsampling, and residual connections to capture and reconstruct filter-specific features.

### Training and Evaluation
- The model is trained for each filter type (Sobel, Laplacian, Prewitt) using the defined architecture.
- Training includes learning rate scheduling and early stopping.
- Training and validation losses are plotted.
- Models are evaluated on test data using metrics such as Mean Squared Error (MSE) and Mean Absolute Error (MAE).
- The Structural Similarity Index (SSIM) is calculated to assess the quality of filter application.

### Visualization
- Feature maps from various layers of the model are visualized to understand what features are learned at different stages.
- Sample images and their filter responses are displayed for analysis.

## How to Use

1. **Clone the Repository**: Ensure you have the repository cloned to your local environment.
2. **Install Dependencies**: Install the necessary libraries listed in the `requirements.txt` file.
3. **Open the Notebook**: Launch Jupyter Notebook or any compatible environment and open `nn_multiplefilters.ipynb`.
4. **Run the Notebook**: Execute the cells sequentially to load data, define the model, train it, and visualize results.

## Results
- Training plots for each filter type show the loss progression.
- Test performance metrics including MSE, MAE, and SSIM values are reported.
- Visualizations of feature maps and sample images are provided to illustrate the model's learned features and filter effectiveness.

## Conclusion

This notebook presents an advanced method for applying multiple image filters using neural networks. By integrating various filter types and leveraging modern deep learning techniques, it offers a robust approach to image enhancement and edge detection.
