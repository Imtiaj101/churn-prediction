Telecom churn case study


***Abstract***—**In  the  dynamic  telecommunications landscape,  service  providers  face  the  persistent challenge of retaining their customers. Nowadays, a customer has multiple options to choose an operator and can easily switch from one operator to another. The  telecommunications  industry's  annual  churn rate tends to range between 10 and 20 percent due to the intense competition in the sector. Given the fact that a new customer acquisition cost is 3 to 4 times higher,  retaining  an  existing  customer  becomes crucial.  As  a  result,  telecom  operators  are  now focusing  more  on  customer  retention  than acquisition. The objective of this project is to explore telecom  customer-level  data,  follow  the  detailed steps of data analytics, and predict customer churn, which  will  help  telecom  companies  proactively address and mitigate retention challenges.** 

**This study specifically targets high-value customers in  the  Southeast  Asian  markets,  who  contribute significantly to  the  revenue  stream.  By  analyzing customer behavior and usage patterns during the 'good' phase (initial months of service), we identify those  at  high  risk  of  churn.  Our  methodology involves a comprehensive analysis of customer data, with  machine  learning  techniques  using  Logistic Regression.  These  models  are  evaluated  using metrics like accuracy, precision, recall, and ROC- AUC, ensuring a robust predictive model.** 

**Our research provides valuable insights into why customers  leave  a  telecom  service.  We  have identified specific patterns in customer behavior and service  usage  that  indicate  potential  churn.  This understanding can help telecom operators develop targeted  strategies  to  keep  their  most  valuable customers. Our study highlights the importance of predictive analytics in the telecom industry, which can be used as a tool to improve customer loyalty and reduce churn rates.** 

***Keywords—  customer  churn,  logistic  regression, accuracy, precision, recall, roc-auc*** 

1. **INTRODUCTION** 

Telecommunications  providers  face  the  persistent challenge  of  retaining  their  customers.  In  a  highly competitive  environment,  customers  have  various options to choose from and can easily switch between 

providers. Due to this intense competition, the annual churn rate in the telecommunications industry typically fluctuates between 10 and 25 percent. It is important to note that retaining an existing customer is more cost- effective than acquiring a new one, which can cost three to four times more. Therefore, telecom operators are more focused on customer retention than acquisition, recognizing its importance in the industry. 

*A.  Problem Statement:*  

Telecom  companies  in  Southeast  Asia  face  unique challenges in retaining high-value customers. Losing such customers can significantly impact their revenue, particularly in this demographic. To ensure sustainable growth,  it  is  essential  to  address  this  challenge strategically and proactively. Telecom companies must understand the indicators and factors contributing to customer  churn  in  these  markets  to  design  effective retention strategies. 

2. **LITERATURE REVIEW**

This  review  explores  studies  that  have  used  data analytics  to  predict  customer  churn  in  the telecommunications industry. The focus of these studies has been on high-value customers who have stopped using  a  service.  The  loss  of  such  customers  is  a significant challenge in the telecommunications sector. 

Different studies have used different methods to predict the likelihood of customers leaving a company. One research  by Vafeiadis  et al.  (2015)  pointed  out  that machine  learning  techniques  such  as  Logistic Regression, Decision Trees, and Neural Networks are commonly  used  for  this  purpose.  These  models  are generally built using customer demographic data, usage patterns, and billing information.[1] 

Keramati and colleagues conducted a study in 2014 that focused on call details, data usage, and subscription changes  to  investigate customer  usage  patterns.  The study revealed that small details in usage patterns are significant  indicators  of  potential  churn.  This underscores the importance of analyzing minute details in  customer  usage  patterns  to  identify  potential churn.[2] 

According to Hadden et al. (2007), if customers are less satisfied and perceive the service quality to be low, there 

XXX-X-XXXX-XXXX-X/XX/$XX.00 ©20XX IEEE 

is a higher chance that they will stop using the service, also known as "churn".[3] 

3. **EXPERIMENTAL SETUP** 
1. *Dataset:*  

Customer-level  data  provided  by  a  leading  telecom firm. The dataset contains customer-level information for a span of four consecutive months  - June, July, August, and September. The months are encoded as 6, 7, 8 and 9, respectively.  

Dataset details: 226 columns 

`            `99998 records 

