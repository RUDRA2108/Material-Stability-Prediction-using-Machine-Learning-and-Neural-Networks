---

# Material Stability Prediction using Machine Learning and Neural Networks

## Project Overview

This project aims to predict the stability of materials based on their properties using various machine learning algorithms and neural network architectures. The dataset includes properties such as band gap, total magnetization, elasticity, and formation energy, which are used as features to predict the target variable, `e_above_hull`, a measure of material stability.

## Dataset

The dataset contains the following columns:

- `material_id`: Unique identifier for each material
- `pretty_formula`: Chemical formula of the material
- `e_above_hull`: Target variable, a measure of material stability
- `band_gap`: Band gap energy of the material
- `total_magnetization`: Total magnetization of the material
- `elasticity.elastic_anisotropy`: Elastic anisotropy
- `elasticity.K_VRH`: Bulk modulus
- `elasticity.G_VRH`: Shear modulus
- `energy`: Total energy
- `energy_per_atom`: Energy per atom
- `formation_energy_per_atom`: Formation energy per atom

## Exploratory Data Analysis (EDA)

EDA was conducted to understand the distribution of features, identify correlations, and visualize relationships between features and the target variable. Key steps included:

- Checking for missing values and handling them
- Visualizing distributions of numerical features
- Plotting correlation matrix
- Creating pair plots and scatter plots

## Models and Results

Several machine learning models and neural networks were trained and evaluated:

1. **Simple Neural Network**
2. **Deep Neural Network**
3. **Wide and Deep Neural Network**
4. **Linear Regression**
5. **Decision Tree**
6. **Random Forest**
7. **Gradient Boosting**

### Performance Metrics

- **Root Mean Squared Error (RMSE)**
- **Mean Absolute Error (MAE)**
- **R² Score**

### Results

| Model                 | RMSE   | MAE    | R² (%) |
|-----------------------|--------|--------|--------|
| Simple NN             | 0.1354 | 0.0724 | 90.04  |
| Deep NN               | 0.1270 | 0.0639 | 91.25  |
| Wide and Deep NN      | 0.1285 | 0.0698 | 91.04  |
| Linear Regression     | 0.3657 | 0.2238 | 27.38  |
| Decision Tree         | 0.1699 | 0.0723 | 84.34  |
| Random Forest         | 0.1207 | 0.0586 | 92.10  |
| Gradient Boosting     | 0.1314 | 0.0711 | 90.62  |

### Conclusion

- **Best Model**: The Random Forest model outperformed all other models with the lowest RMSE (0.1207), lowest MAE (0.0586), and highest R² score (92.10%).
- **Neural Networks**: Deep Neural Networks showed strong performance, indicating their capability to model complex relationships in the data.
- **Linear Models**: Linear Regression performed poorly, suggesting that the relationship between features and the target variable is non-linear.

## Installation and Usage

### Prerequisites

- Python 3.6+
- TensorFlow 2.x
- Scikit-learn
- Pandas
- Matplotlib
- Seaborn

### Installation

Clone the repository:
```bash
git clone [https://github.com/RUDRA2108/Material-Stability-Prediction-using-Machine-Learning-and-Neural-Networks.git]
```

Install the required packages:
```bash
pip install -r requirements.txt
```

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---
