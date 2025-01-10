### Traffic Prediction Modeling

**Author**
Navin Bilwar

#### Executive summary
Traffic congestion and its associated issues are frequent challenges in urban environments. By studying traffic patterns and analyzing data, valuable insights can be gained for transportation planning, infrastructure development, and managing congestion effectively.

#### Rationale
Enables data-driven decisions to enhance urban mobility and create efficient, sustainable cities.

#### Research Question

Potential Applications: </br>
- Congestion Management: Identifies congested areas and supports targeted interventions like signal optimizations and lane adjustments. </br>
- Traffic Flow Analysis: Facilitates the study of traffic patterns and correlations with different factors. </br>
- Urban Planning: Assists in assessing traffic impact for infrastructure decisions. </br>
- Transportation Planning: Helps in understanding vehicle demand and determining new public transport requirements. </br>

#### Data Sources
https://www.kaggle.com/datasets/hasibullahaman/traffic-prediction-dataset </br>
- Dataset Overview: Two CSV files containing traffic data collected by a computer vision model, detecting four vehicle classes: cars, bikes, buses, and trucks. </br>
- Data Details: Includes columns for time, date, day of the week, vehicle counts, total vehicle counts for 15-minute intervals, and traffic situation categorized as Heavy, High, Normal, or Low. </br>
- Update Frequency: Data is updated every 15 minutes, 1st CSV file covers one month of traffic patterns, 2nd CVS file covers two months of traffic patterns. </br>

#### Methodology
Analyze data collected to capture traffic patterns over a period of time and build different machine learning models, compare them, and suggest the best model.

#### Results

Models Performance Summary: </br>

KNN: </br>

- Train and test accuracies are similar (~88%), suggesting the model is neither underfitting nor overfitting. </br>
- Precision, recall, and F1-scores are all balanced, indicating consistent performance across classes. </br>
- Low training time (~3s) makes it computationally efficient. </br>

Logistic Regression: </br>

- Performance is slightly lower than KNN (~85% test accuracy). </br>
- Precision is higher than recall, which might mean it is better at avoiding false positives than catching all positives. </br>
- Low training time (2.8s) makes it computationally efficient. </br>

Decision Tree: </br>

- Excellent performance on both training (94.3%) and test data (94.3%), indicating it generalizes well. </br>
- High F1-score (94.5%) means it achieves a balance between precision and recall. </br>
- Training time is the lowest among all models (~1.02s). </br>

SVM: </br>

- Strong performance (91.1% test accuracy) </br>
- However, it took a longer training time (~32s), which may limit its scalability. </br>
- Best suited when computational resources are available and for high-dimensional problems. </br>

Random Forest: </br>

- Best model overall, achieving the highest test accuracy (94.5%) and F1-score (94.66%). </br>
- Slightly longer training time (~84s) compared to others but compensates with robustness and performance stability due to ensemble learning. </br>

#### Apply ensemble techniques and determine the best model

Random Forest: </br>
- Classification report shows exceptional precision, recall, and F1-scores for most classes.

AdaBoost:  </br>
- While AdaBoost executed with a short training time, it underperforms in accuracy and F1-score compared to other models.

Gradient Boosting: </br>
- Gradient Boosting demonstrates competitive performance, but at a cost of longer training time.

Voting Classifier (Ensemble):  </br>
- As an ensemble method combining all classifiers, the Voting Classifier achieves a balance between performance and training efficiency, almost on par with Random Forest.

#### High-Level Insights:

Model Ranking:  </br>
- Best Model: Random Forest provides the most balanced performance, excelling in accuracy, precision, and recall while maintaining efficiency.
- Second-Best: Voting Classifier benefits from ensemble learning to offer high accuracy and generalization, though slightly lagging behind Random Forest.

#### Business-Level Recommendations:

- Random Forest is the most reliable choice for robust and scalable predictions, especially for imbalanced data scenarios.
- For critical applications, the Voting Classifier offers an ensemble solution with competitive performance, potentially benefiting from its hybrid approach.

#### Conclusion:
- For accurate and balanced predictions across traffic situations, Random Forest emerges as the best-performing model, achieving the highest accuracy, precision, recall, and F1-score with minimal training time. 
- Voting Classifier is a strong alternative if a hybrid ensemble approach is desired.

#### Next steps
1. For further exploration, recommend evaluating other advanced modeling algorithms such as XGBoost or Deep Neural Networks. </br>
2. Apply the recommended model on newer unseen datasets and test the model. </br>
3. Derive more insights when the analysis can be further expanded with other similar datasets with more rich set of features. </br>

#### Outline of project

- [Link to notebook](https://github.com/navinbilwar/capstone/blob/main/Capstone.ipynb) : https://github.com/navinbilwar/capstone/blob/main/Capstone.ipynb


#### Contact and Further Information
Navin Bilwar | navinbilwar@gmail.com
