# GlycoPP: Web Server for Prediction of Prokaryotic Glycosites

Welcome to the official repository and documentation overview for **GlycoPP**, an open-access platform designed for the accurate prediction of N- and O-linked glycosites in prokaryotic protein sequences. Developed to address the unique structural and sequence contexts of Archaea and Bacteria, GlycoPP provides a specialized tool for identifying these critical post-translational modifications (PTMs).

**Web Server:** [http://webs.iiitd.edu.in/raghava/glycopp/](http://webs.iiitd.edu.in/raghava/glycopp/)

---

## Citation

Chauhan JS, Bhat AH, Raghava GPS, Rao A (2012). 
**GlycoPP: A Webserver for Prediction of N- and O-Glycosites in Prokaryotic Protein Sequences.** 
*PLoS ONE* 7(7): e40155. 
[https://doi.org/10.1371/journal.pone.0040155](https://doi.org/10.1371/journal.pone.0040155)

Zenodo:-(https://doi.org/10.5281/zenodo.20063897)

---

## About the Platform

GlycoPP is the first web server specifically trained on prokaryotic glycoproteins, recognizing that eukaryotic prediction tools often fail when applied to bacterial and archaeal sequences[cite: 3]. The platform utilizes Support Vector Machine (SVM) algorithms to distinguish between glycosylated and non-glycosylated residues based on extensive experimental data.

The platform supports:
*   **N-linked Glycosylation**: Glycan attachment to the amide group of Asparagine (Asn).
*   **O-linked Glycosylation**: Glycan attachment to the hydroxyl group of Serine (Ser), Threonine (Thr), or Tyrosine (Tyr.

---

## Key Features

### Predictive Modeling
*   **Machine Learning**: Built using SVMlight with various kernels, optimized to handle the specific sequence motifs of prokaryotes.
*   **Feature Diversity**: Incorporates Binary Profiles (BPP), Composition Profiles (CPP), and Position-Specific Scoring Matrices (PSSM/PPP).
*   **Accuracy**: Achieved an accuracy of **82.71%** (MCC 0.65) for N-glycosites and **73.71%** (MCC 0.48) for O-glycosites.

### Structural & Hybrid Models
*   **Post-Translational Insight**: Since prokaryotic glycosylation often occurs on folded proteins, models include predicted secondary structure and surface accessibility.
*   **Surface Accessibility**: GlycoPP uses ASA (Accessible Surface Area) values to improve prediction, as glycosites are predominantly found on flexible, exposed loops.

### Data Resources
*   **Extensive Training Set**: Derived from 59 experimentally characterized glycoproteins, including 107 N-linked and 116 O-linked glycosites.
*   **Wide Domain Coverage**: Includes data from phyla such as *Proteobacteria*, *Crenarchaeota*, *Firmicutes*, and *Bacteroidetes*.

---

## Overview of Model Development

GlycoPP models were validated using 5-fold cross-validation and tested against an independent dataset of 28 prokaryotic glycoproteins to ensure reliability across different phyla.

| Feature Model | N-linked Accuracy | O-linked Accuracy |
| :--- | :--- | :--- |
| **BPP (Binary Profile)** | 79.91% | 66.81%|
| **PPP (PSSM Profile)** | 73.11% | 73.28% |
| **Hybrid (BPP + ASA)** | **82.71%**| 69.40% |
| **Hybrid (PPP + SS + ASA)** | 73.83%| **73.71%**|

---

## Applications

*   **Pathogen Research**: Understanding host-pathogen interactions mediated by bacterial glycoproteins.
*   **Vaccine Development**: Identifying immunogenic glycoproteins in pathogens like *Campylobacter jejuni* or *Mycobacterium tuberculosis*.
*   **Evolutionary Biology**: Gaining insights into the acceptor specificities of prokaryotic glycosyltransferases.

---

## Contact & Authors

**Prof. G.P.S. Raghava**  
raghava@iiitd.ac.in  
Bioinformatics Centre, Indraprastha Institute of Information Technology (IIIT-Delhi), India.

---

## License

This platform and its associated research are distributed under the **Creative Commons Attribution License**, allowing for unrestricted use and distribution with proper credit to the original authors.
