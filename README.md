# Synthetic Landslide Stability Dataset

This project generates a synthetic dataset to simulate conditions related to landslide stability using topographic and soil data. It also includes a neural network model for binary classification (stable vs. unstable terrain) and exports the generated dataset to an Excel file.

## 📁 Files Included

- `synthetic_landslide_data.xlsx`: The generated dataset with 1,000 samples.
- `landslope_model.py`: Python script for data generation, preprocessing, training, evaluation, and exporting.
- `README.md`: This documentation file.

## 📊 Dataset Description

Each row in the dataset represents a synthetic sample of terrain, with the following features:

| Feature         | Description                               |
|-----------------|-------------------------------------------|
| Elevation       | Elevation of the terrain (in meters)      |
| Slope           | Slope in degrees                          |
| Aspect          | Aspect direction in degrees               |
| Soil_Moisture   | Percentage of soil moisture               |
| Cohesion        | Soil cohesion (synthetic units)           |
| Stability       | Target label (1 = stable, 0 = unstable)   |

The `Stability` is determined based on a synthetic rule:
Stability = 1 if (Elevation + Slope + Cohesion) > 150 else 0



## 🤖 Machine Learning Model

- Framework: TensorFlow/Keras
- Model: Feedforward neural network
- Hidden Layers: 2 (128 and 64 neurons)
- Output: Binary classification (sigmoid activation)
- Loss: Binary Crossentropy
- Optimizer: Adam

## 📦 Requirements

Install dependencies with:

```bash
pip install numpy pandas scikit-learn tensorflow openpyxl
🚀 Usage
Run the Python script to:

Generate the synthetic dataset.

Preprocess and split the data.

Train a neural network.

Evaluate model performance.

Export the dataset to Excel.

📬 Contact
Tarinabo williamtarinabo@gmail.com
