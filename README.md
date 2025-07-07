# Model 1 – Linear Pricing Strategy

This notebook implements a basic **linear dynamic pricing model** based on occupancy and queue length using a fixed mathematical formula.

The pricing is derived from a formula:
price = BASE_PRICE + α * occupancy_ratio + β * queue_length

- **Base Price:** $10.00  
- **Occupancy Ratio:** Occupancy / Capacity  
- **α (Alpha):** 8.0  
- **β (Queue Weight):** 0.5

- Calculates a **target price** using a simple linear equation.
- Computes **Mean Absolute Error (MAE)**.
- Visualizes predicted vs. actual price performance (if included).

  # Model 2 – AI-Based Dynamic Pricing with XGBoost

This notebook builds an **advanced dynamic pricing model** using **XGBoost**, driven by a **mathematical demand function** and real-time features like time, traffic, and vehicle type.

The model calculates a **demand factor** influenced by:

- Occupancy ratio
- Queue length
- Traffic conditions
- Day of the week
- Hour of the day
- Vehicle type
- Special days

The target price is:


1. Load the dataset `dataset.csv`.
2. Run the cells to generate predicted prices.
3. Adjust `alpha` or `queue_weight` to tune model behavior.

- Ideal for simple real-time pricing where computational simplicity is a priority.
- Does not consider complex temporal, traffic, or vehicle factors.
