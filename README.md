##Content: 

Between 2013 and 2019, 26,000 households were wrongly accused by Dutch authorities of committing fraudulent tax benefit claims. Parents received orders which required them to pay back the childcare benefits they received in their entirety (often 10’s of thousands of euros). Minorities were disproportionately affected as over 8,000 Caribbean-Dutch families were falsely accused. This was due to a risk classification algorithm used for the sake of fraud monitoring that turned out to be discriminatory and filled with institutional biases. 

##The Syri System :

The risk classification model was a black box system that included a self-learning algorithm. This means the civil servant did not have access to any details about what information had been used as the basis for assigning a specific risk score to an applicant as in a Black box systems, inputs and workings are not visible to the users of the system. Therefore, the self-learning algorithm gave the risk classification model the ability to learn from experiences over time, independently and autonomously, and to make changes to how it worked without these changes being explicitly programmed by the programmers from the tax authorities. 
After investigation by the the Dutch Data Protection Authority (AP), it was established that NATIONALITY was an indicator used in the risk assessment.


##Our project:

Based on a similar idea, we create our own model by using a dataset with enough informations in order to illustrate how discriminatory biases may occur. We use 5 variables (employment status, level of education, marital status, gender and the country of origin) to which we assign between 2 and 6 options (e.g. married/divorced/never married). To each of these options corresponds a value. Eventually, the addition of the values give us a score that indicate whether or not the individual is likely to fraud.
In a second step, in order to refine our algorithm, we assign a specific coefficient to each variable in that each variable influences the outcome (likelihood to commit fraud) differently. To calculate the weight of each variable, we rely on academic papers that explain statistic relations between Crime rate and different variables. Those studies conducted the Chi-square test which determine whether there is a statistically significant difference (null hypothesis) between the expected frequencies and the observed frequencies. In other words, it shows to which extent  two variables are independent.
After some manipulation of the Chi-square, we conclude that gender is the most influencing variable on the likelihood to commit crime, followed by education, marital status and employment status.
The final step is to add nationality as a determining variable in order to compare results with and without and see how nationality is important and whether the results correlate in both cases.  


##Why are biased algorythm an issue?
