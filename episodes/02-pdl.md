---
title: "Particle Discovery Lab"
teaching: 30
exercises: 60
---
:::::::::::::::::::::::::::::::::::::: questions

How can we identify different particles in collision data?
What are the characteristics of muons in the dataset?
How do we perform basic and advanced data analysis in particle physics?
::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

Reconstruct decays of an unknown particle X to 2 muons.
Use histograms to display the calculated mass of particle X.
Learn to fit and subtract background contributions from data.
Understand uncertainty propagation throughout the analysis.
Identify the discovered particle and compare its properties to known values.
::::::::::::::::::::::::::::::::::::::::::::::::

## Particle Discovery Lab

Participants will analyze real particle collision data from the CMS experiment. They will identify different particles, such as muons and electrons, by examining the data's characteristics. This exercise helps students understand how physicists discover and study fundamental particles.

## Overview
The Particle Discovery Lab is designed to introduce participants to the fascinating world of particle physics by working with actual data from the CMS experiment. This hands-on experience will provide valuable insights into the process of particle identification and the analysis techniques used by physicists.

### Identifying Particles
Participants will learn to identify different particles by analyzing their collision data. Key characteristics such as energy, momentum, and decay patterns will be examined to distinguish between various particles. The focus will be on identifying muons and electrons, which are fundamental components in many particle physics studies.

### Basic and Advanced Data Analysis
The lab will guide participants through both basic and advanced data analysis tasks. Initially, they will perform simple tasks such as plotting histograms and calculating basic statistics. As they progress, more advanced techniques will be introduced, including fitting data to theoretical models and performing complex statistical analyses.

## Instructions for the Exercise
To get started with the Particle Discovery Lab, follow these steps:

1. Set Up the Python Container: Ensure you are working within the provided Python container environment.
2. Clone the Repository: Open a terminal in the Python container and run the following command to clone the repository:
```bash
git clone -b instructors https://github.com/bethel-physics/ParticleDiscoveryLab.git
cd ParticleDiscoveryLab/PythonAnalysis
```
3. Run the Analysis: Navigate to the cloned repository directory and follow the instructions provided in either the Python script or the Jupyter notebook to complete the exercise.
- Script: Run the following command:
```bash
python MuonAnalysis_student.py
```
- Jupyter Notebook:

- Start Jupyter Lab:

```bash
jupyter lab
```
- Open MuonAnalysis_student.ipynb and follow the instructions.

## Visualize with CMS Spy WebGL
To enhance your understanding and visualization of the particle collision events, use the CMS Spy WebGL visualizer. This tool provides a 3D visualization of the CMS collision data, allowing you to better grasp the spatial distribution and interactions of particles.

::::::::::::::::::::::::::::: callout

You Have Choices!

While ROOT and C++ are essential for early-stage analysis of CMS Open Data in the AOD (Run 1) or MiniAOD (Run 2) formats, participants can use other tools and file formats for downstream analysis or for analyzing Run 2 NanoAOD files. Feel free to choose the tools that best suit your needs and preferences.

:::::::::::::::::::::::::::::

### Recommendations for Hackathon Activities

Participants in the hackathon can leverage their skills and the themes explored in the Particle Discovery Lab to tackle innovative challenges and projects. Here are some suggested activities:

- **Advanced Particle Identification Algorithms**: Develop and implement advanced algorithms for particle identification using collision data.
- **Enhanced Data Visualization Tools**: Create interactive tools for exploring and analyzing CMS collision data in real-time.
- **Integration of Machine Learning**: Apply machine learning techniques to automate data analysis and improve particle identification accuracy.
- **Collaborative Analysis Projects**: Form teams to tackle complex analysis challenges or develop new methodologies for studying particle interactions.
- **Educational Outreach and Visualization**: Design educational materials or demos that explain particle physics principles using CMS collision data.
- **Open Data Innovation**: Develop tools or platforms to enhance accessibility and usability of CMS Open Data for the scientific community.

These activities encourage innovation, collaboration, and exploration of particle physics concepts beyond the basic lab exercises.


::::::::::::::::::::::::::::::::::::: keypoints

Introduction to particle collision data.
Techniques for identifying particles such as muons and electrons.
Methods for performing both basic and advanced data analysis.
::::::::::::::::::::::::::::::::::::::::::::::::