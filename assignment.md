## Overview
The purpose of this assignment is understand the variability in scientific approaches to answering the same question, and to familiarize yourself with some of those approaches. You will be responsible for understanding the details of their procedures, as well as the statistical methods employed. In order to appropriately answer the questions below, you will likely need to **read the papers multiple times**. I suggest that you skim each paper to get a broad understanding, then **re-read the papers** to understand the details. Attempting to answer the questions below without reading the entire paper will both be less accurate and take more time.

## Crowdsourcing Analytics (primary article)

1. Provide an overview of the purpose(s) of this study. Be sure to describe the **specific** contribution it makes to the scientific community. _(8 points)_     

> The purpose of this study is to help better understand how variations in analytical choices affect results. The intention is to show how diverse are the analytical choices of different teams for the same data set and to check whether diversity truly results in many different results. Since different researchers have different analytical skills and backgrounds which affect their choices while investigating it is common to have different outcomes, and thus this study is practical. It is trying to contribute to the scientific community that given the same resources, different approaches may vary in their results due to the inherent presence of subjective bias when making small decisions.

2. Provide an overview of the procedure of this study -- how did it seek to accomplish its purpose? _(8 points)_      

> The study recruits 29 teams to analyze a soccer data set to ask the same question - 'Are dark skin toned players more likely to receive a red card from the referee'. The teams consisted of a very diverse group of 61 data analysts with various academic and work backgrounds. The teams were first independently made to do an analysis for the hypothesis. Then they were asked to peer review others' work and see if there was something intriguing that they had accidentally missed to account for. This was done through email discussions and surveys. Through this, they were able to see how peer reviews and feedback could affect the approaches taken by the researchers. In the end, they were asked to collaboratively work on a final piece. 

3. Describe the structure of the dataset, including how data about skin-tone was represented. Then, identify specific limitations the data has for assessing the hypothesis. _(8 points)_       

> The dataset was obtained from a  company based for sports statistics. It contained the data for player demographics of 2053 soccer players in the first male division. The data also contained 3147 referee interaction for the 2053 soccer players. The final data set with a list with 146028 dyads of players and referees. For the players that had photos, independent raters gave them a scale from 1-5, with 1 for very light skin and 5 for very dark skin. The raters were not made aware of the purpose of research. The scale was then transformed to a scale of 0-1 to reflect the largest possible effect. One limitation could be the differences in the subjective approach of rating a picture on a scale of 1-5.

4. Table 2 shows the frequency of researchers including each covariate in their analysis. Does the distribution surprise you? Why/why not? _(8 points)_       

> I was surprised by the knowledge that only one team used Player as a covariate. I also think victories might be something I would want them to consider as well since in many soccer games the losing teams often become more aggressive than usual. So taking into consideration whether this may account for the red cards might be useful. I was not surprised by the use of a country since it talks a lot about the background and nature of the player. Same goes for age, weight, and height since bigger players might be more vulnerable to receiving a red card since they appear more threatening or aggressive. 

5. Many of the results (of each individual analysis) are reported in terms of an _odds ratio_. Why is this? Define the odds ratio, and interpret (in plain text) what a specific odds ratio indicates (i.e., _"an odds ratio of 1.34 means that...")_). _(8 points)_       

> Odds Ratios are statistically defined as the odds of A in the presence of B and the odds of A in the absence of B. This means that the odds ratio represents the odds that an outcome will occur given a particular exposure, compared to the odds of the outcome occurring in the absence of that exposure. Further, they mean :      

- OR=1 Exposure does not affect odds of an outcome
- OR>1 Exposure associated with higher odds of an outcome
- OR<1 Exposure associated with lower odds of an outcome      


>So, an odds ratio of 2.89, in this case, means that covariates are associated with higher odds of getting a red card. In other words, the odds of a dark-skinned player getting an RC is 2.89 times more likely than the odds of a light-skinned player getting an RC.

6. How did the authors (of the primary study) answer the question, _do teams with more statistical expertise use different approaches or arrive at different conclusions_? Did answers vary by statistical expertise? Be sure to define any technical terms that you use. _(8 points)_      

> The paper showed the variability in statistical expertise did not affect the variability in results. The authors were able to show this by comparing the results of high and comparatively lower levels of quantitative expertise and found that both exhibited high levels of variability in their own estimated effect sizes. Latent class analysis was used to explain the variance across the statistical expertise to help classify them individually into mutually exclusive and exhaustive types, or latent classes, based on their pattern of answers on a set of categorical variables. 

## Supplement 5

1. Using the data/graphics in this section, describe how analysts' beliefs changed over time. Does this surprise you? Does this give you more or less faith in the scientific process? _(8 points)_      

