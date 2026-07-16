## About

The Randomized Intervention with CPAP in Coronary Artery Disease and Obstructive Sleep Apnea (RICCADSA) trial is a prospective, single-center randomized controlled trial conducted between 2005 and 2013. It enrolled 511 adult patients from two hospitals in Skaraborg County, Sweden with angiography-verified coronary artery disease (CAD) who underwent percutaneous coronary intervention (PCI) or coronary artery bypass grafting (CABG) within 6 months prior to study start.

The study incorporated home sleep apnea testing to screen all participants for OSA, followed by comprehensive baseline cardiovascular and sleep assessments. Patients with moderate-to-severe OSA were classified according to daytime sleepiness using the Epworth Sleepiness Scale (ESS). Non-sleepy participants with OSA (ESS \<10) were randomized to CPAP treatment or no CPAP, while sleepy participants with OSA (ESS ≥10) were offered CPAP without randomization. Participants without OSA served as an observational control group.

Primary clinic assessments were performed at baseline, 3 months, and 1 year. Additional longitudinal follow-up included CPAP adherence data collected from device downloads and long-term surveillance for cardiovascular events, including myocardial infarction, stroke, repeat coronary revascularization, hospitalization, cardiovascular mortality, and all-cause mortality.

## Methods

### Recruitment and eligibility 

Participants were Swedish adults with angiography-confirmed coronary artery disease who had undergone coronary revascularization by PCI or CABG within the previous six months. Eligible participants were recruited after their cardiovascular condition had stabilized following revascularization. Participants with predominantly central sleep apnea/Cheyne-Stokes respiration or borderline OSA were not enrolled in the trial.

### Clinical visits
#### Screening visit (Visit 0)

All eligible participants underwent unattended home sleep apnea testing (HSAT) using the Embletta® portable monitoring system. The screening study recorded nasal airflow, thoracoabdominal respiratory effort, pulse oximetry, body position, and heart rate to estimate the apnea-hypopnea index (AHI).

Participants were classified into one of three groups based on the HSAT results:

- **AHI \<5 events/hour:** Non-OSA control group

- **5 ≤ AHI \< 15 events/hour:** Borderline OSA (excluded from enrollment in the trial)

- **AHI ≥ 15 events/hour:** OSA group, eligible for further baseline sleep evaluation

#### Baseline visit (Visit 1)

Participants enrolled in the study subsequently attended the baseline clinic visit that included the following evaluations:

- demographic information, medical history, and anthropometric measurements

- coronary angiography and revascularization information

- fasting blood tests for clinical biomarkers

- transthoracic echocardiography

- questionnaires assessing daytime sleepiness (ESS), functional outcomes of sleep (FOSQ), quality of life (SF-36), anxiety, and depression

**Polysomnology (PSG)**

Participants in the OSA group (HSAT AHI ≥ 5) also underwent a subsequent unattended overnight polysomnography (PSG) using Embla A10\^© system for detailed characterization of sleep architecture and respiratory events. Physiological signals included cortical EEG, eye movement, chin muscle tone, ECG, thoracic and abdominal respiratory movements, nasal airflow and pressure, oxygen saturation.

**Randomization and treatment allocation**

Treatment allocation was determined after completion of baseline sleep evaluation using OSA status from HSAT screening and sleepiness symptoms, classified by Epworth Sleepiness Scale (ESS) score:

- **ESS \<10 (non-sleepy OSA):** Randomized in a 1:1 ratio to CPAP treatment or no CPAP using block randomization stratified by sex and type of coronary revascularization (n = 200).

- **ESS ≥ 10 (sleepy OSA):** Offered CPAP treatment without randomization for ethical reasons (n=155).

- **AHI \<5 events/hour:** Included as a non-OSA observational control group.

#### Follow-up visits (Visits 2&3)

Approximately three months after baseline, participants underwent a follow-up visit that repeated the major clinical assessments performed at baseline, including anthropometric measurements, blood pressure, laboratory testing, echocardiography, questionnaires, and maximal exercise testing.

One year after baseline, participants underwent another comprehensive follow-up visit that repeated assessments obtained at baseline and visit 2.

#### Long-term follow-up

Following completion of the primary clinic visits, participants were followed longitudinally for major adverse cardiovascular events or mortality, including:

- myocardial infarction

- stroke

- repeat coronary revascularization

- hospitalization for atrial fibrillation or heart failure

- cardiovascular mortality

- all-cause mortality

### CPAP usage collection

