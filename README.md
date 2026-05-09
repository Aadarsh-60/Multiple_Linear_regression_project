
# Multiple Linear Regression Project

This project demonstrates a multiple linear regression workflow using the California Housing dataset from `scikit-learn`.

The notebook covers:

- Loading the California Housing dataset
- Creating a Pandas DataFrame for exploration
- Visualizing feature relationships with Seaborn and Matplotlib
- Splitting the data into training and testing sets
- Scaling features with `StandardScaler`
- Training a `LinearRegression` model
- Evaluating the model with MAE, MSE, RMSE, and R2 score
- Saving and loading the trained model with `pickle`

## Project Files

```text
.
├── 4.0-Multiple+Linear+Regression.ipynb
├── regressor.pkl
├── README.md
└── .gitignore
```

- `4.0-Multiple+Linear+Regression.ipynb`: Main Jupyter notebook for data loading, training, evaluation, and model serialization.
- `regressor.pkl`: Saved trained regression model generated from the notebook.

## Requirements

Install the required Python packages:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

## How to Run

Start Jupyter Notebook from this project folder:

```bash
jupyter notebook
```

Then open:

```text
4.0-Multiple+Linear+Regression.ipynb
```

Run the notebook cells from top to bottom. The dataset is loaded through `sklearn.datasets.fetch_california_housing`, so no local dataset file is required.

## Model Output

The notebook saves the trained model as:

```text
regressor.pkl
```

You can load it in Python with:

```python
import pickle

model = pickle.load(open("regressor.pkl", "rb"))
```
