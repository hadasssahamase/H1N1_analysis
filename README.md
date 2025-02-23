# H1N1_ANALYSIS
![alt text](<Screenshot 2025-02-23 024006.png>)
## Business Problem
- During flu outbreaks, low vaccination rates contribute to increased hospitalizations, economic burdens, and public health crises. 
- Understanding the factors that influence an individual's willingness to get vaccinated is - critical for government agencies, healthcare providers, and pharmaceutical companies.
- Traditional vaccination campaigns rely on broad, one-size-fits-all messaging, which may not effectively target hesitant populations.
- Come up with a model that predicts how likely individuals are to receive their H1N1 vaccine.

## Objectives
- Identify the relationship between risk perception and vaccine uptake.
- Determine if higher knowledge about H1N1 increases the likelihood of getting vaccinated.
- Analyze if concerns about vaccine side effects reduce uptake.
- Segment population groups based on trust in vaccine effectiveness.
- Come up with a model that predicts how likely individuals are to receive their H1N1 vaccine.
 
## The Data
- There are 36 columns in this dataset.
- respondent_id,h1n1_concern, h1n1_knowledge, behavioral_antiviral_meds, behavioral_avoidance,behavioral_face_mask, behavioral_wash_hands, behavioral_large_gatherings, behavioral_outside_home, behavioral_touch_face, doctor_recc_h1n1, doctor_recc_seasonal, chronic_med_condition, child_under_6_months, health_worker, health_insurance, opinion_h1n1_vacc_effective, opinion_h1n1_risk, opinion_h1n1_sick_from_vacc, opinion_seas_vacc_effective, opinion_seas_risk, opinion_seas_sick_from_vacc, age_group, education, race, sex, income_poverty, marital_status,rent_or_own, employment_status, hhs_geo_region, census_msa, household_adults, household_children, employment_industry, employment_occupation.

### DATA PREPARATION.
- Dropping null values 
- Feature Engineering of columns like : safety_behavior_score, doctor_recc_total, health_risk_score,household_vulnerability.

### Interactive Analysis With Tableau

### Data Analysis
![alt text](<Screenshot 2025-02-23 024843.png>)
from the above we can h1n1 knowledge has not significant impact on h1n1 vaccine uptake
![alt text](<Screenshot 2025-02-23 025043.png>)
from the above it eveident that in the age of below 12 are the ones practising safety behavior patterns with females in the lead .

### Modeling
- The modeling was done using two classification models : Logistic regression and Gradient boosting model.
- The key metrics for analysis was receiver operator characteristics curve(roc) where the models performed 0.876953 and 0.873427 roc respectively.
- A cross validation was performed and the results  0.8734025687873294 in logistic regression and  0.8762370756159505 gradient boosting model.
- Later  did a feature importance analysis on gradient boosting model which suggested that socio-demographic factors and individual attitudes are key predictors.  

- Logistic Regression Preferred (Slightly): While both models performed very similarly (ROC AUC around 0.87), logistic regression has a slight edge in cross-validated performance (0.8734 vs 0.8762 for gradient boosting). More importantly, logistic regression offers greater interpretability.- In public health contexts, understanding why a model makes a prediction is often as important as the prediction itself. Therefore, unless there's a strong reason to prioritize the slightly higher (but likely not statistically significant) performance of gradient boosting, logistic regression is the recommended choice.

## Recommendations
1. Target Educational Interventions:
Tailored Messaging: Develop safety behavior campaigns that are specifically tailored to different education levels. Use language, channels, and examples that resonate with each group. For lower education levels, focus on clear, simple messages and practical demonstrations.
Accessible Information: Ensure that information about vaccines and safety behaviors is easily accessible and available in multiple formats (e.g., videos, infographics, community workshops). Consider language barriers and digital literacy levels.
Community Outreach: Partner with community organizations, schools, and local leaders to disseminate information and build trust, especially in communities with lower education levels.
Interactive Education: Implement interactive educational programs that engage individuals and allow them to practice safety behaviors in a safe environment.

2. Address Vaccine Hesitancy by Emphasizing Effectiveness:
Highlight Success Stories: Share real-life stories of how vaccines have prevented serious illnesses and protected communities.
Trusted Messengers: Utilize trusted figures (doctors, nurses, community leaders) to communicate vaccine effectiveness and safety information.
Address Misinformation: Actively combat misinformation and debunk common myths about vaccines using scientific evidence.
Transparency and Openness: Be transparent about the vaccine development process and any potential side effects. Openly address concerns and questions.

3. Communicate Risk Clearly and Empathetically:
Personalized Risk Communication: Help individuals understand their personal risk level based on factors like age, health conditions, and lifestyle.
Emphasize the Benefits of Vaccination: Clearly communicate how vaccination reduces the risk of contracting the disease, experiencing severe symptoms, and spreading it to others.
Address Fears and Concerns: Acknowledge and address common fears and concerns about vaccines, such as side effects and long-term health risks.
Use Emotional Appeals Sparingly but Effectively: Use emotional appeals (e.g., protecting loved ones) judiciously to connect with individuals on a personal level.

4. Reinforce Belief in Vaccine Effectiveness:
Data-Driven Communication: Share data and statistics on vaccine effectiveness in a clear and understandable way.
Expert Endorsements: Highlight endorsements from reputable scientific and medical organizations.
Address Concerns about Safety: Provide information on the rigorous safety testing that vaccines undergo.
Counter Misinformation: Proactively address and correct misinformation about vaccine effectiveness.

5. Empower Individuals to Make Informed Decisions:
Provide Balanced Information: Present information about both the risks and benefits of vaccination, allowing individuals to make informed decisions.
Encourage Dialogue: Create opportunities for open dialogue and discussion about vaccines and safety behaviors.
Respect Individual Choices: While strongly encouraging vaccination and safe behaviors, respect individual choices and avoid coercive tactics.



## For More Information
See the full analysis in the Jupyter Notebook or review this presentation. Contact me at:https://www.linkedin.com/in/amase-oyakapeli-7848a8343/

![alt text](<Screenshot 2025-02-23 023933.png>)


