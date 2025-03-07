---
title: Modeling of Serine Protease Substrate Catalysis In Synthetic Micelle Environment
image:
  path: /images/catalysis.jpeg
  thumbnail: /images/catalysis.jpeg
  width: 50%  # Reduce the display size to 50% of the container
  height: auto
  alt: "Organization Structure"
---
Mentors: Xueyu Song, Davit Potoyan

{% include toc %}

# Background

Catalysis inside micellar environments presents an intriguing mechanism for accelerating biochemical reactions. In this project, we aim to model the catalytic activity of serine proteases on small molecule substrates encapsulated in micelles synthetized in the lab of Prof. Yan Zhao at ISU. The goal is to develop a machine learning-based simulation framework that integrates enzyme structures, ligand docking, and substrate information to predict catalytic efficiency within micelles.

# Key Objectives

- Develop a computational workflow to model enzyme-substrate interactions inside micelles
- Train machine learning models, including graph neural networks (GNNs), on structural data of serine proteases and their substrates.
- Utilize SMILES-based representations and molecular docking to study binding affinity and reaction dynamics
- Simulate enzymatic catalysis within micellar environments to gain mechanistic insights.

# What You’ll Do

1. **Data Collection and Preprocessing** 
- Curate a dataset of serine protease structures from the Protein Data Bank (PDB).
- Collect substrate molecules and represent them using SMILES notation
- Perform molecular docking to identify binding poses within the enzyme’s active site.

2. **Machine Learning Model Development**
- Implement graph neural networks to learn substrate features and predict catalytic efficiency
- Train models using labeled data derived from experimental kinetics and computational simulations.
- Utilize transfer learning techniques on pre-trained molecular models for enhanced predictive accuracy.

3. **Computational Simulations**
-  Perform molecular dynamics (MD) simulations of enzyme-ligand interactions inside enzymes.
- Investigate how enzyme environment influences binding affinity and transition state stabilization by alchemically modifying interactions inside pocket.
- Compare computational predictions with available experimental data

# Expected Outcomes
 
- A trained machine learning model capable of predicting catalytic efficiency in micelles.
- A validated simulation framework combining ML predictions with MD simulations.
- Insights into the mechanistic aspects of micelle-mediated enzymatic catalysis.
