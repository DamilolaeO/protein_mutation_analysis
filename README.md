# Impact of Amino Acid Mutations on Protein Structure and Function

## Overview
 This project analyses the structural and functional impact of individual amino acid substitutions in proteins by integrating two datasets: **SIFT**, which predicts functional effects, and **FoldX**, which estimates structural destabilisation. The results are visualised and used to identify key amino acids that have a major impact, contributing to a better understanding of protein biology.
 
---


## Objective
To assess how single amino acid substitutions affect protein function and structure by:
- Merging predictions from SIFT and FoldX based on unique protein–mutation pairs;
- Identifying mutations that are simultaneously **deleterious** to structure and function;
- Investigating which amino acids are most frequently involved in such damaging mutations;
- Visualising the frequency and impact of these mutations across the proteome.

---

## Key Questions Addressed
- Which mutations impact both protein function (SIFT < 0.05) and structure (FoldX > 2)?
- Which amino acid substitutions occur most frequently among deleterious mutations?
- What trends emerge in amino acids with >100 damaging mutations?
- What might the structural and functional properties of these amino acids suggest?

---

## Tools Used
- **Language**: Python (Google Colab)
- **Libraries**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `collections`
- **Data Format**: TSV

---

## Key Findings
- Successfully created a unique mutation identifier (`specific_Protein_aa`) and merged the two datasets.
- Filtered for mutations with a **SIFT score < 0.05** and **FoldX score > 2**, identifying those that impact both structure and function.
- Glycine and Leucine were among the amino acids most frequently affected.
- Amino acids with more than 100 occurrences tend to be small and flexible (e.g., Glycine) or highly reactive (e.g., Cysteine). These properties make them prone to mutations that significantly alter protein structure and function.

---

## Visuals Included
- **Bar Plot**: Frequency of amino acids involved in high-impact mutations
- **Pie Chart**: Proportional representation of mutation frequency

---

## Business Impact
Provides valuable insights for predicting genetic mutations that affect protein function. The findings can help guide research into **genetic diseases**, **mutation prediction**, and **precision medicine**. 

---

## Files in this Repository
- `protein_mutation_analysis.ipynb` – Colab notebook with full code and analysis
- `sift_functional_mutation_scores.tsv` – Functional prediction dataset
- `foldx_structural_mutation_scores.tsv` – Structural impact dataset
- `README.md` – Project documentation

---

## Acknowledgements
This project was developed as part of the **HackBio** bioinformatics internship, under the Biochemistry & Oncology module. 
Dataset obtained from Galardini et al. (2019). *The impact of genetic variation on protein structure and function*. [https://doi.org/10.15252/msb.20198831](https://doi.org/10.15252/msb.20198831)


---

## Author
**Damilola Ogungbemi**  
MSc Biotechnology | Aspiring Data Scientist
