## About

The Randomized Intervention with CPAP in Coronary Artery Disease and Obstructive Sleep Apnea (RICCADSA) trial is a prospective, single-center randomized controlled trial conducted in Sweden between 2005 and 2013. It enrolled 511 adult patients with angiography-verified coronary artery disease (CAD) who underwent percutaneous coronary intervention (PCI) or coronary artery bypass grafting (CABG) within 6 months prior to study start. The cohort includes patients diagnosed with obstructive sleep apnea (OSA) based on home sleep apnea testing (HSAT) or polysomnography (PSG): 399 patients with OSA (apnea–hypopnea index [AHI] ≥ 15 events/hr) and 112 without OSA (AHI \< 5 events/hr). Patients with borderline OSA (AHI 5.0–14.9) or predominantly central apneas were excluded. The main objective of the study was to assess whether continuous positive airway pressure (CPAP) treatment reduces long-term adverse cardiovascular outcomes. Participants were stratified by symptomatic status (Epworth Sleepiness Scale [ESS] ≥10 defined as sleepy, \<10 as nonsleepy). Nonsleepy OSA patients (n=200) were randomized 1:1 to CPAP treatment or no CPAP (control). Sleepy OSA patients (n=155) were offered CPAP in an observational arm. Subjects without OSA served as controls. Sleep studies were done both in-home (HSAT via Embletta portable digital system) and in-lab (overnight PSG) using standardized protocols Primary outcomes included a composite of new revascularization, myocardial infarction (MI), stroke, and cardiovascular mortality over an average follow-up of approximately 4.7 years. Secondary outcomes included cardiovascular biomarkers, left ventricular function, maximal exercise capacity, anxiety, depression, quality of life, detailed sleep parameters, and adherence to CPAP therapy. Main study assessments were performed at baseline, 3 months, and 1 year, with additional collected annually for up to 6 years.

## Methods

### Clinic Visits/Data Collection

-   Screening HSAT performed at home with Embletta® device.
-   Participants with HSAT AHI ≥ 15/h and nonsleepy phenotype were randomized 1:1 to auto-titrating CPAP or no treatment.
-   In-hospital PSG performed for OSA participants with acquisition of EEG, EOG, EMG, ECG, respiratory effort, airflow, and oximetry.
-   Questionnaires and clinical data collected at baseline: included ESS, Functional Outcomes of Sleep Questionnaire, SF-36 Health Survey, Zung Self-Rated Depression Scale, Zung Self-Rated Anxiety Scale), and medication history, anthropometrics, smoking status, and echocardiographic parameters.
-   Blood samples collected after overnight fast at baseline and follow-up visits
-   Echocardiographic assessment and maximal exercise testing performed at baseline, 3 months, and 1 year.

### HSAT Collection / Scoring

Initial screening with unattended home sleep apnea testing (HSAT) was done using the Embletta® digital system measuring nasal pressure, thoracoabdominal movements, pulse oximetry, and body position. Apnea was defined as ≥ 90% airflow cessation; hypopnea as ≥ 50% reduction in nasal pressure or thoracoabdominal movement for ≥ 10 seconds.

### Polysomnology (PSG) Collection

All OSA participants underwent in-hospital attended PSG using Embla A10. Physiological signals included cortical EEG, eye movement, chin muscle tone, ECG, thoracic and abdominal respiratory movements, nasal airflow and pressure, oxygen saturation. These data confirmed diagnosis and characterized sleep architecture, including total sleep time (TST) and REM sleep percent . Sleep stages and respiratory events scored according to established criteria.

### Polysomnology (PSG) Scoring

-   Sleep data centrally scored by blinded sleep technologists.
-   Sleep stages scored in 30-second epochs using standard rules.
-   Apneas defined as \>90% reduction in airflow for ≥10 seconds.
-   Hypopneas defined as ≥50% reduction in airflow or thoracoabdominal movement for ≥10 seconds, with associated desaturation or arousal.

### CPAP Usage Collection

-   CPAP usage data were collected longitudinally at scheduled visits (1, 3, 6, and 12 months, then annually up to 6 years) and downloaded from device memory for objective adherence monitoring.

## Data Overview

### Covariate/Phenotype Datasets (CSV)

The [covariate dataset files](:files_path:/datasets) contain 511 unique subjects with repeated measures across study visits.

-   The study includes clinical and demographic attributes, questionnaire data, laboratory measurements, and CPAP adherence metrics collected at baseline and follow-ups.
-   Unique subject identifiers link clinical and sleep data across visits.
-   Repeated measures allow for longitudinal assessment up to 3 years and 6 years for some outcomes.

The dataset columns are described in the accompanying data dictionary files. The **variables** data dictionary file includes folder names (id), labels (display names), descriptions, and other metadata. Categorical variables also include an associated “domain” (e.g., 1=male, 2=female), which are described in the **domains** data dictionary file.

