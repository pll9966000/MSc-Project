# MSc-Project
This repositorie consists of three parts, the source code folder, the data folder and a README.txt.

//code folder//.

1. data_processing_1.jpynb: This code synthesizes the table of basic information on patients with acute renal failure, patients_informations. csv, by manipulating four tables, ADIMISSION.csv, PATIENTS.csv, DIAGNOSES_ICD.csv and D_ITEMS. csv.

2. data_processing_2.jpynb: This part of the code implements the collection of body fluid tests for patients. The three tables, LABEVENTS.csv, D_LABITEMS.csv and the patient_informations.csv, generated in data_processing_1.jpynb, are manipulated to obtain the six laboratory information tables, ph_result.csv, cal_ result.csv, cre_result.csv, glu_result.csv, urea_result.csv and urine_result.csv.

3. data_processing_3.jpynb: This code merges the six tables generated by data_processing_2.jpynb with patients_informations.csv to form the patient table final_data.csv which contains body fluid tests and basic information.

4. data_processing_4.jpynb: This part of the code processes the missing values and outliers from final_data.csv generated by data_processing_3.jpynb to form the standardised tables required to build the model, processed_data2.csv.

5. model design.jpynb: This section is the code to build the model, comparing four models, Decision Tree, KNN, Logistic Regression and Random Forest, to select the best prediction model.

//data folder//.link: 

1. ADIMISSION.csv: Records information from the patient census.

2. PATIENTS.csv: Records patient base information including patient number, date of birth, date of death, and death marker.

3. DIAGNOSES_ICD.csv: records the patient's diagnosis for a particular admission.

4. D_ICD_DIAGNOSES.csv: Dictionary table corresponding to the ITEMS in DIAGNOSES_ICD.csv.

5. LABEVENTS.csv: Record of the patient's laboratory data.

6. D_LABITEMS.csv: dictionary table corresponding to ITEMS in LABEVENTS.csv.

7. patients_informations.csv: table of results generated by a run of data_processing_1.jpynb. It contains basic information about the patient.

8. ph_result.csv: The rate of abnormal pH in blood tests for patients with acute renal failure.

9. cal_result.csv: Rate of calcium abnormalities in blood tests for patients with acute renal failure. 

10. cre_result.csv: Rate of creatinine abnormalities in blood tests in patients with acute renal failure.

11. glu_result.csv: Rate of abnormal glucose in blood tests in patients with acute renal failure. 

12. urea_result.csv: Rate of abnormal urea nitrogen in blood tests in patients with acute renal failure.

13. urine_result.csv: The rate of abnormal urine in patients with acute renal failure.

14. final_data.csv: A patient table containing body fluid tests and underlying information, created by merging the six tables generated by data_processing_2.jpynb with patients_informations.csv.

15. processed_data2.csv: The results were obtained by processing the null values from final_data.csv. This table can be used for model building.

16. Synthetic_data_1.csv: Simulation data for testing the usability of the model (from a project by a member of the same group).
