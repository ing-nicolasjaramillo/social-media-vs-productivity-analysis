Social Media vs Productivity Analysis

This project explores the relationship between social media usage, productivity, sleep habits, stress levels, and job satisfaction using the Kaggle dataset Social Media vs Productivity.

The analysis focuses on:

Data quality assessment.
Missing value treatment.
KNN-based imputation.
Exploratory Data Analysis (EDA).
Correlation analysis.
Validation of productivity and sleep-related hypotheses.
Dataset

Dataset obtained from Kaggle:

Dataset: Social Media vs Productivity
Author: Mahdi Mashayekhi

Download command:

kaggle datasets download -d mahdimashayekhi/social-media-vs-productivity -p social_media_productivity --unzip

Research Questions
H1 – Sleep and Productivity

Do professionals in Healthcare and IT experience different productivity impacts when suffering from sleep deprivation?

H2 – Technology Exposure and Stress

Do IT professionals experience fewer offline hours and higher stress levels compared to non-technical profiles?

H3 – Breaks and Job Satisfaction

Is there a positive relationship between work breaks and job satisfaction? Do breaks help mitigate stress?

Data Quality Process
Completeness

The following variables contained missing values:

daily_social_media_time
perceived_productivity_score
actual_productivity_score
stress_level
sleep_hours
screen_time_before_sleep
job_satisfaction_score
Initial Approach

Median imputation grouped by job type.

Improved Approach

KNN Imputation using:

One-Hot Encoding
StandardScaler
KNNImputer (k=40)

This method preserved the original distributions more effectively than median imputation.

Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-Learn
KNNImputer
StandardScaler


## Hypothesis Results
H1: Sleep vs Productivity

Not supported by the dataset.

Both Healthcare and IT groups showed nearly flat productivity trends regardless of sleep duration.

H2: Offline Hours vs Stress

Not supported.

Correlation between weekly offline hours and stress level was approximately zero.

H3: Breaks vs Job Satisfaction

Not supported.

No meaningful correlation was observed between work breaks and job satisfaction.