The history of the covariate dataset and data dictionary files have been tracked on GitHub (<https://github.com/nsrr/riccadsa-data-dictionary>).

The CPAP dataset **riccadsa-cpap-dataset-0.1.0.csv** contains the CPAP usage data for up to 9 follow-up timepoints downloaded from the device memory .

The harmonized dataset **riccadsa-harmonized-dataset-0.1.0.csv** contains the most frequently used variables available in the RICCADSA dataset from the three main study visits. These variables were curated by the NSRR team to allow ready inter-operability with other NSRR datasets. Key harmonized variables include:

|  |  |
|-----------------------------------------------------|-------------------|
| **Variable** | **Label** |
| [nsrr_age](:variables_path:/nsrr_age) | Subject age |
| [nsrr_sex](:variables_path:/nsrr_sex) | Subject sex |
| [nsrr_bmi](:variables_path:/nsrr_bmi) | Body mass index (BMI) |
| [nsrr_current_smoker](:variables_path:/nsrr_current_smoker) | Currently smoking cigarettes |
| [nsrr_bp_diastolic](:variables_path:/nsrr_bp_diastolic) | Diastolic blood pressure |
| [nsrr_bp_systolic](:variables_path:/nsrr_bp_systolic) | Systolic blood pressure |
| [nsrr_odi_dsge4](:variables_path:/nsrr_odi_dsge4) | Oxygen Desaturation Index (4%) |
| [nsrr_phrnumar_f1](:variables_path:/nsrr_phrnumar_f1) | Arousal Index: Number of arousals per hour of sleep from polysomnography |
| [nsrr_pctdursp_s3](:variables_path:/nsrr_pctdursp_s3) | Percentage of total sleep duration (i.e., total sleep time, TST) in stage 3/4 from polysomnography |
| [nsrr_pctdursp_sr](:variables_path:/nsrr_pctdursp_sr) | Percentage of total sleep duration (i.e., total sleep time, TST) in REM from polysomnography |
| [nsrr_tst_f1](:variables_path:/nsrr_tst_f1) | Total Sleep Duration: the interval between sleep onset and sleep offset while the participant is asleep from polysomnography |

The [cpap dataset] \### PSG Signal and Annotation Files - Raw PSG data with EEG, EOG, EMG, ECG, respiratory channels, and oximetry for diagnosis and staging. - Event annotations (apneas, hypopneas, arousals) scored per standard criteria. - Data used to determine variables such as total sleep time, sleep stages, and apnea-hypopnea indices.

## Access and Usage Considerations

The RICCADSA dataset is only available for non-commercial use.

## Citation and Acknowledgement

When using this dataset, users must cite the following publication:

> [Zhang GQ, Cui L, Mueller R, Tao S, Kim M, Rueschman M, Mariani S, Mobley D, Redline S. The National Sleep Research Resource: towards a sleep data commons. J Am Med Inform Assoc. 2018 Oct 1;25(10):1351-1358. doi: 10.1093/jamia/ocy064. PMID: 29860441; PMCID: PMC6188513.](https://pubmed.ncbi.nlm.nih.gov/29860441/)

> [Peker Y, Glantz H, Eulenburg C, Wegscheider K, Herlitz J, Thunström E. Effect of positive airway pressure on cardiovascular outcomes in coronary artery disease patients with nonsleepy obstructive sleep apnea: the RICCADSA randomized controlled trial. Am J Respir Crit Care Med. 2016 Sep 1;194(5):613-20. doi: 10.1164/rccm.201601-0088OC. PMID:26914592.](https://pubmed.ncbi.nlm.nih.gov/26914592/)

Users must include the following text in any Acknowledgements section:

> Funding for the RICCADSA randomized control trial was provided by the Swedish Research Council, the Swedish Heart-Lung Foundation, the Agreement concerning research and education of doctors of Västra Götalandsregionen, Research Fund at Skaraborg Hospital, Skaraborg Research and Development Council, the Heart Foundation of Kärnsjukhuset, ResMed Foundation, and ResMed Ltd. ResMed Sweden supplied some sleep recording devices and technical support. None of the funders had direct influence on study design, data analysis, manuscript drafting, or publication decisions.

> The National Sleep Research Resource was supported by the U.S. National Institutes of Health, National Heart Lung and Blood Institute (R24 HL114473, 75N92019R002).

## References

-   The RICCADSA Trial is registered at ClinicalTrials.gov (NCT00519597): <https://clinicaltrials.gov/study/NCT00519597>
-   NSRR RICCADSA GitHub Documentation: <https://github.com/nsrr/riccadsa-documentation>
-   NSRR RICCADSA GitHub Data Dictionary: <https://github.com/nsrr/riccadsa-data-dictionary>
