# Dynamic Parking Pricing – Summer Analytics 2025

This is my submission for the capstone project of Summer Analytics 2025 by Consulting & Analytics Club × Pathway.

The goal was to build a dynamic pricing model for urban parking lots using real-time data like traffic, occupancy, queue length, vehicle type, etc. I used pandas, numpy and bokeh for everything.

## What I Did

I made two models:

### 1. Baseline Model
This is a simple model where price increases based on how full the parking lot is. Just occupancy divided by capacity and a small alpha multiplier.

### 2. Demand-Based Model
This model uses a few more features:
- Occupancy
- Queue length
- Traffic level
- Whether it’s a special day
- Vehicle type (car, bike, truck)

I made a demand score using these, and changed the price based on that. Price is kept smooth and within a fixed range.

## Assumptions

- More traffic → less demand  
- Special days → more demand  
- Prices should not change too fast  
- Vehicle type affects how much space it takes

## Tools Used

- Python (Google Colab)  
- pandas  
- numpy  
- bokeh (for visualizations)

## Visualization

I plotted both models using Bokeh:
- Green line = baseline model  
- Blue line = demand-based model

## Files in This Repo

- `pricing_model.ipynb` → My main code notebook  
- `report.txt` → Short explanation of what I did   
- `star_screenshot.png` → Screenshot after starring the Pathway repo


