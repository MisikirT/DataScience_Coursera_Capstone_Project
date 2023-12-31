Introduction and capston overview

In this challenge, you'll get the opportunity to tackle one of the most industry-relevant maching learning problems with a unique dataset that will put your modeling skills to the test. Subscription services are leveraged by companies across many industries, from fitness to video streaming to retail. One of the primary objectives of companies with subscription services is to decrease churn and ensure that users are retained as subscribers. In order to do this efficiently and systematically, many companies employ machine learning to predict which users are at the highest risk of churn, so that proper interventions can be effectively deployed to the right audience.

In this challenge, we will be tackling the churn prediction problem on a very unique and interesting group of subscribers on a video streaming service!
Imagine that you are a new data scientist at this video streaming company and you are tasked with building a model that can predict which existing subscribers will continue their subscriptions for another month. We have provided a dataset that is a sample of subscriptions that were initiated in 2021, all snapshotted at a particular date before the subscription was cancelled. Subscription cancellation can happen for a multitude of reasons, including:
the customer completes all content they were interested in, and no longer need the subscription
the customer finds themselves to be too busy and cancels their subscription until a later time
the customer determines that the streaming service is not the best fit for them, so they cancel and look for something better suited

Regardless the reason, this video streaming company has a vested interest in understanding the likelihood of each individual customer to churn in their subscription so that resources can be allocated appropriately to support customers. In this challenge, you will use your machine learning toolkit to do just that!In this notebook you should follow the steps below to explore the data, train a model using the data in train.csv, and then score your model using the data in test.csv. Your final submission should be a dataframe (call it prediction_df with two columns and exactly 104,480 rows (plus a header row). The first column should be CustomerID so that we know which prediction belongs to which observation. The second column should be called predicted_probability and should be a numeric column representing the likellihood that the subscription will churn.
Your submission will show an error if you have extra columns (beyond CustomerID and predicted_probability) or extra rows. The order of the rows does not matter.
The naming convention of the dataframe and columns are critical for our autograding, so please make sure to use the exact naming conventions of prediction_df with column names CustomerID and predicted_probability!

To determine your final score, we will compare your predicted_probability predictions to the source of truth labels for the observations in test.csv and calculate the ROC AUC. We choose this metric because we not only want to be able to predict which subscriptions will be retained, but also want a well-calibrated likelihood score that can be used to target interventions and support most accurately.