> I was expecting the outcome for the graphics showing the change in analysts' beliefs over the period of study. The hypothesis does sound convincing, however, can be open to question, considering its nature and its relevance to the real world. Hence initially many analysts thought the relationships might be positive. When they started digging further, individually they were facing tough problems and questions and hence may be low confidence let their initial stance weaker. But then as they see others' work as well as discuss amongst each other, they regain their confidence in the hypothesis and come back with stronger opinions with lower standard deviations. This gives me more faith in scientific studies that include discussion and peer review feedback since that increases the overall strength and accuracy of the study as it been reviewed by intellectuals and covers controversial or supporting perspectives as required.

## Team 10 Analysis

1. This team chose to create new variables using the existing one. What new variables did they create, and why did they do this? _(8 points)_   

> 1. Body Mass Index: As stated in one of my previous answers, the chances of a *bigger* or physically stronger player getting a red card might be higher since they appear to be more aggressive or intimidating. The researchers used the standard BMI formula to calculate this suing height and weight of these players.
2. Star Status: This variable also gives a good insight into whether star status could cause any bias in receiving a red card. However, I am not totally in agreement with the formula they used it to create it since it neglects defensive players. For instance, Pepe - a very aggressive defensive player is of star status however, does not have many goals in his records. 
3. Game Status: Again, As previously said, losing teams might often be more aggressive. They calculated this by calculating sperate win-loss and draw percentages. 

2. In this analysis, the authors tested for _confounding_ prior to the analysis. What is a confounding variable, and what did the authors do with variables they found to be confounding? _(8 points)_              

> A confounding variable is an “extra” variable that hasn't been accounted for. These are variables not a part of your set of independent variables but still, have an effect on the outcome/dependent variable. But coming back to the main question of whether skin tones affect the chances of getting a red card, these confounding variables might create useless biases since they have nothing to do with skin tones.  The researchers used the confounding variables as controls. For instance, Star status might affect the chances of getting red but does not relate to the skin tones of the player. Hence the researchers omitted such confounding variables from their study.

3. This study attempted to correct for **nested data**. Describe how the data in this study were _nested_, and how the study accounted for this structure. Then, provide an example of another (hypothetical) dataset which would have a nested structure. _(7 points)_               

> When a variable in the data signifies an observation as belonging to a group it is termed as nested data. In this dataset, the red card data for individual players were nested within different player-referee dyads, and the referees were nested within a variety of countries-of-origins. The necessary level of
nesting for the final model was determined by retaining any grouping variable might explain the significant variance in the red cards above and beyond the simplest level. Additional tests performed then predicted that red cards received from games in the player-referee dyad and coded skin-tone to further evaluate whether modeling the slope of the skin tone as a random effect explained significantly more variance than modeling it as a fixed effect. Another hypothetical nested data set could be a game of Cricket data set with information about players, Umpires and getting a Leg-Before-Wicket from the Umpire. The data would be similar to the soccer data we just saw and could be nested by country, leagues etc. 

## Team 13 Analysis

1. Describe how (and why) this team manipulated the data prior to analysis. Do you believe the transformations performed were appropriate given the research question? _(7 points)_              

> The teams were concerned about interpreting the scale of 1-5 for skin tone as being continuous, interval measure of skin tone. So they dichotomized it to create a new binary variable by choosing values above and below three. I feel this was okay standardization to perform since it gives a broad category of skin tones without going too deep into whether the chances of red cards depend upon *how* dark skin toned you are. But again, decisions may vary by what you are really trying to answer.

2. Provide a **thorough** explanation of the modeling approached used by this team. Be sure to provide a detailed explanation of Poisson regression. _(7 points)_             

> 
1. The first approach was to run a glm with a Poisson link to investigate whether the number of red cards differed by skin tone. This approach also accounted for unlikely positions such as the goalkeeper. Even though the results for dark skin toned were higher, they were not statistically significant (0.11 p-value). 
2. Approach After feedback: The team realized they had neglected repeated instances of referee and players. Secondly, they went back to using the measure of skin tone as a continuous variable than dichotomizing it. The second model ran a Poisson distributed GLM using num of red cards as the dependent variable and log(games) as the offset variable. The results with changes covariates produced a stronger output. 
3. They used Poisson distribution to fit the experimental data because it is suitable to determine the distribution of rare events in a large population.  For example, at any particular time, there is a certain probability that a particular soccer player within the numerous teams might receive a red card.

3. Why did the authors need to _offset_ their Poisson model? _(7 points)_         

> Poisson regression is typically used to model counts data. But, sometimes, it is more relevant to model rates instead of counts. This is relevant when, e.g., individuals are not followed for the same amount of time. In this dataset, this case is valid since each player is not followed for the same amount of time. 
