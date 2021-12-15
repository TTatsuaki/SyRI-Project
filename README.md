## What happened? 

Between 2013 and 2019, 26,000 households were wrongly accused by Dutch authorities of committing fraudulent tax benefit claims. Parents received orders which required them to pay back the childcare benefits they received in their entirety, often representing tens of thousands of euros. Moreover, minorities were disproportionately affected as over 8,000 Caribbean-Dutch families were falsely accused. This was due to a risk classification algorithm used for the sake of fraud monitoring that turned out to be discriminatory and filled with institutional biases. 


![picture scandal Netherlands guardians](https://user-images.githubusercontent.com/96054718/146206542-ae0d1175-04c8-4631-a6b4-c8400303308b.png)


![picture BBC fraud scandal (testimony)](https://user-images.githubusercontent.com/96054718/146206561-8e46a6db-4fb7-4c50-8232-c978610499cd.png)



## Legal aspects : Why we decided to talk about this ?

From then on, using nationality was equivalent to differentiate people based on their ethnicity, which is a clear violation of fundamental rights. Yet, the Dutch Tax office was fined €2.75 million only for privacy violations by national courts.

![dutch NP headline](https://user-images.githubusercontent.com/96054718/146206584-707c1a55-7f7e-426a-ae9f-53cccff204c5.png) 

This decision is particularly revealing of a growing problem faced by the law: the difficulty of identifying and punishing algorithmic discrimination despite an already extensive legal arsenal on discrimination issues.
Indeed, discrimination is prohibited in the vast majority of legal systems across the world and also by the Universal Declaration of Human Rights (art. 7), the European Convention of Human Rights (art. 14) and the European Union law (Treaty on European Union, art. 2 and 3 ; Treaty on the functioning of the European Union, art. 10 ;  Charter of Fundamental Rights of the EU, art. 21,  Directive 2004/113/EC that includes prohibition of discrimination in social security and healthcare).

According to the United Nations, a discrimination is « any distinction, exclusion, restriction or preference which is based on any grounds such as race, colour, sex, language, religion, political or other opinion, national or social origin, property, birth or other status, and which has the purpose or effect of nullifying or impairing the recognition, enjoyment or exercise by all persons, on an equal footing, of all rights and freedoms ». The Council of Europe defines it as « treating people in analogous situations differently, or people in different situations alike, without objective and reasonable justification ».  
Therefore, establishing that there has been discrimination presupposes the existence of two elements: unfavourable treatment (I) on the basis of protected ground (II).  
However, it is precisely on this stage that algorithmic discrimination is very challenging for the current law, for two main reasons.

First of all, in most cases, protected ground are not explicitly targeted by the algorithms but often reached through the use of proxies : facially neutral variable that disproportionately harms members of a protected class. Indeed, algorithms base their outputs on a multitude of variables that are all statistically correlated. The basis of a decision is granular and diverse which makes it difficult to relate to a particular protected ground. Fortunately, sometimes proxies are easily attachable to a protected ground (pregnancy-related discrimination is equivalent to sex discrimination for example), but most of them are not. 

Secondly, even if a protected feature is explicitly targeted by the algorithm, the discriminating nature of the outcome remains difficult to grasp. In many cases the decision of the algorithm is based on multiple protected grounds, like sex and ethnicity, or age and sexual orientation for example. Yet, the European courts do not recognize intersectional discrimination as an autonomous category of discrimination. The Cour of Justice of the European Union holds that discrimination is established only when taking one ground in isolation (Parris v. Trinity College Dublin, 2016, Case C-443/15), meanwhile the discriminatory outcome may be due precisely to the combination of several grounds.
European lawyers are currently working on this major difficulty through recommendations and reports (see GERARDS J. and XENIDIS R., Algorithmic discrimination in Europe, Challenges and opportunities for gender equality and non-discrimination law, European Commission, 2021 ; LACROIX J., Prévenir les discriminations résultant de l’utilisation de l’intelligence artificielle, Council of Europe, 2020), but no new legislation has been passed to address the issue of algorithmic discrimination so far.



## The Syri System :

In the case of the SyRI case the risk classification model was a black box system that included a self-learning algorithm. This means the civil servant did not have access to any details about what information had been used as the basis for assigning a specific risk score to an applicant as in a Black box systems, inputs and workings are not visible to the users of the system. Therefore, the self-learning algorithm gave the risk classification model the ability to learn from experiences over time, independently and autonomously, and to make changes to how it worked without these changes being explicitly programmed by the programmers from the tax authorities. 
After investigation by the the Dutch Data Protection Authority (AP), it was established that NATIONALITY was an indicator used in the risk assessment.



## Our project:

Based on a similar idea, we create our own model by using a dataset with enough informations in order to illustrate how discriminatory biases may occur. The data contained in it does not concern the Netherlands, but rather the US. The reason why is that data about european citizen are more difficult to find due to the European legislation. 
We use 5 variables (employment status, level of education, marital status, gender and the country of origin) to which we assign between 2 and 6 options (e.g. married/divorced/never married). To each of these options corresponds a value. Eventually, the addition of the values give us a score that indicate whether or not the individual is likely to fraud.

In a second step, in order to refine our algorithm, we assign a specific coefficient to each variable in that each variable influences the outcome (likelihood to commit fraud) differently. To calculate the weight of each variable, we rely on academic papers that explain statistic relations between Crime rate and different variables. Those studies conducted the Chi-square test which determine whether there is a statistically significant difference (null hypothesis) between the expected frequencies and the observed frequencies. In other words, it shows to which extent  two variables are independent.
After some manipulation of the Chi-square, we conclude that gender is the most influencing variable on the likelihood to commit crime, followed by education, marital status and employment status.
The final step is to add nationality as a determining variable in order to compare results with and without and see how nationality is important and whether the results correlate in both cases.  


