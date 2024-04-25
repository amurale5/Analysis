# Predicting Bike Sharing Demand in Seoul

## Project Overview

### Project Objective:
> To develop a robust predictive model that accurately forecasts the demand for bike-sharing services in Seoul. The key aims are to:
    >1. Determine high and low demand periods daily and hourly.
    >2. Identify seasonal and weather-induced demand variations.
    >3. Suggest inventory optimization strategies.
    >4. Maintain a steady availability of bikes.
    >5, Enhance the precision of predictions using various machine learning models.

### Methodology:
> The methodology includes preprocessing data, selecting features, and tuning hyperparameters for different machine learning models. This involves running numerous iterations of each model with varying hyperparameters to find the most optimal settings for accuracy and efficiency.
The approach involves:
>1. Aggregating historical data on bike rentals along with weather conditions, city events, and traffic patterns.
>2. Conducting exploratory data analysis to uncover underlying patterns and influential demand factors.
>3. Utilizing machine learning models such as Random Forest, Gradient Boosting, and Neural Networks to capture complex relationships and forecast demand.
>4. Evaluating models based on accuracy, precision, and their ability to generalize without overfitting.

### Top 5 ML Models:
**XGBoost:**
> **Description** - An efficient implementation of gradient boosting that is designed to be highly efficient, flexible, and portable. It provides a parallel tree boosting that solve many data science problems in a fast and accurate way.
**Results** - XGBoost achieved a 94% accuracy rate with optimized hyperparameters like a learning rate of 0.2, a max depth of 4, and 100 estimators.
**Findings** - XGBoost is selected as the winning model due to its high accuracy and shorter runtime compared to other models.

**Gradient Boosting:**
> **Description** - Similar to XGBoost, but often refers to the use of gradient boosting machines without the specific optimizations that XGBoost brings.
**Results** - It also reached a 94% accuracy rate but was not selected as the top model, possibly due to longer runtimes or less optimized hyperparameters.

**Neural Network:**
> **Description** - A model that mimics the human brain's interconnected neuron structure, useful for capturing nonlinear complexities in the data.
**Results** - Achieved 94% accuracy and demonstrated high AUC scores, indicating a robust model for classification tasks.

**Random Forest:**
> **Description** - An ensemble learning method that operates by constructing a multitude of decision trees and outputting the class that is the mode of the classes of the individual trees.
**Results** - Achieved a 93% accuracy rate but showed signs of overfitting with a perfect accuracy on the training set.

**Decision Tree:**
> **Description** -  A decision support tool that uses a tree-like model of decisions and their possible consequences. It's straightforward to understand and interpret.
**Results** - Had the lowest accuracy rate among the top models at 91%, making it less preferable for this project's objectives.

### Overall Findings:
> Across the models, hyperparameter tuning was essential to improve accuracy. Notably, the ensemble methods like XGBoost and Random Forest tend to perform well on this kind of task. However, considerations such as overfitting and runtime were crucial in selecting the best model. XGBoost came out on top for having a strong balance of accuracy and efficiency.

### Analysis and Key Findings:
>- Time of day and weather conditions, especially temperature and humidity, emerged as significant predictors of bike rental demand.
>- Machine learning models demonstrated a promising ability to predict demand, with certain models showing potential for fine-tuning to avoid overfitting.
>- Our analysis indicates that integrating the forecast into the bike-sharing operation workflow could substantially enhance service reliability and efficiency.
  
### Business Value:
> Implementing the forecast model will benefit Seoul's bike-sharing system through:
>- Optimal inventory management, reducing underutilization and shortages.
>- Data-driven decision-making for strategic placement and redistribution of bikes.
>- Potential for dynamic pricing during peak demand, improving profitability.
>- Enhanced customer experience through improved service reliability.
