# Miniproject 2 
After reading the information for each project, choose your preferred one here : 
https://docs.google.com/forms/d/e/1FAIpQLSd8O3dEJ7xSUpw1TkIZx80o4LlnB2x0X-Goy-jnNHnm4lTI4w/viewform?usp=sf_link.

### GP spiking data 
_Arthur Leblois_

<details>

<summary> Project information </summary>
Parkinsonian patients and animal models are known to display abnormal oscillations in the beta range (12-30 Hz) in the basal ganglia-thalamo-cortical network. In particular, neural activity in the basal ganglia, including the Globus pallidus, show abnormally strong synchrony with cortical EEG in the beta range. Recently, Mallet et al (Mallet et al., 2012, attached) described two neural populations in the Globus pallidus (GP) based on the axonal projections and synchrony of their activity to cortical EEG during slow wave activity in anaesthetized rats. In this project, you will analyse four data sets concisting in extracellular activity of single GP neurons simulatneously recorded (10-15 neurons per recording) in anaesthetized rats in four    conditions: normal animals in 'slow wave state' and 'activated state',and parkinsonian rats in 'slow wave state' and 'activated state'. The slow wave and activated states are 2 different states displayed by rats during anaesthesia which displkay different patterns of EEG activity. 

The goal of the project is to quantify the oscillatory synchrony between GP neurons and the cortical EEG in the parkinsonian rats in both states. The two distinct neuronal populations of the GPe display different patterns of low frequency (1Hz) synchrony with cortical EEG in the slow wave state. Synchrony between GP neurons and EEG at beta frequency (12-30 Hz) during the activated state will be caracterized, and the correlation between GP neurons will be used to show the difference in their firing pattern during beta oscillations. Altogether, the results of Figure 1 of the paper can be reproduced on this sample data set. [https://doi.org/10.1016/j.neuron.2012.04.027](https://doi.org/10.1016/j.neuron.2012.04.027)

</details>

### Amsterdam Open MRI Collection (AOMIC) 
_Slim Karkar_
<details>

<summary>Project information</summary>
In this project, we will work on fMRI data from the  Amsterdam Open MRI Collection (AOMIC).

The AOMIC dataset gathers MRI data from more than a thousand individuals obtained on a 3 Tesla imager. For each subject we can access the T1-weighted images ( anatomical image), the diffusion-weighted images ( white-matter tracts)  and fMRI sequences (task-based and resting states). The dataset gives access to both raw and preprocessed (derivative) data. The description of the data acquisition and processing is available here : 

Snoek, L., van der Miesen, M. M., Beemsterboer, T., Van Der Leij, A., Eigenhuis, A., & Scholte, H. S. (2021). The Amsterdam Open MRI Collection, a set of multimodal MRI datasets for individual difference analyses. Scientific data, 8(1), 1-23.

All data are publicly available for downloads using AWS s3 buckets s3://openneuro.org/.
The projects will use Jupyter Notebook with the following library : numpy, scipy,  scikit-learn; nilearn.

aim (i):  we will study HRF variation for various task and use convolution tools to fine tune HRF models in different activation task using following model : https://github.com/andrewjahn/AndysBrainBook/blob/master/docs/SPM/SPM_Short_Course/SPM_Statistics/SPM_03_Stats_HRF_Overview.rst

aim (ii): we will use time-frequency analysis to propose connectivity map in resting-state and compared with the RSN proposed in the paper :  
Smith, SM, Fox, PT, Miller, KL, Glahn, DC, Fox, PM, Mackay, CE, Filippini, N, Watkins, KE, Toro, R, Laird, AR, Beckmann, CF (2009). Correspondence of the brain's functional architecture during activation and rest. Proc Natl Acad Sci U S A, 106, 31:13040-5.**


  
</details>

### EEG: Analyzing signals from the brain! 
_Nikolaos Vardalakis_
<details>

<summary>Project information</summary>
The goal of this project is to learn how to manipulate EEG data. In EEG research, recorded raw data that are used in analyses require preparation, also called preprocessing, a process that involves a number of manipulations. We will use a live dataset recorded from a single participant and we will take a closer look on the data collected during the equipment calibration step, assessing the baseline brain activity of the participant with their eyes open and their eyes closed. Can we identify the subtle differences on the EEG traces and the underlying rhythms?

To start preparing for the project, you can get familiar with the resources below. This pipeline is a useful guide when it comes to the steps required to preprocess (clean) EEG data: https://sccn.ucsd.edu/wiki/Makoto%27s_preprocessing_pipeline.
</details>

### Modeling: Propagation of activity patterns in a network of locally interconnected populations of neurons.
_Fjola Hyseni_
<details>

<summary>Project information</summary>
  
Aim: The aim of the project is to implement and investigate a simplified model of HVC.

Background: Experimental evidence shows that in several sensory and motor related parts of the brain, neurons present an activity that depends on particular features of the sensory stimuli or of the motor output.  For example, specific neurons in the cat visual cortex modulate their firing rate depending on the orientation of the visual stimulus and neurons in the premotor song control nucleus HVC of singing birds fire preferentially at specific times during the song production. For the project, we focus mainly on the function of the nucleus HVC.

Implementation: The model consists of a network of interconnected neurons or populations of neurons. The neurons are modelled as integrate and fire neurons. Each neuron in the network fires at different time instants during song production. We aim to build step by step a chain of populations of neurons featuring a propagating neuronal activity. At each step we will discuss the limits of the achieved network model and try to overcome these limits. 
  
https://doi.org/10.1038/s41467-018-03261-5
</details>

--- 
## What needs to be done for mini-project 2

## Report and notebooks are due (by mail) on Monday 21 November, 8am.

--- 
### Notebook

The notebook will be mostly used to prepare your figures for the report (see below). Make sure to make it easy to generate figures. Ideally, the last few cells of your notebook should produce directly the figures that are included in the report. You can also produces supplementary figures that won't be included in the report but could be used for presentation.

--- 
### Report

A short report (2 pages (or more if necessary)) with the structures described below. No need to have extensive description of the context, you can make the report very short and writing quality is not a criteriokn as long as we can understand what you write.

#### Title + authors

#### Abstract

#### Introduction
- What is the domain and what kind of data or model
- What are the questions you're trying to answer
- What are your starting hypothesis

#### Methods & materials
- Describe briefly the nature of your data (if any)
- Describe the method you'll be using to analyse
  or describe the model you're using with proper reference
- Explain how to check if your analysis is correct

#### Results
- Introduce your results with some text and figure.
  (Make sure to caption your figure to explain what is to be seen)

#### Conclusion/Discussion
- What are the limits of your analysis (if any)
- How hard would it be to use other data or model with your code?

#### References


--- 
### Presentation

The goal of the presentation is to introduce your data analysis or modelling following more or less your report structure. 10 minutes is very short such that you might need to focus on a specific part of your analysis pipeline.

10 minutes presentation (~ 10 slides)
15 minutes question (with possibly live demo of your notebook)

--- 
### Evaluation criterions

#### Notebook
- Can we download your notebook according to the description in your report
- Is your notebook well organized (e.g. comments, explanations with markdown, name of variables, not too big cells, etc)
- Do we get the same figure as the ones in your report when xe run your notebook

#### Report

- If we were to redo you analysis/model from the report, do we have enough information (data and code access for example)
- Did you caption every figures ?
- Do you have links to code and data (or explanation how to get them)

#### Defense

- No requirements for each member of the group to talk, you can choose to have only one speaker.
- We might ask you to re-run a part of your notebook, modifying this or that parameters. 

