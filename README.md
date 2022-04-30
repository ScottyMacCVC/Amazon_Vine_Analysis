# Amazon_Vine_Analysis

## Overview of the analysis: Our task is to analyze Amazon reviews written by members of the paid Amazon Vine program. The service provides manufacturers and publishers a direct way to receive reviews of their products. For a small fee, Amazon will connect end users to products under the Amazon Vine membership. Members are required to give reviews and feedback on all products received through the program. Our goal is to access 50-or-so datasets, gather the review of a specific product, and perform an analysis. The analysis is a combination of ETL through PySpark, connection to Amazons' AWS RDS database instance, and then loaded into pgAdmin. We will take the data and determine whether there is bias toward favorable reviews. 

### Results - We will directly answer the questions below regarding Vine & Non-Vine Reviews:

![Vine Reviews 1](https://github.com/ScottyMacCVC/Amazon_Vine_Analysis/blob/main/Resources/Vine_Review_1.PNG) 
![Vine Reviews 2](https://github.com/ScottyMacCVC/Amazon_Vine_Analysis/blob/main/Resources/Vine_Review_2.PNG) 

- How many Vine reviews and non-Vine reviews were there? Non-vine reviews (40,471) greatly outweighs vine reviews (94).

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars? Non-vine reviews received 15,663, 5-star reviews, and vine review received 48.

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars? Non-vine reviews received 38.7%, 5-star reviews, and vine review received 51.1%.


### Summary: We need to determine if there is any positivity bias for reviews in the Vine program. We will use the results of our analysis to support our statement. We will also provide one additional analysis that we could do with the dataset to support our statement.

Based on the data, there is little-to-no observable bias toward vine users. The assumption is limited to our current analysis, the numbers of users are greatly different, but the 5-star % delta between non-vine & vine user reviews was negligible. The vine users tend to show a more positive result, but the difference between the non-vine reviews was about 12%. Although there is a difference, we should not gather this information as statistical proof of bias. It would be best to do a additional investigation. One suggestion would be use a correlation coefficient and look at the multivariate statistics of the data set. The test would let us summarize sample data without inferring anything about the population. We also see an effect size measure, whuch tells us the practical significance of a result and allows us to plot the summary results. 
