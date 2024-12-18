### Project Title

**Author**
Navin Bilwar

#### Executive summary
Traffic congestion and its associated issues are frequent challenges in urban environments. By studying traffic patterns and analyzing data, valuable insights can be gained for transportation planning,
# infrastructure development, and managing congestion effectively.

#### Rationale
Enables data-driven decisions to enhance urban mobility and create efficient, sustainable cities.

#### Research Question

Potential Applications:
 Congestion Management: Identifies congested areas and supports targeted interventions like signal optimizations and lane adjustments.
 Traffic Flow Analysis: Facilitates the study of traffic patterns and correlations with different factors.
 Urban Planning: Assists in assessing traffic impact for infrastructure decisions.
 Transportation Planning: Helps in understanding vehicle demand and determining new public transport requirements.

#### Data Sources
https://www.kaggle.com/datasets/hasibullahaman/traffic-prediction-dataset
Dataset Overview: Two CSV files containing traffic data collected by a computer vision model, detecting four vehicle classes: cars, bikes, buses, and trucks.
Data Details: Includes columns for time, date, day of the week, vehicle counts, total vehicle count for 15-minute intervals, and traffic situation categorized as Heavy, High, Normal, or Low.
Update Frequency: Data is updated every 15 minutes, 1st CSV file covers 1 month of traffic patterns, 2nd CVS file covers two months of traffic patterns.

#### Methodology
Analyze data collected to capture traffic patterns over a period of time and build different machine learning models, compare them, and suggest the best model.

#### Results

Models Performance Summary:

KNN:

Train and test accuracies are similar (~88%), suggesting the model is neither underfitting nor overfitting.
Precision, recall, and F1-scores are all balanced, indicating consistent performance across classes.
Low training time (~3s) makes it computationally efficient.

Logistic Regression:

Performance is slightly lower than KNN (~85% test accuracy).
Precision is higher than recall, which might mean it is better at avoiding false positives than catching all positives.
Low training time (2.8s) makes it computationally efficient.

Decision Tree:

Excellent performance on both training (94.3%) and test data (94.3%), indicating it generalizes well.
High F1-score (94.5%) means it achieves a balance between precision and recall.
Training time is the lowest among all models (~1.02s).

SVM:

Strong performance (91.1% test accuracy)
However, it took a longer training time (~32s), which may limit its scalability.
Best suited when computational resources are available and for high-dimensional problems.

Random Forest:

Best model overall, achieving the highest test accuracy (94.5%) and F1-score (94.66%).
Slightly longer training time (~84s) compared to others but compensates with robustness and performance stability due to ensemble learning.


#### Next steps
1. For further exploration, recommend evaluating other advanced modeling algorithms such as XGBoost or Deep Neural Networks.
2. Apply the recommended model on newer unseen datasets and test the model.
3. Derive more insights when the analysis can be further expanded with other similar datasets with more rich set of features.

#### Outline of project

- [Link to notebook 1]()


##### Contact and Further Information
Navin Bilwar
navinbilwar@gmail.com
