## What happened? 
Around the world, algorithmic decision-making systems are increasingly deployed to automate governmental tasks and to identify, detect, and punish people that meet a presupposed profile of alleged criminal activity. What variables are deployed to construct a "presupposed profile", are often human determined, and thus prone to bias. Governments are increasingly using such algorithmic decision-making system with a particular objective to combat fraud. In the Netherlands, fraud became increasingly more important within political debate since the early 2000's. Consequently, stricter policy measurements to combat fraud were developed. 
In turn, the use of such algorithmic decion-making systems can lead to unforeseen consequences, especially if these models are programmed with an unexpected bias.
In the Netherlands, such a case has come to forefront: it is known as the "Dutch Childcare benefits schandal" (Dutch: de Toeslagenaffaire)
In 2013, an algorithmic decision-making system for fraud detection was adopted: the “risk classification model”. (In English, also known as SyRI: "system risk indication")

Between 2013 and 2019, 26,000 households were wrongly accused by Dutch authorities of committing fraudulent tax benefit claims. Parents received orders which required them to pay back the childcare benefits they received in their entirety, often representing tens of thousands of euros. 
The financial repercussions for these parents were often so high, that this affected their personal life severely. Many parents reported to have had mental health issues, divorce, or even considered suicide. 

Moreover, minorities were disproportionately affected as over 8,000 Caribbean-Dutch families were falsely accused. 
It has thus come to light, that the scandal included racial profiling by the risk classification model, which is the focus of our project. 
The tax authorities used information on whether an applicant had Dutch nationality as a risk factor in the algorithmic system. “Dutch citizenship: yes/no” was used as a parameter in the risk classification model for assessing the risk of inaccurate applications. Consequently, people of non-Dutch nationalities
received higher risk scores. 



