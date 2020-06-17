# H1b-Petitions

It contains five year's worth of H-1B petition data, with approximately 3 million records overall. The columns in the dataset include case status, employer name, worksite coordinates, job title, prevailing wage, occupation code, and year filed.

The H1B Visa is a highly desired non-immigrant visa which permits foreign workers in specialty occupations to enter the country. H-1B visas are a category of employment-based, non-immigrant visas for temporary foreign workers in the United States. For a foreign national to apply for H1-B visa, a US employer must offer them a job and submit a petition for a H-1B visa to the US immigration department. This is also the most common visa status applied for and held by international students once they complete college or higher education and begin working in a full-time position.

We will perform exploratory data analysis with python to get insights from data.

# Tools and Libraries Used
We have used the following python packages to perform the exploratory data analysis

* Pandas
* Matplotlib
* Seaborn
* Sklearn

# Files

The repository contains two files other than the readme file
H1b-Petition-Prediction.ipynb: Jupyter Notebook file contains all the python code, documentation and visualization
h1b_kaggle.csv: Our dataset file

Dataset contains the following features:

* CASE_ID - A unique case ID for every applicant.
* CASE_STATUS – The target variable consists of 6 different classes or values. Status is associated with the last significant event.
* EMPLOYER_NAME – Name of the employer submitting the application.
* SOC_NAME – Occupational name associated with an occupational code
* JOB_Title – Title of the Job
* FULL_TIME_POSITION – Whether the position is full time or not
* PREVAILING_WAGE - The prevailing wage for a job position is defined as the average wage paid to similarly employed workers in the requested occupation in the area of intended employment
* YEAR – Year in which h1b petition was filed
* WORKSITE - City and State information of the foreign worker’s intended area of employment
* Lon – Longitude of the worksite
* Lat – Latitude of the worksite

# Result

During the model training, RandomForestClassifier performs better than Guassian and LogisticRegression, analyzed using ROC curve.

We learned that:

* The H1b-petitions have increased from the year 2011-2016
* H1-B petitions filed by the universities have more chances of getting accepted
* California, Texas and NewYork tops the list in filing of the H1b-petitions, as they are known for the IT companies
* Majority of the people who applied for h1b were in full time role.

# Dataset Information

The dataset was posted on kaggle. It is avaiable to download here [H1-B Dataset](https://www.kaggle.com/nsharan/h-1b-visa/data)

# Improvements and Future Work
Due to low machine capability, proper handling of the imbalanced dataset can be performed using SMOTE or Over sampling instead of undersampling which can result loss of information.