After  Processing  the  data  to  calculate  the  recharge amount is critical. This formula is essential for selecting high-value clients using criteria. 

2. *Evaluation Metrics* 

Model performance was evaluated using below three calculations: 

Accuracy: This is the proportion of true results (both true  positives  and  true  negatives)  among  the  total number of cases examined. To calculate accuracy, you can use the formula: 

![](Aspose.Words.0224bbc6-2498-4207-be8a-c87940f625bf.001.png)

Sensitivity  (also  known  as  Recall  or  True  Positive Rate): This measures the proportion of actual positives that are correctly identified. The formula for sensitivity is: 

![](Aspose.Words.0224bbc6-2498-4207-be8a-c87940f625bf.002.png)

Specificity (also known as True Negative Rate): This measures the proportion of actual negatives that are correctly identified. The formula for specificity is: 

![](Aspose.Words.0224bbc6-2498-4207-be8a-c87940f625bf.003.png)

1. *Data Preparation:*  

We define churn in terms of inactivity during the churn phase. This inactivity is identified by the absence of both outgoing and incoming calls, as well as data usage. 

2. *Data Quality Assurance:*  

Rigorous data quality checks are performed, focusing on  identifying  and  addressing  missing  values.  We utilize  visual  tools  like  klib  to  analyze  and  address columns with over 5% missing data, ensuring the data's integrity. 

![](Aspose.Words.0224bbc6-2498-4207-be8a-c87940f625bf.004.jpeg)

Fig.1:  Missing Value plot 

3. *Exploratory Data Analysis (EDA):* 

We perform in-depth univariate and bivariate analyses to understand individual features like Average Revenue Per  User  (ARPU),  Minutes  of  Usage  (MOU),  and recharge amounts, and their interrelations with churn. We examine  patterns,  trends, and  outliers  to extract meaningful insights about customer behavior. 

4. **METHODOLOGY** 

The project sets out with an aim to significantly reduce churn  among  high-value customers  in  the  Southeast Asian markets. These customers, who contribute a large portion  (around  80%)  to  the  overall  revenue,  are primarily identified based on their recharge behavior. Specifically, those who recharge at or above the 70th percentile of the average recharge amount during the first two months, referred to as the 'good phase,' are categorized as high-value customers. 

The methodology unfolds through several strategically designed steps: 

![](Aspose.Words.0224bbc6-2498-4207-be8a-c87940f625bf.005.jpeg)

Fig.2: ARPU trend 

Analyzing  the  trend  in  Average  Revenue  Per  User (ARPU) over three months (6th, 7th, and 8th month) to understand  customer  churn  patterns.  Here  notable decline in ARPU for churn customers, particularly in the 8th month. 

![](Aspose.Words.0224bbc6-2498-4207-be8a-c87940f625bf.006.jpeg)

Fig.3- Recharge Trends 

A subsequent decrease in the 8th month, particularly among churn customers. 

![](Aspose.Words.0224bbc6-2498-4207-be8a-c87940f625bf.007.jpeg)

Fig.4: AoN Trend  

Statistical Insights: 

- Mean Age on Network: 1219.85 days 
- Median Age on Network: 863 days 
- Mode: 3651 days 
- Standard Deviation: 954.73 days 
- Percentiles: 25th (467 days), 50th (863 days), 75th (1807.5 days) 

Customers have been with the operator for different lengths  of  time, from  new  to  very  long-term. Some customers have stayed over 4000 days, showing strong loyalty. Many customers are relatively new, suggesting a  chance  to  keep  them  longer.  Different  customer tenures  mean  different  needs  and  preferences.  A significant  number  of customers are  new  and  might need extra attention to stay. 

![](Aspose.Words.0224bbc6-2498-4207-be8a-c87940f625bf.008.png)

Fig.5: Outgoing MoU trend  

![](Aspose.Words.0224bbc6-2498-4207-be8a-c87940f625bf.009.png)

Fig.6: Incoming MoU trend  

Here above two graph showing significant drop in total incoming  calls  and  total  outgoing  calls  for  churn customers.  However,  for  non-churn  customer  its increasing. 

![](Aspose.Words.0224bbc6-2498-4207-be8a-c87940f625bf.010.png)

Fig.7: Recharge trend  

