# Delivery-Time-Prediction
### 1 Introduction

Delivery time prediction has long been a part of city logistics, It is important for customer satisfaction
that the initial prediction is highly accurate and that any delays are communicated effectively.
In this report, I’ll discuss my roadmap of building the model that takes data about food delivery
as input to predict the total delivery duration seconds.
Some other things to note:
• Drivers can be assumed to arrive at the supplier at exactly the dictated pick-up time. In
reality this isn’t always true, but with a sufficient number of drivers this can be kept to a
minimal amount.
• Food should not be delivered too late as the customer will be left waiting and angry and not
too early as it will have to sit out before the customer is ready to eat it.

### 2 Analyze, identify patterns, and explore the data

As an input to our model, we have five categories of data:Time Features, Store Features, Order
Features, Market Features, Predictions From Other Models
Other than the existing features, I generated 6 additional features from the given data to
improve model performance.
1. Total available dashers: get the number of available(free) dashers who are within 10 miles of
the store at the time of order creation.
2. Average value: average value of each order
3. Order submission day of week
4. Order submission hour
5. Order submission month
6. Estimated delivery duration: Sum of estimated order place duration store to consumer driving
duration
