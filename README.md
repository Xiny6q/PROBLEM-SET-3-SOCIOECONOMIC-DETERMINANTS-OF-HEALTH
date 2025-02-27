Download link :https://programming.engineering/product/problem-set-3-socioeconomic-determinants-of-health/

# PROBLEM-SET-3-SOCIOECONOMIC-DETERMINANTS-OF-HEALTH
PROBLEM SET 3: SOCIOECONOMIC DETERMINANTS OF HEALTH
This problem set explores the socioeconomic correlates of health status in the United States. The dataset https://github.com/tvogl/econ121/raw/main/data/nhis2010.Rdata contains a sample of adults from the 2010 National Health Interview Survey, with mortality follow-up to 2019. You will analyze two outcome variables:

mortality and (2) self-reported health status. Self-reported health status is based on the question: “On a scale of 1 (excellent) to 5 (poor), how would you rate your health?” The dataset contains many interesting covariates, including measures of socioeconomic status, race, health behaviors, and health conditions. You will notice that the dataset has sampling weights, but we will not use them here to keep matters simple.

To install R and RStudio, follow this link. You are encouraged to work in a group of up to 4 members. You may write code together, but you must write verbal answers yourself. Please use a Markdown template for your code. Write verbal answers in the comments within the Markdown file, so that you produce a single PDF with code, results, and writing, which you will upload to Gradescope.

List your group members.

Load packages and the dataset. Generate a binary variable that equals 1 if the respondent reports fair or poor health and 0 otherwise. Summarize the data and describe your findings in at most 4 sentences.

To get a sense of how self-reported health status relates to mortality risk over the lifecycle, compute mortality rates by age in two separate groups: (a) people who report being in fair-to-poor health and (b) people who report being in good-to-excellent health. Then draw separate line plots of the mortality-age relationship for the two groups in the same graph. How does the risk of death change with age? Do people with worse self-reported health status have higher risk of death? Answer in at most 4 sentences.

Draw four bar graphs to describe how average fair/poor health and mortality vary by socioeconomic status. In ggplot(), you should use geom_bar(stat = “identity”). For each of the four graphs, describe your results and take note of any unexpected patterns in 2-3 sentences.

Graph rates of mortality and fair/poor health by the level of family income.

Graph rates of mortality and fair/poor health by education level, with five categories of educational attainment: less than high school completion (<12), high school completion (12), some college (13-15), college completion (16), and post-graduate study (>16).

Age, income, education, and race/ethnicity are correlated, so we must use multiple regression to disen-tangle the relative importance of these variables in predicting health. For both mortality and fair/poor health, run linear probability models, probit models, and logit models with age, education, family in-come, and race/ethnicity as independent variables. Choose an appropriate functional form for age and education (linear, categorical, etc.), and be sure to motivate your choice in your written answer. (Re-member that complicated functional forms are sometimes diﬃcult to interpret, and interpretability is valuable. Sometimes it is useful to split a continuous variable into a series of dummy variables for diﬀerent ranges.) For the probit and logit models, also compute the marginal eﬀects of the independent variables. For the logit model, further compute the odds ratios of the independent variables. Describe your results and take note of any expected or unexpected patterns. Are the LP, probit, and logit results similar? Answer in at most 5 sentences.

At the same age, who has a greater mortality risk? Is the diﬀerence in mortality risk statistically

significant?

Group A: Asian adults with less than 12 years of education and family incomes less than $35k

Group B: Black adults with 16 years of education and family incomes over $100k

Use your logit estimates from question (5) to answer. Do you think this model with no interaction terms is the best one for testing for diﬀerences between these groups? If not, how would you alter it? Answer in at most 4 sentences.

Should we think of the coeﬃcients (or marginal eﬀects or odds ratios) on family income as causal? Why or why not? Answer in at most 4 sentences.

Many wonder how much of the relationship between socioeconomic status and mortality reflects diﬀer-ences in health insurance or diﬀerences in health behaviors. Using a logit model and reporting odds ratios, explore how much of the mortality relationship these mediating variables can explain. Make sure you are able to interpret the results of the technique you use. Describe your results in at most 4 sentences.
