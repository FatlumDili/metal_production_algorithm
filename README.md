Last updated: Mon Nov  3 12:37:28 UTC 2025

Last updated: Sun Nov  2 12:31:04 UTC 2025

Last updated: Sat Nov  1 12:31:36 UTC 2025

Last updated: Fri Oct 31 12:36:30 UTC 2025

Last updated: Thu Oct 30 12:36:33 UTC 2025

Last updated: Wed Oct 29 12:37:22 UTC 2025

Last updated: Tue Oct 28 12:36:10 UTC 2025

Last updated: Mon Oct 27 12:37:45 UTC 2025

Last updated: Sun Oct 26 12:31:58 UTC 2025

Last updated: Sat Oct 25 12:31:32 UTC 2025

Last updated: Fri Oct 24 12:37:07 UTC 2025

Last updated: Thu Oct 23 12:37:20 UTC 2025

Last updated: Wed Oct 22 12:37:26 UTC 2025

Last updated: Tue Oct 21 12:37:02 UTC 2025

Last updated: Mon Oct 20 12:36:37 UTC 2025

Last updated: Sun Oct 19 12:31:26 UTC 2025

Last updated: Sat Oct 18 12:31:28 UTC 2025

Last updated: Fri Oct 17 12:35:34 UTC 2025

Last updated: Thu Oct 16 12:37:07 UTC 2025

Last updated: Wed Oct 15 12:37:11 UTC 2025

Last updated: Tue Oct 14 12:37:19 UTC 2025

Last updated: Mon Oct 13 12:35:37 UTC 2025

Last updated: Sun Oct 12 12:30:57 UTC 2025

Last updated: Sat Oct 11 12:30:18 UTC 2025

Last updated: Fri Oct 10 12:35:19 UTC 2025

Last updated: Thu Oct  9 12:35:48 UTC 2025

Last updated: Wed Oct  8 12:35:59 UTC 2025

Last updated: Tue Oct  7 12:35:51 UTC 2025

Last updated: Mon Oct  6 12:35:44 UTC 2025

Last updated: Sun Oct  5 12:30:36 UTC 2025

Last updated: Sat Oct  4 12:30:18 UTC 2025

Last updated: Fri Oct  3 12:33:43 UTC 2025

Last updated: Thu Oct  2 12:33:18 UTC 2025

Last updated: Wed Oct  1 12:36:44 UTC 2025

Last updated: Tue Sep 30 12:36:40 UTC 2025

Last updated: Mon Sep 29 12:36:03 UTC 2025

Last updated: Sun Sep 28 12:30:53 UTC 2025

Last updated: Sat Sep 27 12:30:26 UTC 2025

Last updated: Fri Sep 26 12:35:05 UTC 2025

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
