---
title: Automating the Fragmentation of Proteins
image:
  path: /images/fragmenting_protein.png
  thumbnail: /images/fragmenting_protein.png
  width: 50%  # Reduce the display size to 50% of the container
  height: auto
  alt: "A group of scientists cut fragments up with scissors."
---
Mentors: Qi Li, Ryan Richard, Theresa Windus

{% include toc %}

# Background

In order to predict enzymatic reactions we must be able to compute the energy
of proteins, ligands, and their environment. Our preferred energy models are
computationally very expensive (requiring supercomputers for systems with a
100 atoms or more). To reduce the cost we can break the large calculation into
many smaller calculations. The larger calculation can then be approximated by
adding up the energies of the smaller calculations. In practice there are a
very large number of possible ways to break the large system up and 
unfortunately the accuracy of the approximation is very sensitive to how the
system is broken up. This project aims to develop an automated solution to
fragmenting proteins that minimizes the error in the approximation.

# Key Objectives

- Workflow for automating fragmentation of proteins.
- Compare and contrast different fragmentation schemes.
- Investigate the use of AI/ML to predict better fragments.

# What You’ll Do

1. **Develop Components for Automating Fragmentation** 
- Component for reading Protein Data Bank (PDB) files.
- Component for splitting PDB files by amino acids.
- Component for preparing an NWChem input file for a set of amino acids.

2. **Develop Infrastructure for Curating Training Data**
- Infrastructure for running NWChem input files.
- Infrastructure for parsing NWChem output files into curated data sets.
- Infrastructure for storing input, output, and curated data.

3. **Train AI/ML Models for Fragmentation**
- Pre-process data for running ProtBERT model.
- Fine-tune ProtBERT to predict if adjacent amino acids should be grouped or separated. 

# Expected Outcomes

- Reusable and sustainable software components for fragmenting proteins.
- An understanding of how fragmentation scheme affects time to solution and
  accuracy.
- Experience: developing software, running computational chemistry calculations,
  curating data, automating research, and contributing to better models of
  realistic protein systems.
