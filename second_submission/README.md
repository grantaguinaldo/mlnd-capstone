# Identifying the Key Features of a Customer Dataset that can be used to Predict Chrun 

## Machine Learning Nanodegree Capstone Project 
By: Grant Aguinaldo

![](./images/mlnd-image.jpg)


We live in a subscription-based economy. The global consulting firm, [McKinsey & Company](https://www.mckinsey.com/industries/high-tech/our-insights/thinking-inside-the-subscription-box-new-research-on-ecommerce-consumers) noted that:

> The subscription e-commerce market has grown by more than 100 percent a year over the past five years. The largest such retailers generated more than $2.6 billion in sales in 2016, up from a mere $57.0 million in 2011.

However, while it seems that things are rosy for these businesses there is a stark reality: churn. Simply put, churn can be defined as the rate at which a company loses customers during a given time period. Indeed, despite record and rapid growth for these subscription-based businesses, churn can bring a subscription-based down, as quickly as it has grown, if companies do not deliver a superior product. Given the importance of the churn rate to the bottom line of any subscription-based business, it is key that business leaders not only track and monitor the churn rate but also identify the key factors that contribute to customer churn. By doing so, it then becomes possible to not only focus the business on customer acquisition efforts but more important than that, are the customer retention strategies that are needed for sustainable growth.  

This project was inspired by previous work from the [New York University where Deep Learning was used to predict customer churn](https://arxiv.org/pdf/1703.03869.pdf). For this project, we will develop an approach for identifying the key indicators of a customer data set that most contribute to churn, and will also develop a predictive model, based on the features in the dataset that can predict customer churn. My motivation for undertaking this project is two-fold. First, the large shifts of traditional based business to subscription-based business models (like [Adobe](https://www.bloomberg.com/news/articles/2017-06-08/how-adobe-got-its-customers-hooked-on-subscriptions)) as well as a large amount of activity of funding these businesses by [venture captial firms](https://hbr.org/2017/12/subscription-businesses-are-booming-heres-how-to-value-them). Second, is the notable acquisition of [Whole Foods by Amazon in  2017](https://www.forbes.com/sites/gregpetro/2017/08/02/amazons-acquisition-of-whole-foods-is-about-two-things-data-and-product/#7df17c63a808) for which many believe was a move to strengthen Amazon’s understanding of their current customer base via the data that Whole Foods have collected on their customer base. Finally, For this project, we will be using a dataset named `WA_Fn UseC_ Telco Customer Churn.csv` that was obtained from [IBM’s Watson's Analytics](https://www.ibm.com/communities/analytics/watson-analytics-blog/guide-to-sample-datasets/). 

In this problem, we will develop a machine learning model to predict customer churn from a given set of customer metadata (as given in the dataset). On a high level, the problem does have one potential, supervised learning, solution since there is a clear set of independent and dependent variables (discussed further in the following section). In addition, this problem is quantifiable in that all of the features of the data set are either continuous or categorical. In the case that features are categorical and non-numeric, we will employ the suitable methods to convert them into numerical values.  The problem is also measurable since there are quantitative methods to assess or measure the quality of the model once developed. Finally, the project will be replicable since there are more than 7,000 customers in the dataset that have a labeled outcome regarding churn (Yes/No) and we use random_states within the model so that others can reproduce our findings. 


#### Libraries used:

* imbalanced-learn==0.3.3
* numpy==1.14.2
* pandas==0.23.4
* scikit-learn==0.19.1
* xgboost==0.80

Note that the clean dataset that is being used for this project is included in the repo and is named `df_vect.csv`.

###