Our  data  shows  that  customers  who  churn  tend  to decrease their spending. 

![](Aspose.Words.0224bbc6-2498-4207-be8a-c87940f625bf.011.jpeg)

Fig.8: Feature-Correlation Pearson graph 

The image is a heatmap showing how closely related different pairs of telecom data points are. Darker colors mean  stronger  relationships,  which  will  be  used  to reduce the features efficiently. 

4. *Feature Engineering:* 

This  phase  entails  refining  the  dataset  by  removing columns with excessive missing values and irrelevant data,  such  as  details  pertaining  to  the  9th  month. Categorical  variables  are  meticulously  handled,  and numerical  features  are  normalized  using  Min-Max scaling, excluding date columns. 

5. *Model Implementation (Logistic Regression):*  Logistic regression helps us predict who will stay with 

   a service and who might leave. It looks at customer details and sees patterns. If a customer fits a pattern of leaving, the model raises a flag. It is simple and smart like  a  crystal  ball  for  customer  loyalty.  Prior  to addressing the data imbalance, we implement a Logistic 

Regression model. This model serves as a baseline to understand churn prediction in its current state of data imbalance. 

6. *Addressing Data Imbalance:*  

To tackle the skewed churn distribution, we apply the Synthetic  Minority  Over-sampling  Technique (SMOTE). This technique balances the dataset, making it more suitable for predictive modeling.After balancing the  dataset,  Logistic  Regression  is  re-implemented. This step is crucial to evaluate the effectiveness of the model on the newly balanced dataset. We also utilize Recursive Feature Elimination (RFE)  to identify  the most predictive features. 

7. *Model Evaluation and Optimization:*  

We conduct a comprehensive evaluation of the Logistic Regression model using metrics such as ROC curves, accuracy, sensitivity, and specificity. Additionally, we determine the optimal threshold for churn prediction based on precision-recall analysis. 

The final step involves analyzing the model to identify key drivers of churn. Based on these insights, we formulate strategic recommendations for the business, focusing on customer segments with lower total recharge amounts and devising personalized retention strategies. 

5. RESULT 
1. *Model Validation* 

Our  exploration  into  churn  prediction  revealed compelling findings: 

Use RFE with Logistic Regression to narrow down to 20 key features. Before balancing the dataset, Logistic Regression  gave  us  a  baseline  understanding.  Its performance  was  reasonable  but  not  optimal, particularly in identifying the less represented churn cases. The achieving an accuracy rate of almost 94.8%.  Additionally, it demonstrated good performance on the fraud class with a sensitivity of 53% and specificity of 97%. 

![](Aspose.Words.0224bbc6-2498-4207-be8a-c87940f625bf.012.png)

Fig.9: Optimal Prediction Threshold 

The real game-changer was the application of SMOTE. Here,  Logistic  Regression's  accuracy  improved significantly.  

![](Aspose.Words.0224bbc6-2498-4207-be8a-c87940f625bf.013.jpeg)

`             `Fig.10: Optimal Prediction Threshold after SMOT 

The first curve shows a more typical behavior where precision decreases more uniformly as recall increases. The second curve has more variability, and the unusual spike in precision suggests that the model might have a set of thresholds where it is particularly confident, 

![](Aspose.Words.0224bbc6-2498-4207-be8a-c87940f625bf.014.jpeg)

Fig.11: ROC curve 

The area under the ROC curve (AUC) for the trained model is 0.877. This value ranges from 0 to 1, where 1 represents a perfect model and 0.5 represents a model with no skill, equivalent to random guessing. An AUC of 0.877 suggests that the model has a very good ability to  distinguish  between  the  positive  class  and  the negative class. 

When we compare the two models, the difference is clear. The model trained on the balanced dataset post- SMOTE application emerged as more robust for high- value customer churn. 

2. *Key Indicators of Churn* 

We've found some key factors that suggest a customer might  stop  using  our  service.  The  most  significant 

indication we've noticed is the recharge behavior. When a customer recharges less money than usual, it is more likely that they'll decide to stop using that service. It is like they are slowly reducing their commitment to that service provider. 

A decrease in usage, both in calls and data, is a vital indication of customers' declining engagement with the network. This trend is signaling that customers might be looking for a more reliable service provider. Therefore, it is essential to keep a close eye on the usage patterns of customers to retain their trust and loyalty. 

