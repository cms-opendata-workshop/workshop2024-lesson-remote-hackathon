---
title: "Particle Discovery Lab"
teaching: 30
exercises: 60
---
:::::::::::::::::::::::::::::::::::::: questions

- How can we identify different particles in collision data?
- What are the characteristics of muons in the dataset?
- How do we perform basic and advanced data analysis in particle physics?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Reconstruct decays of an unknown particle X to 2 muons.
- Use histograms to display the calculated mass of particle X.
- Learn to fit and subtract background contributions from data.
- Understand uncertainty propagation throughout the analysis.
- Identify the discovered particle and compare its properties to known values.

::::::::::::::::::::::::::::::::::::::::::::::::


## Particle Discovery Lab

The goal of the [Particle Discovery Lab](https://github.com/bethel-physics/ParticleDiscoveryLab), is to reconstruct decays of an unknown particle X (initial state) to 2 muons (final state). Participants will display histograms for the calculated mass of particle X and learn about fitting and subtracting background distributions from data.

Uncertainty propagation concepts are included at each step of the analysis. After isolating the signal distribution, participants will determine which particle they have discovered and compare its properties (mass and width) to known values.

### Get Ready

1. **Prepare Your Environment**:
   - Ensure that the `my_python` container is ready. Refer to the pre-exercise instructions for Docker setup and container creation.
   
2. **Set Up and Launch Jupyter Lab**:
   - Execute the following commands in your terminal:

     ```sh
     docker start -i my_python
     mkdir Particle_Discovery_Lab
     cd Particle_Discovery_Lab
     git clone https://github.com/DanielaMerizalde/CMS-Workshop.git
     cd ..
     jupyter-lab --ip=0.0.0.0 --no-browser
     ```

   - After running the last command, open the provided link in your browser to access Jupyter Lab.

3. **Verify Files**:
   - Ensure that the following files are present in the `Particle_Discovery_Lab` directory after cloning the repository:
     - `pollsf.py`
     - `Particle_Discovery_Lab.ipynb`
     - `DoubleMuParked_100K.pkl`

### Instructions for the Exercise

1. **Launch Jupyter Lab**:
   - In Jupyter Lab, navigate to `Particle_Discovery_Lab.ipynb` from the file menu and open it.

2. **Complete the Notebook**:
   - Follow the instructions in the notebook to complete the analysis interactively. You will perform tasks such as plotting histograms, fitting data, and analyzing uncertainties.


::::::::::::::::::::::::::::: callout
## Visualize with CMS Spy WebGL

To enhance your understanding and visualization of the particle collision events, use the CMS Spy WebGL visualizer. This tool provides a 3D visualization of the CMS collision data, allowing you to better grasp the spatial distribution and interactions of particles.

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

- Introduction to particle collision data.
- Techniques for identifying particles such as muons and electrons.
- Methods for performing both basic and advanced data analysis.

::::::::::::::::::::::::::::::::::::::::::::::::