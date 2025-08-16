---
layout: single
title: "Deep Learning vs Machine Learning for Dry Spell Modeling"
permalink: /projects/dry-spell-forecasting/
---

How do we model the patterns of drought? This project explores how well Machine Learning and Deep Learning methods can capture the behavior of dry spell sequences—periods without rainfall critical to agriculture and water management.

By comparing different modeling approaches, I aim to assess their performance, interpretability, and potential use for real-world forecasting in climate-sensitive regions.


Large parts of the world rely on rainfed agriculture for their food security. In Africa, 90% of the agricultural yields rely only on precipitation for irrigation purposes and approximately 80% of the population’s livelihood is highly dependent on its food production. Parts of Ghana are prone to droughts and flood events due to increasing variability of precipitation phenomena. Crop growth is sensitive to the wet- and dry-spell phenomena during the rainy season. To support rural communities and small farmer in their efforts to adapt to climate change and natural variability, it is crucial to have good predictions of rainfall and related dry/wet spell indices.

This research constitutes an attempt to assess the dry-spell patterns in the northern region of Ghana, near Burkina Faso. We aim to develop a model which by exploiting satellite products overcomes the poor temporal and spatial coverage of existing ground precipitation measurements. For this purpose 14 meteorological stations featuring different temporal coverage are used together with satellite-based precipitation or cloud top temperature products.

We will compare conventional copula models and deep-learning algorithms to establish a link between satellite products and field rainfall data for dry-spell assessment. The deep-learning architecture used should be able to both have the feature of convolution (Convolutional Neural Networks) and the ability to capture a sequence (Recurrent Neural Networks). The deep-learning architecture used for this purpose is the Long Short-Term Memory networks (LSTMs). Regarding the copula modeling, the Archimedean, the Gaussian and the extreme copulas will be examined as modeling options.

Using these models we will attempt to exploit the long temporal coverage of the satellite products in order to overcome the poor temporal and spatial coverage of existing ground precipitation measurements. Doing that, our final objective is to enhance our knowledge about the dry-spell characteristics and, thus, provide more reliable climatic information to the farmers in the area of Northern Ghana.

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