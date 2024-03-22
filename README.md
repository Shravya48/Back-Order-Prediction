Back Order Prediction in Supply Chain Management:

What is Back Order?
Back order prediction in supply chain management refers to the process of forecasting or estimating the future demand for a product 
or item that is currently out of stock or unavailable for immediate delivery. When a customer places an order for a product that is not currently in stock,
the order is typically placed on back order, meaning it will be fulfilled and delivered once the product becomes available again.

Business Significance:
1. Customer Satisfaction and Retention: Accurate back order predictions ensure customer satisfaction and loyalty.
2. Efficient Inventory Management: Optimize stock levels and minimize stockouts with back order forecasting.
3. Enhanced Supply Chain Efficiency: Streamline operations and improve efficiency through precise back order predictions.

Project Objective:
1. Develop a machine learning model to accurately predict the occurrence of back orders for products based on various factors,
   including inventory levels, sales history, forecasts, lead time, and supply chain indicators.
2. Optimize inventory management by leveraging the predictive model to proactively identify products at risk of going on back order,
   allowing for timely replenishment and minimizing stock outs.
3. Improve customer satisfaction by ensuring timely fulfilment of orders and reducing the occurrence of back orders, thereby enhancing the overall customer experience.
4. Enhance supply chain efficiency by effectively managing potential disruptions or risks associated with deck issues, OE constraints, PPAP risks, stop auto-buy signals,
 and revision stops, enabling proactive mitigation strategies.

Conclusion:
1.The Data Set We Got Was Significantly imbalanced to the ratio 99.3 % negative and 0.70 % Positive Class , So we had to Use minority Oversampling Technique SMOTE 
   on the train dataset for training the model.
2.The Extreme Skewness of the Data was Dealt by using Robust Scaler and then Doing Yeo Johnson Power Transformation.
3.The Outliers in the Dataset was genuine values hence we used winsorization to cap the outliers at 97.5 quantile and 2.5 quantile.
4.The Multicollinearity in the dataset was removed by using PCA, The PCA was used by combining the Sales Columns into one, Forecast columns into one 
  and Performance Columns into one so that The explainability of the model is not lost.
5.The Final Model is Selected based on Test Recall Score.
6.Best Three models was used in the Voting Classifier for the final model
7. The major Limitation of the model is the lack of Precision in the positive class prediction , as many negative class was predicted as positive due low threshold, 
    but for our Business problem the priority is on Recall/Sensitivty as an order not being predicted will be having huge economic Impact that False prediction



