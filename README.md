# Closed Loop Manufacturing With Machine Learning And Integer Programming

Machine Learning is a remarkably powerful tool for gaining insights into various processes. However, Machine Learning, on its own, does not provide explicit directives on the actions we should undertake given specific situations. Bridging this gap between insight generation and decision-making requires the integration of Machine Learning and Integer/Linear Programming. Yet, it's worth noting that Integer/Linear programming doesn't readily accommodate Machine Learning models as inputs, particularly non-linear ones. This notebook aims to illustrate one potential approach to combining Machine Learning and Integer/Linear Programming effectively.

## Analytics Cycle Ressemble Closed Loop Manufacturing
![Analytical Cycle](./resources/Analytics_cycle.png)

![Closed Loop Illustration](./resources/grantek.png)

The concept of smart manufacturing or closed loop manufacturing ressembles a typical analytical cycle very much. Like shown below, The IOT data can be collected by software like Ignition (By Inductive Automation) can first be used to perform descriptive analytics like a dashboard. The next phase is using Machine Learning (ML), in combination with other data sources, to gather insights, understand the data. The final information delivery phase can than use the insights from ML models to feed into optimization algorithm like integer/linear programming to tell us what decisions should be made or machine settings should use based on different circumstances. 

![Closed Loop With Process](./resources/closed_loop_manufacturing.png)

## Insights Uncovered From Predictive Analytics
To illustrate the concept, Xgboost regressor were used for training of a sample dataset. An R^2 of 0.45 were achieved for the predicted data points vs actual and plot of predicted data against actual is shown below. 
![Prediction](./resources/Prediction.png)
The next 3 graphs are used to show the type of insights (relationships) can be generated from performing ML on the dataset. 
![Feature Importance](./resources/Feature.png)
The feature importance graph shows that aside from the time related features, relative humidty 
![Dew Point](./resources/Pressure.png)

![Overlay](./resources/Overlay.png)

![Illustration of Problem Setup](./resources/Decision_Flow.png)

![All Together](./resources/All_together.png)

![Optimized Instructions](./resources/Optimized_Instructions.png)

![Current Instructions](./resources/Current_Instructions.png)
