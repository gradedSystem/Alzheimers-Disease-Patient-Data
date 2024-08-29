---
datapackage:
  title: Alzheimer's Disease Patient Data
  description: This dataset contains health records for 2,149 patients identified by unique ID numbers (4751-6900), providing extensive information on demographics, lifestyle, medical history, clinical measurements, cognitive and functional assessments, symptoms, and diagnostic data related to Alzheimer's disease.
  created: 2024-08-29
  updated: 2024-08-29
  licenses:
  - path: https://creativecommons.org/licenses/by/4.0/
    title: Attribution 4.0 International (CC BY 4.0)
  sources:
  - path: https://www.kaggle.com/datasets/muhammadehsan02/alzheimers-disease-patient-data
    title: Alzheimer's Disease Patient Data
  resources:
  - name: alzheimer-disease-patient-data
    title: Alzheimer's Disease Patient Data
    description: This dataset is a comprehensive collection of health records for 2,149 patients who have been diagnosed with or are at risk for Alzheimer's disease. Each patient in the dataset is uniquely identified with an ID number ranging from 4751 to 6900. The dataset covers a wide range of information that is crucial for understanding the various factors associated with Alzheimer's disease. It includes demographic details, lifestyle habits, medical history, clinical measurements, cognitive and functional assessments, symptoms, and diagnostic information.
    lastModified: 2024-08-29
    path: alzheimers_disease_patient_data.csv
---

# Alzheimer's Disease Patient Data Analysis

## Overview

This analysis explores a dataset related to Alzheimer's disease patients. We examine various factors, including age, gender, health metrics, and diagnostic information, to uncover trends and patterns.

## Age Distribution

Age is a significant factor in understanding Alzheimer's disease. The chart below displays the distribution of patients across different age ranges:

<PlotlyBarChart
  data={{
    file: 'alzheimers_disease_patient_data.csv',
    columns: ['Age', 'PatientID']
  }}
  title="Age Distribution of Patients"
  xAxis="Age"
  yAxis="Count"
/>

## Gender Breakdown

The distribution of gender among patients is illustrated in the chart below. This provides insights into the gender proportion within the dataset:

<PlotlyBarChart
  data={{
    file: 'alzheimers_disease_patient_data.csv',
    columns: ['Gender', 'PatientID']
  }}
  title="Gender Distribution of Patients"
  xAxis="Gender"
  yAxis="Count"
/>

## BMI and Alzheimer's Diagnosis

Body Mass Index (BMI) is an important health metric. The following chart shows the distribution of BMI among Alzheimer's patients. This helps in understanding how BMI varies across different diagnostic statuses:

<PlotlyBarChart
  data={{
    file: 'alzheimers_disease_patient_data.csv',
    columns: ['BMI', 'Diagnosis']
  }}
  title="BMI Distribution by Alzheimer's Diagnosis"
  xAxis="BMI"
  yAxis="Count"
/>

## Age vs. MMSE Scores

Mini-Mental State Examination (MMSE) scores are used to assess cognitive function. The chart below examines the distribution of MMSE scores across different age groups:

<PlotlyBarChart
  data={{
    file: 'alzheimers_disease_patient_data.csv',
    columns: ['Age', 'MMSE']
  }}
  title="MMSE Scores Distribution by Age"
  xAxis="Age"
  yAxis="MMSE Scores"
/>

## Distribution of Health Metrics

The dataset includes various health metrics, such as cholesterol levels and blood pressure. The following charts display the distribution of these metrics among patients:

<PlotlyBarChart
  data={{
    file: 'alzheimers_disease_patient_data.csv',
    columns: ['CholesterolTotal', 'PatientID']
  }}
  title="Cholesterol Levels Distribution"
  xAxis="CholesterolTotal"
  yAxis="Count"
/>

<PlotlyBarChart
  data={{
    file: 'alzheimers_disease_patient_data.csv',
    columns: ['SystolicBP', 'DiastolicBP']
  }}
  title="Blood Pressure Distribution"
  xAxis="Blood Pressure"
  yAxis="Count"
/>

## Patient Demographics

For a comprehensive view of patient demographics, including age, gender, and other factors, refer to the table below:

<FlatUiTable
  data={{
    file: 'alzheimers_disease_patient_data.csv'
  }}
/>

## Conclusion

The analysis of the Alzheimer’s disease patient data provides valuable insights into how age, gender, and health metrics relate to the diagnosis. Further investigation into these patterns can aid in understanding the risk factors associated with Alzheimer's disease and potentially guide future research and treatment approaches.
