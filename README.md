# NYC Taxi Analysis and Forecasting Project at Denmark Technical University

**Introduction**
The analysis provided a comprehensive retrospective on NYC taxi rides, categorizing them into green and yellow taxis. The dataset, originating from the NYC Taxi and Limousine Commission (TLC), covered various aspects including trip records, passenger counts, and financial transactions.

**Task 1: Data Understanding**
Dataset Contents:
Dates and times for both pickup and drop-off were included.
Locations for both pick-up and drop-off were detailed.
The data encompassed trip distances, fares, rate types, and payment methods.
Driver-reported passenger counts were also included.

Data Source:
The data was obtained from technology providers through the Taxicab & Livery Passenger Enhancement Programs (TPEP/LPEP).
The TLC did not generate this data and, thus, did not vouch for its accuracy.

**Task 2: Exploratory Data Analysis (EDA)**
General Findings:
A noticeable correlation between fare amounts and tips was observed, excluding those who did not tip.
No connection between passenger counts and the total fare amount in yellow taxis was discerned.
It was confirmed that yellow taxis had no fees associated with passenger counts.

Comparison between Green and Yellow Taxis:
An unexpected approximate $5 difference in the average tip between the two taxi types was detected.
For the year 2022, yellow taxis exceeded green taxis in ride counts by 38,815,696.
A significant variance in the average distances traveled by the two taxi types was identified, necessitating future exploration.

**Task 3: Spatial Analysis**
Tools Used: Kepler.gl along with its Python integration.
Findings:
Yellow taxis primarily had their operations centered within Manhattan.
In contrast, green taxis predominantly functioned outside Manhattan, and demand diminished with increasing distance from the city center.

**Task 4: Temporal Analysis**
Detailed analyses of taxi ride temporal patterns were performed, broken down by time metrics.
Relationships between these temporal patterns and variables like trip distance and fare were scrutinized.
Codes were adapted from an informative tutorial.

**Task 5: Time-Series Forecasting**
Tool Utilized: Prophet was employed for forecasting.
Approach:
The model was trained on historical data to project future ride counts.
Projections for both green and yellow taxis for periods of 7 and 14 days were generated. The projected figures were then contrasted with actual figures.

**Metrics:**
Yellow Taxi (7 days forecast):
MAE: 4435.26
RMSE: 5065.49
Accuracy: 95.90%

Yellow Taxi (14 days forecast):
MAE: 4885.39
RMSE: 5725.02
Accuracy: 95.54%

Green Taxi (7 days forecast):
MAE: 75.67
RMSE: 99.51
Accuracy: 96.94%

Green Taxi (14 days forecast):
MAE: 94.38
RMSE: 114.58
Accuracy: 96.06%

**Conclusions:**
Both the 7-day and 14-day projections showcased commendable accuracies (>95%) for both taxi variants.
Although the model accurately depicted the dynamics of ride counts, minor discrepancies in magnitude predictions during abrupt variations were noted.

**Closing Remarks**
The investigation unveiled crucial insights into NYC's taxi dynamics, enabling stakeholders to make data-driven decisions. Future studies might focus on the identified disparities and incorporate additional external parameters for enhanced predictions.
