# AnomalieDetectionMethods
Discussion and Evaluation of Anomaly Detection Data Science Methods

## Overview
Perhaps the most common or familiar type of outlier is the observations that are far from the rest of the observations or the center of mass of observations although it becomes very challenging when we have many input variables defining a high-dimensional input feature space.

Outliers can skew statistical measures and data distributions, providing a misleading representation of the underlying data and relationships. Removing outliers from training data prior to modeling can result in a better fit of the data and, in turn, more skillful predictions.

## How do I ensure my project is delivering value?
The TOP Value Equation is specifically designed to fill the value ‘gap’ by:
1. Identifying all of the available benefits (not just ‘enough benefits’ to get the project approved)
2. Defining specific measurable end states—the desired business outcomes—that need to be achieved in the business for the benefits to be delivered in full (filling the ‘gap’)
3. Maximizing and then quantifying all of the available financial benefits
4. Identifying the change activities required to deliver these outcomes, benefits and value.

This Value Equation approach gives you:
- a clear, measurable definition of your future operational business-as-usual end states;
- a clear roadmap for delivery, making clear the interdependencies between outcomes;
- a basis for directing, controlling and governing the subsequent change/implementation/ program to achieve the business outcomes and their benefits (and not get ‘lost’ in the technical issues and options);
The detailed change activity list, which includes all of the activities for the business and the project that can then be used to develop far more robust cost estimates for the project and also be used as the basis from developing the work break down structure and schedule for the project plan.

## Installation
To use this project, first clone the repo on your device using the command below:

git init
git clone https://github.com//RoryDataScience/AnomalieDetectionMethods.git

## Development: Algorithms Considered
**Minimum Covariance Deteminant (Elliptic Envelope)**
- Defines a hypersphere (ellipsoid) that covers the normal data, and data that falls outside this shape is considered an outlier. 

**Isolation Forest**
- Isolation Forest, or iForest for short, is a tree-based anomaly detection algorithm.

**DBSCAN**
- Density-Based Clustering refers to unsupervised learning methods that identify distinctive groups/clusters in the data, based on the idea that a cluster in data space is a contiguous region of high point density, separated from other such clusters by contiguous regions of low point density.
- DBSCAN is a density based clustering algorithm (actually DBSCAN stand for Density-Based Spatial Clustering of Applications with Noise), what this algorithm does is look for areas of high density and assign clusters to them, whereas points in less dense regions are not even included in the clusters (they are labeled as anomalies). This is, actually, one of the main reasons I personally like DBSCAN, not only I can detect anomalies in test, but anomalies in training will also be detected and not affect my results.
- Automatically detect the number of clusters based on your input data and parameters: All you need is a function to calculate the distance between values and some guidance for what amount of distance is considered “close”. No need to specify clusters apriori and the algorithm can handle noise & outliers

**Local Outlier Factor**
- Locate those examples that are far from the other examples in the feature space and can work well for feature spaces with low dimensionality (few features), although it can become less reliable as the number of features is increased, referred to as the curse of dimensionality.

**One-Class Support Vector Machines**
- Captures the density of the majority class and classifies examples on the extremes of the density function as outliers where the level of contamination is controlled by the parameter "nu"

**Additional Dataset Resources** <br>
https://towardsdatascience.com/adrepository-anomaly-detection-datasets-with-real-anomalies-2ee218f76292

## Contribute
**Adding new features or fixing bugs**
This section is to give people an idea how they can raise issues or feature requests in this project

## License
