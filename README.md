# AnomalieDetectionMethods
Discussion and Evaluation of Anomaly Detection Data Science Methods

# Overview
Perhaps the most common or familiar type of outlier is the observations that are far from the rest of the observations or the center of mass of observations although it becomes very challenging when we have many input variables defining a high-dimensional input feature space.

Outliers can skew statistical measures and data distributions, providing a misleading representation of the underlying data and relationships. Removing outliers from training data prior to modeling can result in a better fit of the data and, in turn, more skillful predictions.

# Algorithms Considered
**One-Class Support Vector Machines**
- Captures the density of the majority class and classifies examples on the extremes of the density function as outliers where the level of contamination is controlled by the parameter "nu"

**Isolation Forest**
- Isolation Forest, or iForest for short, is a tree-based anomaly detection algorithm.

**Local Outlier Factor**
- Locate those examples that are far from the other examples in the feature space and can work well for feature spaces with low dimensionality (few features), although it can become less reliable as the number of features is increased, referred to as the curse of dimensionality.

**Minimum Covariance Deteminant (Elliptic Envelope)**
- Defines a hypersphere (ellipsoid) that covers the normal data, and data that falls outside this shape is considered an outlier. 