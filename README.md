We will work with the Amazon product reviews dataset for this project. The dataset contains ratings of different electronic products. It does not include information about the products or reviews to avoid bias while building the model.

## Context:

Today, information is growing exponentially with volume, velocity and variety throughout the globe. This has lead to information overload, and too many choices for the consumer of any business. It represents a real dilemma for these consumers and they often turn to denial. Recommender Systems are one of the best tools that help recommending products to consumers while they are browsing online. Providing personalized recommendations which is most relevant for the user is what's most likely to keep them engaged and help business.

E-commerce websites like Amazon, Walmart, Target and Etsy use different recommendation models to provide personalized suggestions to different users. These companies spend millions of dollars to come up with algorithmic techniques that can provide personalized recommendations to their users.

Amazon, for example, is well-known for its accurate selection of recommendations in its online site. Amazon's recommendation system is capable of intelligently analyzing and predicting customers' shopping preferences in order to offer them a list of recommended products. Amazon's recommendation algorithm is therefore a key element in using AI to improve the personalization of its website. For example, one of the baseline recommendation models that Amazon uses is item-to-item collaborative filtering, which scales to massive data sets and produces high-quality recommendations in real-time.

## Objective:

You are a Data Science Manager at Amazon, and have been given the task of building a recommendation system to recommend products to customers based on their previous ratings for other products. You have a collection of labeled data of Amazon reviews of products. The goal is to extract meaningful insights from the data and build a recommendation system that helps in recommending products to online consumers.


# Conclusions:

We have tried multiple models and were able to identify the key factors involved with high coversion rate for the company.

The best model among these options depends on the specific priorities and trade-offs we are willing to make:
- For Maximum Accuracy: The Random Forest model has the highest testing accuracy (0.86).
- For Improved Generalization: The Tuned Random Forest model shows improved generalization with a balanced performance on the testing set (accuracy: 0.82).
- For Simplicity and Interpretability: The Decision Tree model is simpler and easier to interpret but may suffer from overfitting.
- For a Balance of Recall and Precision: The Tuned Decision Tree model shows a trade-off with improved recall but lower precision.

In most cases, if generalization and balanced performance are crucial, the Tuned Random Forest model would be a good choice as it combines good accuracy with improved generalization compared to the original Random Forest model.

Based on the recall scores for class 1 (default), the Tuned Decision Tree model has the highest recall on both the training (0.91) and testing (0.89) sets among all the models provided. Therefore, if maximizing recall to minimize false negatives is the primary goal, the Tuned Decision Tree model would be the best choice among the options provided.

In conclusion, the combination of age, website interaction metrics, profile completion, and specific activity indicators (such as last activity type) are key factors influencing the models' predictions.


# Actionable Insights and Recommendations

- All models suggest that time_spent_on_website, first_interaction_website, age, profile_completed_medium, last_acitivity_phone, last_activity_website and page_views_per_visit are the most important features.
- Metrics related to website interaction (time_spent_on_website, first_interaction_website, page_views_per_visit, last_activity_website Activity) are consistently important, highlighting the significance of user engagement and activity on the website in understanding customer behavior.
- Understanding the factors influencing time spent on the website (such as content engagement, user experience, etc.) can be valuable for optimizing the website's performance and user engagement strategies.
- Understanding factors influencing page views per visit (such as website layout, content organization, etc.) can help optimize user engagement and website performance.
- Dataset reflects a user base primarily consisting of professionals who tend to interact more through digital platforms like websites and email. The majority of users have completed their profiles to a high level, indicating active engagement with the platform. However, there is limited engagement with traditional media channels and referrals, highlighting the preference for digital interactions among this demographic.
- Based on this data, if we're looking to target a specific age group for a particular service or product, we might consider focusing more on Professionals and Unemployed individuals due to their higher average ages, assuming the target demographic aligns with these age ranges. However, it's crucial to consider other factors such as interests, needs, and purchasing power beyond just age when developing marketing strategies or designing products/services.
- Consider implementing cross-channel strategies to leverage the strengths of both the Website and Mobile App.
- Invest in data analytics and A/B testing to continuously optimize user experiences and improve conversion rates across all channels.
- Medium Profile Completion level has the highest number of profiles but also the highest percentage of non-purchases, consider optimizing the completion process to improve conversion rates. This could involve simplifying the steps, providing incentives, or addressing any barriers that may be hindering conversions.