Customer tenure also matters. Shorter tenures suggest a greater risk of churn, indicating newer customers may be more volatile in their loyalty. 

Social factors have a big impact on customer churn. If a customer's network peers are churning, they are more likely to churn too. This shows how social circles can influence customer behavior. 

6. **DISCUSSION**
1. *Interpretation of Results* 

Our research on high-value telecom customers who stop using the service revealed some interesting patterns. We found that they tend to reduce their recharge amounts before completely leaving the service. This means that they  gradually  decrease  their  financial  commitment rather than leaving suddenly. 

When customers start using our services less frequently, it could be a sign that they are losing interest. Before they stop being our customers, they typically reduce the number  of  calls  and  amount  of  data  they  use.  This pattern is crucial because it gives us an opportunity to intervene and prevent churn. 

Newer  customers  are  more  likely  to  stop  using  a company's  services.  Social  networks  can  influence churn  too.  Decisions  made  by  peers  can  influence customers. 

2. *Limitations* 

Our  study  provides  useful  insights  but  has  some limitations. We focused mainly on the Southeast Asian markets, so our findings may not apply to other regions. 

Long-term data that captures customer behavior would give us a more comprehensive understanding than this study, which is just a snapshot in time. Keep in mind that the data we have might have biases, meaning it could  either  overrepresent  or  underrepresent  certain customer groups. This could affect how accurate our predictive models are. 

External  factors  like  market  trends,  economic conditions, and competitive strategies 

7. **CONCLUSION** 

*A.  Summary of Findings* 

Our  research  looked  at  customer  churn  in  the telecommunications  sector,  focusing  on  high-value customers in India and Southeast Asia. We found that customers who recharge their accounts less often and use their phones less frequently are more likely to stop using the service. Shorter customer tenure and social influence were also important factors. 

We used a technique called SMOTE to improve the accuracy of our Logistic Regression model. This helped us deal with data imbalance in churn prediction. 

Our study found that high-value customers tend to stop using the service gradually, rather than all at once. They usually start by using their phone less and spending less money before they stop completely.  

Telecom operators should consider these findings when trying to keep their high-value customers. 

Based  on  our  findings,  telecom  companies  can implement more targeted strategies: 

Monitor  recharge  and  usage  patterns  to  identify potential churn risks. Early intervention programs could be initiated to re-engage these customers. 

Given  the  higher  churn  risk  among  customers  with shorter  tenures,  onboarding  and  early  engagement strategies should be strengthened to build loyalty. 

Understanding the social dynamics and peer influence can help in identifying churn clusters and implementing group-focused retention strategies. 

Recommendations for Future Research 

To build upon our study, we suggest the following areas for further research: 

Expanding the research to include diverse geographic regions would provide a more global perspective on churn behavior. 

Analyzing customer behavior over a longer timeframe could  offer  deeper  insights  into  churn  patterns  and customer lifecycle dynamics. 

Future studies could incorporate external factors like economic  trends  and  competitive  strategies  to understand their impact on customer churn. 

Exploring  advanced  machine  learning  and  artificial intelligence  models,  such  as  deep  learning,  could potentially  uncover  more  complex  patterns  and relationships in churn prediction. 

In conclusion, our study contributes valuable insights into the behavior of high-value customers in the telecom sector,  providing  a  foundation  for  both  targeted retention strategies and future research endeavors. 

**REFERENCES**

1. Vafeiadis, T., Diamantaras, K. I., Sarigiannidis, G., 
   1. Chatzisavvas, K.      C. (2015). A comparison of machine  learning  techniques  for  customer  churn prediction.  Simulation  Modelling  Practice  and Theory, 55, 1-9. 
1. Keramati, A., Jafari-Marandi, R., Aliannejadi, M., Ahmadian, I.,   Mozaffari, M., & Abbasi, U. (2014). Improved churn prediction in telecommunication industry  using  decision  trees  and  logistic regression.  Expert  Systems  with  Applications, 41(14), 6257-6266. 
1. Hadden, J., Tiwari, A., Roy, R., & Ruta, D. (2007). Computer  assisted  customer  churn  management: State-of-the-art  and  future  trends.  Computers  & Operations Research, 34(10), 2902-2917. 
