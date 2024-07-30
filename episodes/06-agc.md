---
title: "Analysis Grand Challenge"
teaching: 5
exercises: 0
---

:::::::::::::::::::::::::::::::::::::: questions 

- How do we perform a cross-section measurement with CMS Open Data?
- What are the challenges of processing large datasets in particle physics?
- How do we ensure reproducibility and scalability in analysis workflows?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Perform a cross-section measurement using CMS Open Data.
- Understand the challenges and methods for processing large particle physics datasets.
- Gain experience in creating reproducible and scalable analysis workflows.

::::::::::::::::::::::::::::::::::::::::::::::::

## Analysis Grand Challenge

This project is designed for more experienced programmers looking for a challenging activity using CMS Open Data.

### Overview

The [Analysis Grand Challenge](https://agc.readthedocs.io/en/latest/?badge=latest) (AGC) is aimed at participants who have a solid programming background and are eager to tackle complex problems. This challenge involves performing the final steps in an analysis pipeline at scale to test workflows envisioned for the High-Luminosity Large Hadron Collider (HL-LHC).

### Setup for Open Data workshop participants

You will need a slightly newer python container to install all the packages needed for this challenge

```
export workpath=$PWD
mkdir cms_open_data_AGC
chmod -R 777 cms_open_data_AGC
docker run -it --name my_agc -P -p 8888:8888 -v ${workpath}/cms_open_data_AGC:/code gitlab-registry.cern.ch/cms-cloud/python-vnc:python3.10.12
```

The AGC $t\bar{t}$ analysis repository contains a file of requirements. Download this file and install the requirements: 

```
## alternate to wget: git clone https://github.com/iris-hep/analysis-grand-challenge
code/$ wget https://raw.githubusercontent.com/iris-hep/analysis-grand-challenge/main/analyses/cms-open-data-ttbar/requirements.txt
code/$ pip install -r requirements.txt
``` 

### Analysis Pipeline

Participants will work on a cross-section measurement using 2015 CMS Open Data. This includes:

1. **Columnar Data Extraction**: Extracting data from large datasets in a columnar format.
2. **Data Processing**: Filtering events, constructing observables, and evaluating systematic uncertainties.
3. **Histogramming**: Summarizing the processed data into histograms.
4. **Statistical Model Construction**: Building statistical models based on the histograms.
5. **Statistical Inference**: Performing statistical analysis to infer the cross-section measurement.
6. **Visualization**: Creating relevant visualizations for each step of the analysis.

### Working with CMS Open Data

Using older CMS data presents unique challenges, such as analyzing data formats within the CMSSW software framework. Participants will learn strategies for overcoming these obstacles, ensuring their analyses are robust and accurate even when working with older CMS Open Data.

::::::::::::::::::::::::::::: callout
## Discussion forums

Make sure to join the [Mattermost channel](https://mattermost.web.cern.ch/cmsodws2024/channels/4-advanced-generative-challenge) for this activity to engage directly with the workshop instructors and fellow participants.

:::::::::::::::::::::::::::::

### Reproducibility and Scalability

An essential aspect of the AGC is ensuring that the analysis workflow is reproducible and can scale to the requirements of the HL-LHC. Participants will learn how to:

- Utilize tools and services for data access and event selection (e.g., Rucio, ServiceX).
- Implement histogramming and summary statistics using tools like Coffea and cabinetry.
- Construct and fit statistical models using software like Pyhf.
- Capture the entire analysis workflow for future reinterpretation using standards and services like [REANA](https://www.reana.io) and RECAST.

### Practical Application

In this project, participants will apply their knowledge to perform a cross-section measurement. This involves building and executing the analysis pipeline, rigorously validating the results, and ensuring the workflow is reproducible and scalable.

For more detailed information and guidelines, please refer to the [Analysis Grand Challenge Documentation](https://agc.readthedocs.io/en/latest/).

::::::::::::::::::::::::::::::::::::: keypoints 

- Cross-section measurement using CMS Open Data.
- Challenges and methods for processing large datasets.
- Creating reproducible and scalable analysis workflows.

::::::::::::::::::::::::::::::::::::::::::::::::
