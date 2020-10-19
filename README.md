# Early Diagnosis of Parkinson’s Disease Progression

<b>Abstract</b>
<br>
Parkinson’s Disease (PD) is triggered due to the loss of dopaminergic neurons in the
substantia nigra, disrupting the neural communication of the central nervous system
towards reception and response of motor and cognitive senses of the patient. PD is a
progressive neural disorder which worsens with ageing. With no clearly outlined pattern
posed in symptoms, it is challenging for medical practitioners to identify the disease in its
prodromal stage. Inspired from the cause, this research’s objective is to predict the rate of
progression based on the baseline assessment of a patient so that an appropriate treatment
plan can be designed for that individual patient. Biomarkers responsible for baseline
assessment are extracted from multiple pre-clinical assessments designed to capture and
scale the motor and cognitive impairments experienced by PD patients during the
prodromal stage. The study performs clustering of PD patients into 3 clusters marking the
rate of progression based on the captured clinical feature of the patients and performance
comparison of 7 different ensembled and neural network-based classification model is
conducted in this study. The study aims to assist medical practitioners in early diagnosis
of risk PD among patients and adopt an appropriate measure to improve patient’s quality
of life.<br><br>

<b>Research Question</b><br>
How well can combined analysis of clinical biomarkers help identify risk of Parkinson’s Disease progression at prodromal stage?
<br><br>
<b>Source of Data</b><br>
Parkinson's Progression Makers Initiative (PPMI) (<a>http://www.ppmi-info.org</a>), Michael J. Fox Foundation for Parkinson’s Research.
Data is fetched from PPMI data repository via dedicated pypmi API package (<a>https://pypmi.readthedocs.io/en/latest/index.html</a>).
<br>

<b>Undrestanding of data</b><br>
Dataset offers a complete evaluation of patient clinical condition from baseline to
5 years follow up visits. Captured data holds the clinical test score of various clinical
assessment trials conducted on the patient to identify different cognitive and motor developed
impairments. Datastore also maintains patient’s genetic data and brain MRI-Scan image data
for purpose of research. However, in this research clinical assessments, data will be used as an
early diagnostic biomarker of PD. Data is collected following standard data acquisition
protocols with consent from the patient regarding the use of data for the purpose of research
work. PPMI holds data for various clinical assessments for over 1800+ patients, belonging to
two prominent categories, suffering from PD and Healthy control (HC).15 clinical assessments capture
the premature motor and non-motor symptoms experienced by PD patients to scale the severity of the disease. 
In this research study important covariates are extracted from these set of assessments.<br>

PPMI monitors symptomatic progression in PD patients at regular intervals. Participation of
the patient at each interval is marked by a unique visit id. During every follow-up visit, patient
is re-accessed for all baseline clinical assessments to capture the change in posed symptoms
and understand the scenario of progression for that individual patient. These scheduled visits
are marked as BL (Basel Line) (Prashanth and Dutta Roy, 2018), which is first-time evaluation
of the patient, later to which each incremental visit is marked between V01 – V12.Participation
of patients declines gradually moving towards the last visit. Also, not each assessment is
mandatorily conducted on every scheduled visit. For the purpose of study, subgroup of 476
patients is created who showed active participation till last visit (V12), eliminating rest of the
patients who quitted the programme halfway. For the purpose of this study, we focus only on Healthy Control
(HC) and Parkinson’s Disease (PD) patients. Also, data available for rest of the category is not
sufficient for analytical study.