CPAP usage data were obtained from device memory at nine usage timepoints (1 month since start, 3 months, 6 months, and then annually 1 through 6 years) for objective adherence monitoring, as well as information on mask type, humidifier use, and treatment parameters.

### Manual scoring

Home sleep apnea testing (HSAT) data were scored using study-specific criteria. Apnea was defined as ≥90% reduction in airflow for at least 10 seconds, and hypopnea as ≥50% reduction in nasal pressure or thoracoabdominal movement for at least 10 seconds.

Polysomnography data were centrally scored by blinded sleep technologists. Sleep stages scored in 30-second epochs using standard rules. Apneas were defined as \>90% reduction in airflow for ≥10 seconds. Hypopneas were defined as ≥50% reduction in airflow or thoracoabdominal movement for ≥10 seconds, with associated desaturation or arousal.

## Data overview

### Covariate/phenotype datasets (CSV)

The [covariate dataset files](:files_path:/datasets) contain 511 unique subjects with repeated measures across primary study visits.

The dataset columns are described in the accompanying data dictionary files. The **variables** data dictionary file includes folder names (id), labels (display names), descriptions, and other metadata. Categorical variables also include an associated “domain” (e.g., 1=male, 2=female), which are described in the **domains** data dictionary file.

The history of the covariate datasets and data dictionary files have been tracked on GitHub (<https://github.com/nsrr/riccadsa-data-dictionary>).

The main covariate dataset **riccadsa-dataset-0.1.0.csv** includes study data from screening, three main clinic visits, as well as outcome/event records.

The CPAP dataset **riccadsa-cpap-dataset-0.1.0.csv** contains the CPAP usage data for up to 9 follow up timepoints.

The harmonized dataset **riccadsa-harmonized-dataset-0.1.0.csv** contains the most frequently used variables available in the RICCADSA dataset from the three main study visits. These variables were curated by the NSRR team to allow ready inter-operability with other NSRR datasets. Key harmonized variables include:

|  |  |
|------------------------------------|------------------------------------|
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

### PSG signal and annotation files

- Raw PSG data with EEG, EOG, EMG, ECG, respiratory channels, and oximetry for diagnosis and staging.
- Event annotations (apneas, hypopneas, arousals) scored per standard criteria.
- Data used to determine variables such as total sleep time, sleep stages, and apnea-hypopnea indices.

## Access and usage restrictions
The RICCADSA dataset is only available for non-commercial use.

## Citation and acknowledgements

When using this dataset, users must cite the following publication:

> [Zhang GQ, Cui L, Mueller R, Tao S, Kim M, Rueschman M, Mariani S, Mobley D, Redline S. The National Sleep Research Resource: towards a sleep data commons. J Am Med Inform Assoc. 2018 Oct 1;25(10):1351-1358. doi: 10.1093/jamia/ocy064. PMID: 29860441; PMCID: PMC6188513.](https://pubmed.ncbi.nlm.nih.gov/29860441/)

> [Peker Y, Glantz H, Eulenburg C, Wegscheider K, Herlitz J, Thunström E. Effect of positive airway pressure on cardiovascular outcomes in coronary artery disease patients with nonsleepy obstructive sleep apnea: the RICCADSA randomized controlled trial. Am J Respir Crit Care Med. 2016 Sep 1;194(5):613-20. doi: 10.1164/rccm.201601-0088OC. PMID:26914592.](https://pubmed.ncbi.nlm.nih.gov/26914592/)

Users must include the following text in any Acknowledgements section:

> Funding for the RICCADSA randomized control trial was provided by the Swedish Research Council, the Swedish Heart-Lung Foundation, the Agreement concerning research and education of doctors of Västra Götalandsregionen, Research Fund at Skaraborg Hospital, Skaraborg Research and Development Council, the Heart Foundation of Kärnsjukhuset, ResMed Foundation, and ResMed Ltd. ResMed Sweden supplied some sleep recording devices and technical support. None of the funders had direct influence on study design, data analysis, manuscript drafting, or publication decisions.

> The National Sleep Research Resource was supported by the U.S. National Institutes of Health, National Heart Lung and Blood Institute (R24 HL114473, 75N92019R002).

## Changelog

### July 2026
- Make RICCADSA dataset version 0.1.0 public and available for data request

## References

- The RICCADSA Trial is registered at ClinicalTrials.gov (NCT00519597): <https://clinicaltrials.gov/study/NCT00519597>
- NSRR RICCADSA GitHub Documentation: <https://github.com/nsrr/riccadsa-documentation>
- NSRR RICCADSA GitHub Data Dictionary: <https://github.com/nsrr/riccadsa-data-dictionary>
