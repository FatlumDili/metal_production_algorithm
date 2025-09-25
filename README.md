Last updated: Thu Sep 25 12:35:47 UTC 2025

Last updated: Wed Sep 24 12:35:00 UTC 2025

Last updated: Tue Sep 23 12:34:27 UTC 2025

Last updated: Mon Sep 22 17:42:16 UTC 2025

# Metal Production Optimization

This project implements a mock metal production scheduling system for mid-sized manufacturing companies, specifically in the automotive and aviation sectors. It combines machine learning and linear programming to optimize order fulfillment.

## Features

- Mock order and machine datasets to simulate realistic production scenarios
- ML-predicted late orders to prioritize scheduling
- Sequential Linear Programming (LP) optimization to minimize lateness
- Batch processing for efficiency and scalability
- Optimized start/finish times per order with weighted prioritization

## Dataset

- `mock_data.csv` contains the mock order, machine, and material data used in the project
- Column examples: OrderID, Product, Quantity, OrderDate, DeliveryTime_days, Priority, MachineID, ProcessTime_hr, PredictedLate
- **Note:** All data is simulated for demonstration purposes

## Usage

1. Open jobshop_notebook.ipynb in Jupyter Notebook
2. Run all cells sequentially from top to bottom
3. The notebook includes:
   - Data generation and checks
   - Feature generation for ML prediction
   - ML model training and predictions
   - Sequential LP optimization for order scheduling
   - Visualizations of optimized orders

## Dependencies

- Python 3.10+
- pandas
- numpy
- scikit-learn
- pulp
- matplotlib
- seaborn

Install dependencies via:

```bash
pip install -r requirements.txt

## Notes 

- Solver times gro with the increase of orders and machines
- All data is mock-generated to simulate real processes, however it may not reflect real production environments
- The project is intended for educational and prototyping purposes
