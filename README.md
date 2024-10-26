# Laptop Price Prediction Model

This project aims to build a model that estimates the prices of laptops based on key features. 
We use a combination of machine learning models and deep learning to provide a prediction system. 

## Dataset

The dataset includes the folowing features :

- **Brand**: The laptop manufacturer (e.g., Dell, HP, Apple). We will consider only the top 8 manufacturers and put the rest of them in a new category named "others"
- **Size**: Screen size in inches. 
- **Screen Resolution**: The display resolution. We will be creating seperate columns for In-Plane Switching panels and Touchscreen laptops.
- **CPU**: The central processing unit type. Again we'll be considering some Intel and AMD CPUs and putting the rest in "others" category.
- **RAM**: The amount of memory. Seperate columns will be created for SSD memory type, HDD memory type, Hybrid memory type and Flash Storage memory type.
- **GPU**: The graphics processing unit type. Here also we'll be considering some of the Intel, Nvidia and AMD CPUs and putting the rest in "others" category
- **Operating System**: The pre-installed operating system (e.g., Windows, macOS).
- **Weight**: The laptop’s weight which affects portability aspect.

## Models Used

To predict laptop prices, we implement multiple models to ensure robust results:

1. **Linear Regression** - Gives a decent accuracy.
2. **K Neighbors Regressor** - Does not perform well here.
3. **Decision Tree Regressor** - Does not perform well here.
4. **Random Forest Regressor** - Gives a decent accuracy.
5. **Voting Regressor** -  Gives a decent accuracy.
6. **Convolutional Neural Network (CNN)** - Traditionally used for images and can capture complex feature interactions, CNN does not give a good accuracy here.

## Evaluation

Each model’s performance is evaluated using metrics such as **Mean Absolute Error (MAE)** and **R² Score**.
Cross-validation is used to ensure stability, and results are averaged across multiple runs to reduce variance in performance.

This project was made mainly to focus on Feature Engineering. It gives an average performance which is something to improve upon. 
Reasons for this can be uneven data distribution, outliers and limitations in features. Laptop pricing often includes subjective factors that are difficult to quantify.

