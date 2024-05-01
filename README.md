# Phase 2 Project Description

GROUP 3 MEMBERS:

- ***CALVIN OMWEGA***
- ***INGAVI KILAVUKA***
- ***MERCY KIRAGU***
- ***COLLINS BIWOTT***

## PROJECT OVERVIEW

A real estate agency aims to provide detailed pricing models to their clients showing how different features impact home sale prices.By understanding these impacts,the agency can advise sellers on how to enhance their property to maximize sale price and assist buyers in evaluating potential homes

## BUSINESS UNDERSTANDING

#### CHALLENGES

- The King County real estate market is subject to fluctuations influenced by economic conditions, interest rates, and other external factors, posing challenges in predicting property values accurately.

- The presence of numerous real estate agencies and agents vying for clients' attention intensifies competition, requiring innovative strategies to stand out and attract business.

- Ensuring the accuracy and completeness of data sources, as well as accessing relevant datasets for analysis, presents challenges in developing robust pricing models and predictive analytics.

- Ongoing regulatory changes, such as zoning regulations, tax policies, and housing laws, can impact market dynamics and require adaptation to ensure compliance and mitigate risks.

#### BUSINESS OBJECTIVES

- Implement sophisticated data analytics techniques, including machine learning algorithms, to analyze historical sales data, identify trends, and predict future property values with greater accuracy.

- Develop customized pricing models that consider a wide range of factors, including property features, neighborhood characteristics, market demand, and buyer preferences, to provide tailored pricing recommendations for each property.

- Establish a framework for continuous monitoring of market trends and model performance, allowing for timely adjustments to pricing strategies and recommendations based on changing market conditions.

- Foster collaborations with data providers, industry experts, and technology partners to access additional data sources, enhance analytical capabilities, and stay abreast of best practices in real estate valuation and predictive modeling.

#### BUSINESS QUESTIONS

1. How can sellers optimize their property to maximize the sale price, and what tailored recommendations should be provided to enhance or highlight features that increase home value?
   
2. How can buyers be empowered to make informed purchasing decisions, and what insights should be provided about the correlation between property features and sale prices?

3. How can the agency enhance its competitive advantage by using advanced pricing models that offer detailed insights into the factors influencing home sale prices?

##### DATA USED
1. King County House CSV Dataset
2. Column Names Dataset

## DATA ANALYSIS

- Importing necessary libraries
- Data processing
- Data cleaning
- EDA (exploratory data analysis)
- Modeling (Simple and Multiple linear regression)

## Conclusions
After conducting a comprehensive analysis of the housing market in King County, the following conclusions can be drawn:

1. **Key Predictors of House Prices**: Through our analysis, we have identified several key predictors that significantly impact house prices in King County. These predictors include:
   - Condition of the property
   - View from the property
   - Latitude and longitude coordinates
   - Square footage of living space
   - Number of bedrooms
   - Number of bathrooms
   - Number of floors

2. **Impact of Predictors**: Our analysis reveals that these predictors have a substantial influence on house prices. Properties with better conditions, desirable views, larger living spaces, and more bedrooms and bathrooms tend to command higher prices in the market. Additionally, factors such as location (latitude and longitude) and the number of floors also play significant roles in determining property prices.

3. **Model Performance**: We developed predictive models to estimate house prices based on these predictors. 
The model does have some limitations: given that some of the variables needed to be log-transformed to satisfy regression assumptions, any new data used with the model would have to undergo similar preprocessing. Additionally, given regional differences in housing prices, the model's applicability to data from other counties may be limited. Given that outliers were removed, the model may also not accurately predict extreme values.

1. **Feature Enhancement**: Encourage sellers to focus on improving key features of their properties that have been identified as significant predictors of house prices. This includes enhancing the condition of the property, maximizing views, and optimizing living space layout.

2. **Property Marketing**: Highlight the key features identified in your analysis when marketing properties to potential buyers. Emphasize the condition, views, square footage, and other desirable attributes to attract interest and justify pricing.

3. **Price Guidance**: Provide sellers with data-driven insights into the factors influencing house prices in King County. Use your predictive models to offer guidance on pricing strategies based on the specific features and characteristics of each property.

4. **Buyer Guidance**: Assist buyers in identifying properties that align with their preferences and budget constraints. Educate them about the importance of key predictors in determining property value and help them make informed decisions during the home-buying process.

5. **Market Analysis**: Continuously monitor market trends and dynamics in King County. Stay updated on changes in buyer preferences, supply and demand dynamics, and other factors that may impact property prices. Use this information to adapt pricing strategies and marketing approaches accordingly.

6. **Data Integration**: Integrate your predictive models into the agency's operations to streamline pricing and decision-making processes. Develop tools or software solutions that leverage your models to provide real-time pricing estimates for properties listed by the agency.

7. **Client Education**: Educate clients about the insights and findings from your analysis. Offer workshops, webinars, or informational materials that explain the factors influencing property prices and how clients can leverage this knowledge to their advantage.

8. **Feedback Loop**: Establish a feedback loop with clients to gather insights and input on their experiences with pricing strategies and property evaluations. Use this feedback to refine and improve your predictive models and services over time.

By implementing these recommendations, the real estate agency can leverage data-driven insights to enhance their pricing models, improve client satisfaction, and ultimately achieve better outcomes for both sellers and buyers in the King County housing market.

## Model 4
R^2: 0.6842216567037567
Adjusted R^2: 0.6835323993283049
MAE: 0.22100190868161157
MSE: 0.08145001705495727
RMSE: 0.28539449373622694
MAPE 1.6909988010250971
cross validation score 0.6743903939586859

## Most relevant model (Interpretation)
- What combination of features is the best fit, in terms of predictive power, for a multiple regression model to predict house prices?
 
- Model 4: conditions,view,lat and long,sqft_living,bedrooms,bathrooms and floors
are the best fit for a multiple regression model. These features are highly correlated with price, have relatively low multicollinearity, and can together account for more than half of the variability of price. All multiple regression assumptions are satisfied with these features included.Also the model is valid as the cross validation score is not low.