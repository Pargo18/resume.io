---
layout: single
title: "Deep Learning vs Machine Learning for Dry Spell Modeling"
permalink: /projects/dry-spell-forecasting/
---

How do we model the patterns of drought? This project explores how well Machine Learning and Deep Learning methods can capture the behavior of dry spell sequences—periods without rainfall critical to agriculture and water management.

By comparing different modeling approaches, I aim to assess their performance, interpretability, and potential use for real-world forecasting in climate-sensitive regions.


This project constitutes an attempt to assess the dry spell patterns in the northern region of Ghana, near Burkina Faso. We aim to develop a model which by exploiting satellite products overcomes the poor temporal and spatial coverage of existing ground precipitation measurements. For this purpose 14 meteorological stations featuring different temporal coverage are used together with satellite-based precipitation products. Conventional machine-learning and deep-learning algorithms were compared in an attempt to establish a link between satellite products and field rainfall data for dry spell assessment.

The deep-learning architecture used should be able to efficiently manipulate spatial data. Hence, Convolutional Neural Networks were used in order to detect spatial patterns in the satellite data. Using these models we will attempt to exploit the long temporal coverage of the satellite products in order to overcome the poor temporal and spatial coverage of existing ground precipitation measurements. Doing that, our final objective is to enhance our knowledge about the dry spell characteristics and, thus, provide more reliable climatic information to the farmers in the area of Northern Ghana. Defining the optimal ANN architecture for each application depends on several factors. In our case, we are looking for an ANN architecture that would actually use as input the satellite-based images of precipitation at a fixed extent around any gauge (e.g. 32x32 pixels), while the labels will be the ground observations, constituting a typical supervised-learning modeling case. This process can be efficiently handled by a CNN. The input satellite precipitation images are passed through the feature extraction part and, then, the classifier of the CNN and the output is mapped in [0, 1]. For a more detailed analysis of the technical characteristics of the proposed CNN (convolutional layers, pooling layers, activation functions, padding etc.) refer to the code.
Even though the aforementioned concepts give a clear advantage to CNNs when dealing with spatial data, the potential of a conventional FNN is also being examined. The number and type of hidden layers, as well as the overall architecture of the FNN, is defined after trial-and-error processes and is a subject closely related to the spatiotemporal characteristics of the data used. Overall, the process scheme of all the modeling strategies used in this research are:

Four benchmark ML classifiers (Logistic Regression, Random Forest, Gaussian Naïve Bayes and Support Vector Machine) and one benchmark FNN;
- The main CNN classifier;
- An alternative of the CNN classifier which also incorporates the stations latitude as an input variable;
- Different modeling approaches attempting to confront class imbalance;
- Several “sophisticated” ensembles of models built in an attempt to combine the information of different satellite precipitation products, featuring majority vote models, models that stack different satellite data in parallel input channels and multi-resolution models;
- Three state-of-art classifiers used for multi-class classification fine-tuned and tested for this binary classification task.
## Project Highlights

- 🌍 **Applied Climate Modeling**: Focuses on reproducing dry spells based on historical weather and satellite data.
- 🤖 **ML vs DL**: Benchmarks classical Machine Learning models (like Random Forests) against Deep Learning architectures (like LSTMs).

## Tech Stack

- **Data Processing**: Pandas, NumPy
- **Machine Learning**: Scikit-learn (Random Forest, SVM)
- **Deep Learning**: TensorFlow/Keras (LSTM), PyTorch
- **Visualization**: Matplotlib + Seaborn

## Key Insights

- Deep Learning models better capture temporal dependencies but require more data and tuning.
- ML models offer faster training and easier interpretability—making them viable for some real-world applications.

> 📄 **Published Work**: [Dry-spell assessment through rainfall downscaling comparing deep-learning algorithms and conventional statistical frameworks in a data scarce region: The case of Northern Ghana](https://meetingorganizer.copernicus.org/EGU21/EGU21-8393.html)

> For the full code, visit the [GitHub repository](https://github.com/Pargo18/Applying-Deep-Learning-vs-Machine-Learning-models-to-reproduce-dry-spell-sequences)