---
layout: single
title: "Predicting Malaria Prevalence with Environmental Data"
permalink: /projects/malaria-predictive/
---

In collaboration with Arup and Médecins Sans Frontières (MSF), I was part of a multidisciplinary team developing an AI-based forecasting tool to predict malaria prevalence in South Sudan. The goal was to provide accurate, location-specific early-warning signals to help MSF optimize resource allocation for prevention and treatment in vulnerable regions.

The project integrated remote sensing environmental data with in-situ malaria prevalence observations. I developed an automated data pipeline that connected to multiple remote sensing APIs (including Copernicus and other open-access climate and land-monitoring sources) to retrieve monthly updates on environmental indicators such as rainfall, vegetation indices, and land surface temperature.

A key focus was extensive feature engineering—both systematic and brute-force approaches—across a wide range of environmental variables. This process uncovered strong correlations between complex feature combinations and subsequent malaria outbreaks, enabling the models to leverage subtle environmental patterns as predictive signals.

We experimented with a diverse set of machine learning and deep learning methods—including Random Forests, Gradient Boosting Machines (XGBoost, LightGBM), and sequence-based models such as LSTMs and Temporal Convolutional Networks (TCNs). We also implemented voting ensemble frameworks to combine complementary model strengths, improving robustness and generalization.

To ensure ongoing relevance of predictions, we delivered a fully automated retraining framework. This system regularly downloaded new environmental and malaria prevalence data, retrained the models at fixed intervals, and updated forecasts without manual intervention. Results were presented through a custom interactive dashboard designed for MSF’s operational teams, enabling rapid interpretation and response.

Rather than relying solely on generic accuracy metrics, we designed scope-oriented evaluation measures tailored to the client’s operational needs. This ensured the forecasts were optimized for identifying upcoming prevalence trends in the context of real-world decision-making, rather than just statistical performance.

This work was conducted as part of the wider Arup project team. Due to confidentiality agreements, the source code and exact implementation details are proprietary and cannot be shared.

## Project Highlights

- 🌍 **Global Health Meets AI**: Supports humanitarian operations through data-driven malaria forecasting.
- 🤖 **Conventional ML Models**: Includes Random Forest, Gradient Boosting, and Linear Regression for prediction tasks.
- 🔧 **Brute-Force Feature Engineering**: Engineered and tested hundreds of environmental variable combinations to find those most predictive.
- 📉 **Performance Evaluation**: Compared model outputs against observed monthly malaria case averages using statistical error metrics.

## Tech Stack

- **Data Sources**: Satellite imagery (NDVI, rainfall, temperature), MSF case data
- **Models**: Random Forest, XGBoost, Linear Regression
- **Feature Engineering**: Lag features, temporal aggregations, composite indices
- **Evaluation**: RMSE, standard deviation, correlation with monthly case averages

## Key Insights

- Certain engineered environmental indicators—created via brute-force combinations—showed **strong correlation** with malaria prevalence.
- ML models outperformed naive baselines, especially in capturing seasonal dynamics.
- The tool demonstrated potential for **scalable, non-invasive forecasting** to guide public health interventions.

> 📄 **More about the implementation**: [Predicting Malaria Prevalence with Environmental Data](https://www.linkedin.com/posts/msf-sweden-innovation-unit_climatecrisis-climatechange-activity-6994204445551038464-pf4M?utm_source=share&utm_medium=member_ios)