![picture scandal Netherlands guardians](https://user-images.githubusercontent.com/96054718/146206542-ae0d1175-04c8-4631-a6b4-c8400303308b.png)


![picture BBC fraud scandal (testimony)](https://user-images.githubusercontent.com/96054718/146206561-8e46a6db-4fb7-4c50-8232-c978610499cd.png)


## Literature review 

To analyse how the childcare benefits algorithm worked, we have tried to investigate reports from independent oversight bodies: 
firstly, the report Dutch Data Protective Authorities (AP), which was the only source available that directly conducted research with the Dutch Tax Authortities to analyse the algorithm in question. 
Secondly, a report by the Amnesty International organization, who did an extensive review on why the algorithm harmed the protection of human rights, analyzed the algorithm etensively by compiling a range of relevant sources, as well as using the case as an argument to put forth concrete demand within the European Union to refrain governments from using self-learning decison-making algorithms where nationality is used as a risk-determinant. 
Thirdly, we have used a multitude of legal cases in order to understand the legal implications of the algorithm. 


## Legal aspects : Why we decided to talk about this ?

From then on, using nationality was equivalent to differentiate people based on their ethnicity, which is a clear violation of fundamental rights. Yet, the Dutch Tax office was fined €2.75 million only for privacy violations by national courts, and led to the collapse of the Dutch government. 

![dutch NP headline](https://user-images.githubusercontent.com/96054718/146206584-707c1a55-7f7e-426a-ae9f-53cccff204c5.png) 

This decision is particularly revealing of a growing problem faced by the law: the difficulty of identifying and punishing algorithmic discrimination despite an already extensive legal arsenal on discrimination issues.
Indeed, discrimination is prohibited in the vast majority of legal systems across the world and also by the Universal Declaration of Human Rights (art. 7), the European Convention of Human Rights (art. 14) and the European Union law (Treaty on European Union, art. 2 and 3 ; Treaty on the functioning of the European Union, art. 10 ;  Charter of Fundamental Rights of the EU, art. 21,  Directive 2004/113/EC that includes prohibition of discrimination in social security and healthcare).

According to the United Nations, a discrimination is « any distinction, exclusion, restriction or preference which is based on any grounds such as race, colour, sex, language, religion, political or other opinion, national or social origin, property, birth or other status, and which has the purpose or effect of nullifying or impairing the recognition, enjoyment or exercise by all persons, on an equal footing, of all rights and freedoms ». The Council of Europe defines it as « treating people in analogous situations differently, or people in different situations alike, without objective and reasonable justification ».  
Therefore, establishing that there has been discrimination presupposes the existence of two elements: unfavourable treatment (I) on the basis of protected ground (II).  
However, it is precisely on this stage that algorithmic discrimination is very challenging for the current law, for two main reasons.

First of all, in most cases, protected ground are not explicitly targeted by the algorithms but often reached through the use of proxies : facially neutral variable that disproportionately harms members of a protected class. Indeed, algorithms base their outputs on a multitude of variables that are all statistically correlated. The basis of a decision is granular and diverse which makes it difficult to relate to a particular protected ground. Fortunately, sometimes proxies are easily attachable to a protected ground (pregnancy-related discrimination is equivalent to sex discrimination for example), but most of them are not. 

Secondly, even if a protected feature is explicitly targeted by the algorithm, the discriminating nature of the outcome remains difficult to grasp. In many cases the decision of the algorithm is based on multiple protected grounds, like sex and ethnicity, or age and sexual orientation for example. Yet, the European courts do not recognize intersectional discrimination as an autonomous category of discrimination. The Cour of Justice of the European Union holds that discrimination is established only when taking one ground in isolation (Parris v. Trinity College Dublin, 2016, Case C-443/15), meanwhile the discriminatory outcome may be due precisely to the combination of several grounds.
European lawyers are currently working on this major difficulty through recommendations and reports (see GERARDS J. and XENIDIS R., Algorithmic discrimination in Europe, Challenges and opportunities for gender equality and non-discrimination law, European Commission, 2021 ; LACROIX J., Prévenir les discriminations résultant de l’utilisation de l’intelligence artificielle, Council of Europe, 2020), but no new legislation has been passed to address the issue of algorithmic discrimination so far.



## The SyRI System:

The risk classification model was a black box system that included a self-learning algorithm. This means the civil servant did not have access to any details about what information had been used as the basis for assigning a specific risk score to an applicant as in a Black Box systems, inputs and workings are not visible to the users of the system. Therefore, the self-learning algorithm gave the risk classification model the ability to learn from experiences over time, independently and autonomously, and to make changes to how it worked without these changes being explicitly programmed by the programmers from the tax authorities. 

The risk classification model was developed by comparing historic examples of correct and incorrect
applications. In practice, this meant that the more an incoming application resembled an application that had previously been classified as inaccurate, the higher the risk score assigned to that incoming application. The system selected applications with the highest risk scores for manual review by a civil
servant. The civil servant in turn had the power to label an application as fraudulent. The civil servant, however, was given no information as to why the system had given the application a high-risk score for inaccuracy.

The nationality of the applicant was used to determine whether that person was a Dutch citizen. “Dutch citizenship: yes/no” was used as a parameter in the risk classification model for assessing the risk of inaccurate applications. 




Consequently, the case of the algorithm was brought by several civil rights organizations, including the Netherlands Committee of Jurists for Human Rights (Nederlands Juristen Comité voor de Mensenrechten, NJCM), and two natural persons against the Dutch government. At first, the Hague Court issued a decision on 5 February 2020 acknowledging that the government had breached the right to privacy and family life set out in Article 8 of the ECHR and ordered  that it cease using this algorithm. The judges based their decision on the fact that the algorithm Syri lacked transparency. The court did not address a possible breach of Article 22 of the GDPR which bans automated decision-making in some cases, nor held that the system was clearly discriminating even though, the use of nationality was equivalent to differentiate people based on their ethnicity, which is a clear violation of the principle of non-discrimination. 

After investigation by the the Dutch Data Protection Authority (DPA), it was established that nationality was an indicator used in the risk assessment. The use of nationality as risk factors in risk-scoring models to identify possible fraudulent or criminal behaviour of individuals or groups which reveals the assumptions held by the designer, developer and/or user of the risk-scoring system that people of certain nationalities would be more likely to commit fraud or crime than people of other nationalities. Nationality was used as an element to target certain groups of people, based on the idea that these groups were supposedly sharing certain common cultural values, traditions and that because of those values and traditions there would be more likely to commit fraud. 

Recently, on 8 December 2021, DPA has imposed a €2.75 million fine on the Dutch Tax Administration. The fine was imposed because for many years the Tax Administration processed data on the (dual) nationality of childcare benefit applicants in an unlawful, discriminatory and therefore improper manner. This constituted serious violations of the General Data Protection Regulation (GDPR), the law governing privacy. In particular, the DPA stated that « by unnecessarily retaining nationality data in its systems, the Tax Administration acted in a discriminatory way.  And recalled that « entitlement to childcare benefit is not contingent on nationality but on lawful residence in the Netherlands ». Alfeid Wolfsen, chair of the DPA declared that « this case shows exactly why: unlawful processing by means of an algorithm led to a violation of the right to equality and non-discrimination ». This is what we want to get into in our work. 



## Methodology:

Despite the fact the Dutch authorities have not revealed the other variables used to determine risk-factor of the Dutch citizens, we have decided to model likely database entries that are used. The relevant variables are illustrated below. 

Consequently, we are creating our model to model the risk-classication algorithm by using a dataset with enough informations in order to illustrate how discriminatory biases may occur. The data contained in it does not concern the Netherlands, but rather the US. The reason why is that data about european citizen are more difficult to find due to the European legislation (GDPR). 
We use 5 variables:
- employment status
- level of education
- marital status
- gender 
- country of origin

to which we assign between 2 and 6 variablities (e.g. married/divorced/never married).
To each of these options corresponds a weight to the likeliness of comitting fraud. 
The range of the weight is **between 0 and 1** -- 0 being most likely to commit fraud, 1 being least likely to commit fraud. 
The range of these values are chosen in order to stay close to the orginal Dutch SyRI model, which assigned the weight of likeliness of fraud between 0 and 1 as well. 
Eventually, the overall aggragated weight give us a score that indicate whether or not the individual in the model is likely to fraud.





//
In a second step, in order to refine our algorithm, we assign a specific coefficient to each variable in that each variable influences the outcome (likelihood to commit fraud) differently. To calculate the weight of each variable, we rely on academic papers that explain statistic relations between Crime rate and different variables. Those studies conducted the Chi-square test which determine whether there is a statistically significant difference (null hypothesis) between the expected frequencies and the observed frequencies. In other words, it shows to which extent  two variables are independent.
After some manipulation of the Chi-square, we conclude that gender is the most influencing variable on the likelihood to commit crime, followed by education, marital status and employment status.
The final step is to add nationality as a determining variable in order to compare results with and without and see how nationality is important and whether the results correlate in both cases.  
//


## Results 

[Link To Our Notebook](https://colab.research.google.com/drive/1OuCX3T0kGAYSRSNwVhUgN3KRQ-dfbw4U#scrollTo=hwVdMgJX7LnR)

![alt text](http://url/to/img.png)




## Conclusion

All in all, the childcare benefits affair of the Netherlands has certainly supported the argument that AI
algorithms can be discriminatory, and that they can cause severe implications. With the increase of
the use of algorithms in data processing of governments and institutions, the risk of discrimination to
become more evident is very logical, considering most bias already preexisted within the institutions
that adopted the biased systems.

