# Dynamic Pricing Model for Parking Lots

This project implements and compares different pricing strategies for dynamically adjusting parking lot prices based on occupancy data. The goal is to simulate and evaluate the impact of dynamic pricing in smart cities using real-world-like data.

## 📊 Project Overview

The notebook includes:
- Data exploration and preprocessing of occupancy and timestamp data.
- A simple baseline dynamic pricing model.
- Visualization of pricing trends based on occupancy changes.
- Simulation of price changes over time using a linear adjustment formula.

## 🧠 Features

- Loads and processes occupancy data with timestamps.
- Implements a simple dynamic pricing algorithm:
  ```
  new_price = prev_price + alpha * (occupancy / capacity)
  ```
- Visualizes computed prices over time for a selected parking lot.
- Uses Matplotlib for time series visualizations.

## 🗃 Dataset

The dataset appears to be CSV-based and includes:
- `SystemCodeNumber` (Lot ID)
- `LastUpdatedDate`, `LastUpdatedTime`
- `Occupancy`, `Capacity`

Loaded from Google Drive:
```python
df = pd.read_csv("/content/drive/My Drive/Colab Notebooks/capstone project/dataset.csv")
```

## 📦 Requirements

This project is run on Google Colab and uses:

- Python 3.x
- pandas
- matplotlib

To run locally:
```bash
pip install pandas matplotlib
```

## 🚀 How to Run

1. Upload the notebook to Google Colab or run it in a Jupyter environment.
2. Mount Google Drive to access the dataset (or update path).
3. Run each cell to preprocess data, apply the pricing model, and generate visualizations.

## 📈 Sample Output

- Time series plots showing how prices adapt over time.
- Tabular output of computed prices with date and occupancy context.

## ✍️ Author

- Prateek Verma

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
