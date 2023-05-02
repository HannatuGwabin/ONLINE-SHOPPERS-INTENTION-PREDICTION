# ONLINE-SHOPPERS-INTENTION-PREDICTION

Machine learning classification algorithms can be an effective tool for businesses to predict their customers' purchasing intentions.


# Resources

• Data Source: 10Alytics

• Tool: Jupyter notebook

• Packages: pandas, numpy, matplotlib, seaborn and sklearn


# Overview

Due to its ease, online shopping has grown in popularity over the past several years. As a result, companies are spending more money on internet marketing techniques to draw in and keep customers. Nonetheless, it can be difficult for businesses to comprehend their clients' purchase intentions and behavior.

Machine learning classification algorithms can be an effective tool for businesses to predict their customers' purchasing intentions. These algorithms analyze data points such as browsing history, search queries, and past purchases to identify patterns and predict future behavior.

Businesses can gain insights into customer's behavior and make more informed decisions about their marketing and sales strategies using a machine learning classification system. For example, a company may use this technology to identify which customers will most likely purchase and target their marketing efforts accordingly. Conversely, they may also use this technology to identify customers who are unlikely to buy and develop strategies to encourage them to complete a transaction. Using machine learning classification algorithms to predict purchasing intention can provide valuable insights for businesses looking to improve their online marketing and sales efforts.

# Objective

•	The objective of this project is to utilize machine learning algorithms to predict the purchasing intention (make a purchase or not) of a visitor to a store's website.

# Variables in the Dataset:

1.	Administrative: This is the number of pages of this type (administrative) the user visited.
2.	Administrative_Duration: This is the amount of time spent in this category of pages.
3.	Informational: This is the number of pages of this type (informational) the user visited.
4.	Informational_Duration: This is the amount of time spent in this category of pages.
5.	ProductRelated: This is the number of pages of this type (product related) the user visited.
6.	ProductRelated_Duration: This is the amount of time spent in this category of pages.
7.	BounceRates: The percentage of visitors who enter the website through that page and exit without triggering any additional tasks.
8.	ExitRates: The percentage of pageviews on the website that end at that specific page.
9.	PageValues: The average value of the page averaged over the value of the target page and/or the completion of an eCommerce transaction.
10.	SpecialDay: This value represents the closeness of the browsing date to special days or holidays (e.g., Mother's Day or Valentine's day) in which the transaction is more likely to be finalized. More information about how this value is calculated below.
11.	Month: Contains the month the pageview occurred in string form.
12.	OperatingSystems: An integer value representing the operating system that the user was on when viewing the page.
13.	Browser: An integer value representing the browser that the user was using to view the page.
14.	Region: An integer value representing which region the user is located in.
15.	TrafficType: An integer value representing what type of traffic the user is categorized into.
16.	VisitorType: A string representing whether a visitor is New Visitor, Returning Visitor, or Other.
17.	Weekend: A boolean representing whether the session is on the weekend.

# Target variable

Revenue: A boolean representing whether or not the user completed the purchase.

# Techniques used

✅ Import Libraries (pandas, numpy, matplotlib, seaborn and sklearn)

✅ Data Inspection (import Data, Descriptive Analysis, Data Shape, Data Info, and Check for missing Values).

✅ EDA (Univariate, Bivariate, Multivariate Analysis).

✅ Data Preprocessing (Feature Engineering, Encoding).

✅ Model Building (Splitting, Training Model evaluation).


# Exploratory Data Analysis (EDA)

![dist of visitors](https://user-images.githubusercontent.com/115185829/232251909-4a0eabb2-fc00-474d-9a9c-fd0f6769c09c.png)

A significant number of 85.6% visitors are returning visitors or customers which could indicate that the business has provided a positive experience and value to the customers


![Revenue by weekend](https://user-images.githubusercontent.com/115185829/232252312-d585eb00-c91a-4e08-89b9-ae73c6d014d5.png)

A significant number of purchases or Revenue was generated on weekdays, with 11.4%, compared to weekends, with 4.0%. People may be more likely to shop online during the week when they are at work and have access to a computer. However, on the weekends, they may prefer to shop in person or engage in other leisure activities.¶


![Revenue by Month](https://user-images.githubusercontent.com/115185829/232252538-b47dee22-05a5-47d4-b5fa-4cfe66053533.png)

May has the highest number of visited users with 27.3%, followed by November (24.3%) and March (15.5%). The fact that May has the highest number of visited users (27.3%) suggests that this month may be a hectic time for the website. This could be due to various reasons, such as seasonal sales or promotional events.


![Correlation](https://user-images.githubusercontent.com/115185829/232252693-e14b21f5-747d-408a-b997-87ec470141b2.png)


There is a strong correlation between BounceRates and ExitRates (0.91).

There is a strong correlation between ProductRelated and ProductRelated Duration (0.86).

There is a Moderate Correlation between Administrative and Administrative Duration (0.62).

There is a Moderate Correlation between Informational and Informational Duration (0.62).

There is a Moderate Correlation between Page Values and Revenue (0.49).


# Model Performance


![RFC](https://user-images.githubusercontent.com/115185829/232252984-ee96dfd3-7933-4d84-9084-4c743164a98d.png)


 Three (3) learning classifiers (Random Forest, Decision Tree and Naive Bayes) were tested. The Random Forest Classifier had the best performance with an accuracy of 89% and F-1 Score of 63%.
 



# Feature Importance Graph


![download](https://user-images.githubusercontent.com/115185829/232253034-be92a68e-ad29-4794-ad65-60ff6587a5d2.png)




The most significant feature in our dataset is PageValues since it correlates Moderately with our target variable (Revenue). This feature importance graph generally aligns with our correlation analysis.



# Recommendations


REGION

•	Offer region-specific promotions or discounts: Create special offers or discounts for visitors from specific areas. This can incentivize them to engage with the business and potentially purchase.
•	Leverage social media: Use social media platforms to engage with potential customers in each region. Share region-specific content, participate in local conversations, and engage with customers in their local language.

•	Use paid advertising: Consider using paid advertising, such as Google Ads or social media ads, to target potential customers in each region. This can help increase visibility and drive more traffic to the website.

WEEKEND 

•	Utilize social media: Use social media platforms like Facebook, Twitter, and Instagram to promote your website and weekend-specific promotions. Be sure to use relevant hashtags and post at times when your target audience is most active.

•	Offer weekend-specific promotions: Consider offering special deals or discounts only on weekends. This can significantly incentivize customers to visit your website during their free time.

BOUNCE RATE AND EXIT RATE

•	Improve Website Load Time: Slow website loading times can lead to high bounce rates. A business can reduce website load time by optimizing images and reducing plugins.

•	Improve Website Content: Engaging and informative website content can help keep visitors on a website longer. Therefore, a business should ensure its website content is high-quality, relevant, and up-to-date.

SPECIAL DAY

•	Run holiday-themed promotions: Offer special discounts or upgrades during the holiday period to incentivize customers to purchase. For example, a clothing store could offer a discount on Mother's Day gifts. In addition, businesses can increase engagement and visits to their website during special holidays by running promotions, utilizing social media, and running paid ads.

