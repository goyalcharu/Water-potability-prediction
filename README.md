# Water-potability-prediction

## ABSTRACT
In recent years the quality of water has degraded tremendously due to the industrial discharge of waste into the water bodies and ignorant and insensitive use of water by humans. This has caused threat to not only human life but also aquatic life. If drinking water contains unsafe levels of contaminants, it can cause health effects, such as gastrointestinal illnesses, nervous system or reproductive effects, and chronic diseases such as cancer.

## MOTIVATION BEHIND OUR PROJECT
The main causes of the alarming rise in surface water pollution around the world are population growth, increased economic activity, agricultural expansion and intensification, and an increase in the volume of untreated sewage discharged into rivers and lakes. Furthermore, the groundwater as well is being affected by daily human activities. Pollutants that are being dumped into the ocean affect the daily life of fish and other marine creatures. Water pollution is a major problem in the developing world, with diseases such as cholera and typhoid fever being the primary cause of infant mortality.

## PROBLEM STATEMENT
* Keeping in mind that rural areas have limited medical resources and water pollution can cause hazardous diseases especially among children, it is important to test the water quality.
* In rural areas the main source of income is agriculture and it requires proper irrigation. Hence water quality prediction should be practiced.

## DATASET AND FEATURES
* pH value: The range of pH is 6.52–6.83 in the dataset.
* Hardness: Caused due to presence of Ca and Mg.
* Solids (Total dissolved solids/ TDS): Tells the mineral content of water. Suitable range is 500 mg/l - 1000 mg/l.
* Chloramines: Chlorine level up to 4 milligrams per liter (mg/L or 4 parts per million (ppm)) is considered safe [2]in drinking water.
* Sulphate: Found in almost all the natural substances. Extensively used in industries.
* Conductivity: Presence of ions increases the conductivity of water. According to WHO standards, electrical conductivity value should not exceed 400 μS/cm.
* Organic_carbon: Total Organic Carbon (TOC) is a measure of the total amount of carbon in organic compounds in pure water.
* Trihalomethanes: Treated with chlorine. Safe drinking water level (80ppm).
* Turbidity: It measures light emitting properties of water. • Potability: Indicates if water is suitable for human consumption.

## SOCIETAL RELEVANCE
Sustainable Development Goal 6 (Good health and well-being) states that water and sanitation are at the very core of sustainable development, critical to the survival of people and the planet. One out of every three people lacks access to safe drinking water, two out of every five people lack access to a basic hand-washing facility with soap and water, and over 673 million people still defecate in the open.This project will help in fish farming, testing of safe drinking water, can help provide data to test for different components water to predict water quality which has been a major difficulty that the globe has encountered in recent decades i.e., estimating water quality.

## METHODS
In order to predict the quality of water we have used the following algorithms:
1. KNN (K Nearest Neighbour)
2. Decision Tree
3. Random Forest
4. Naive Bayes
5. Logistic Regression
6. Support Vector Machine
7. XGBoost
8. Stochastic Gradient Descent

## EXPERIMENTS, RESULTS AND DISCUSSION
The dataset is split into train and test in the ratio 0.7. All the algorithms are tested by taking different hyperparameters and the result giving best accuracy is considered. Following are the observations:

| MODEL                       | HYPERPARAMETERS                                                             | TRAINING ACCURACY (%) | TESTING ACCURACY (%) |
| :---:                       |     :---:                                                                   |           :---:       |       :---:          |
| KNN                         | K- 5, p – 1, metric - minkowski                                             |      79.459           |         62.055       |
| Decision Tree               | Criterion - entropy, max_depth - 12, splitter - best                        |      78.59            |         63.58        |
| Random Forest               | Criterion - entropy, max_depth – None, n_estimators - 100                   |      100              |         66.429       |
| Naive Bayes                 | Gaussian Naïve Bayes                                                        |      63.28            |         100          |
| Logistic Regression         | max_iter - 120, random_state - 0, n_jobs - 20                               |      61.58            |         59.51        |
| Support Vector Machine      | n_samples - 300, noise - 0.05                                               |      73.222           |         66.63        |
| Stochastic Gradient Descent | Default                                                                     |      61.27            |         100          |
| XGBoost                     | learning_rate - 0.001,max_depth - 5,n_estimators - 100,scale_pos_weight - 1 |      70.61            |         63.48        |

From the results obtained, Support Vector Machine is a preferable method. It did not suffer the condition of overfitting and performed well when there is a clear indication of separation between classes. SVM has shown better computational complexity. It has the ability to normalize the data. Hence, we can infer that SVM is better than other algorithms. Also, it can perform on n-dimensional space. Random Forest performed well; however, it shows overfitting, hence it isn’t preferred.

## CONCLUSION
After experimenting and trying out different algorithms the conclusion drawn was that “pH” is the attribute which majorly affects the quality of water samples.

## FUTURE WORK
Estimating water quality has been one of the world's most serious concerns in recent decades. Furthermore, a few developed models exist now to forecast the appropriateness of water for irrigation in an arid region. There do exist certain models which help predicting water quality for irrigation purpose. 40 percent of rural households in India still lack access to drinking water and healthcare, water scarcity being an emerging issue, highlighting these issues. With our project we aimed to determine compliance with drinking water standards, to support and protect designated uses of freshwater. Despite the achievements outlined in this project, some improvements are still possible, including we can collect more training samples to make the model more stable and more progress is possible on the prediction model. Those issues will be overcome in future research, perhaps by proper tuning of the Stochastic Gradient Descent model and using other algorithms










