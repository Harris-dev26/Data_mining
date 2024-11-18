# Data_mining notes:
https://docs.google.com/document/d/15p6dBtKLRjs9QrQgWpXvkawDH2oMKg-pY6WiIyBc-6U/edit?tab=t.0

This is the link for discussion notes.


Data has these columns:

columns = 
    
     
     "ID","Gender", "Age_Group", "Residence", "Education_Level", "Source_of_Income","Marital_Status",
     "Smoked_Cigarettes", "Year_Diagnosed", 
     
     "Surgical_Treatment","Chemotherapy", "Radiotherapy", "Immunotherapy", "Molecular_targeted_Therapy",

    "Hospitalization_Number", "Time_to_Treatment", "Medical_Treatment_Need",

    "Emotional_Impact", "Travel_Impact", "Quality_of_Life", 
    "Symptoms_exp_cough", "Symptoms_exp_Hoarseness","Symptoms_exp_Blood_cough","Symptoms_exp_chestpain" ,"Symptoms_exp_Shortness_of_breath","Symptoms_exp_weakness","Symptoms_exp_None",

    "Symptom_Frequency", "Symptom_Household_Impact", "Sleep_Issues", "Support_From_Close",
    "Dependency_Fear", "Health_Satisfaction", 
    "Daily_Life_Impact_physical","Daily_Life_Impact_Psychological",
    "Daily_Life_Impact_proffesional","Daily_Life_Impact_family_life","Daily_Life_Impact_social_life",
    "Daily_Life_Impact_no_effect",
    
    "Energy_Level", "Self_Care", "Daily_Activities_Difficulty",
    "Work_Readiness", "Support_Satisfaction", "Coping_Strategy", "Negative_Emotions"


1- These can be grouped into:
- demographic features: 
- Therpahy type features:
- Symptom exp:
- Daily_Life_Impact:
- Emotions, Satisfaction ...
- ??

# We will try to make a target feature looking at these groups above. nunique() results can give us an idea:
may be we can consider : Symptomps and Daily Life impact can be reorganized as a single categorical column?

gender                              2
age_group                           4
residence                           4
education_level                     4
source_of_income                    4
marital_status                      4
smoked_cigarettes                   2
year_diagnosed                      7
surgical_treatment                  2
chemotherapy                        2
radiotherapy                        2
immunotherapy                       2
molecular_targeted_therapy          2
hospitalization_number              4
time_to_treatment                   3
medical_treatment_need              4
emotional_impact                    2
travel_impact                       2
quality_of_life                     4
symptoms_exp_cough                  2
symptoms_exp_hoarseness             2
symptoms_exp_blood_cough            2
symptoms_exp_chestpain              2
symptoms_exp_shortness_of_breath    2
symptoms_exp_weakness               2
symptoms_exp_none                   2
symptom_frequency                   4
symptom_household_impact            4
sleep_issues                        4
support_from_close                  2
dependency_fear                     4
health_satisfaction                 2
daily_life_impact_physical          2
daily_life_impact_psychological     2
daily_life_impact_proffesional      2
daily_life_impact_family_life       2
daily_life_impact_social_life       2
daily_life_impact_no_effect         2
energy_level                        4
self_care                           4
daily_activities_difficulty         4
work_readiness                      3
support_satisfaction                3
coping_strategy                     3
negative_emotions                   4




We can look at the highly correlated values.. 
