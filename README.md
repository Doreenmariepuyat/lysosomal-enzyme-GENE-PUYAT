# PLA2G15 Lysosomal Enzyme Sequence Analysis

## Overview

This individual lab analyzes the human lysosomal enzyme encoded by **PLA2G15** using R and a protein sequence obtained from NCBI. The analysis calculates protein length and amino acid composition, identifies potential N-glycosylation motifs, and generates two figures.

- **Gene symbol:** PLA2G15
- **Protein:** Lysosomal phospholipase A and acyltransferase, isoform 1 precursor
- **Organism:** *Homo sapiens*
- **NCBI RefSeq protein accession:** [NP_036452.1](https://www.ncbi.nlm.nih.gov/protein/NP_036452.1)

## Enzyme Function

PLA2G15 encodes lysosomal phospholipase A and acyltransferase, also known as lysosomal phospholipase A2 (LPLA2). This enzyme helps break down certain phospholipids and related lipid molecules in lysosomes.

## Methods

The supplied R script (`lysosomal_enzyme_analysis.R`) downloaded the protein FASTA sequence from NCBI using the `rentrez` package. It calculated the protein length and amino acid composition, searched for potential N-glycosylation motifs, and generated figures using `ggplot2`.

A potential N-glycosylation motif follows the pattern **N-X-S/T**, where X is not proline. A detected motif is only a sequence-based prediction; it does not confirm glycosylation or the presence of a mannose-6-phosphate (M6P) tag.

## Results and Evidence

<img width="1366" height="725" alt="image" src="https://github.com/user-attachments/assets/b119fb5b-8e18-4375-ad28-d056b201f5ad" />

### Figure 1. RStudio project setup showing the selected lysosomal enzyme gene, PLA2G15, and its NCBI RefSeq protein accession.


<img width="1365" height="725" alt="image" src="https://github.com/user-attachments/assets/4dca1e28-3832-44ad-b278-63759d2fbc37" />

### Figure 2. Retrieval of the PLA2G15 protein sequence from NCBI using R and the rentrez package.


<img width="602" height="63" alt="image" src="https://github.com/user-attachments/assets/94dabe12-fe68-4bcc-b723-25e5d027ff18" />

### Figure 3. Calculation of PLA2G15 protein length and summary statistics using the downloaded sequence.


<img width="375" height="152" alt="image" src="https://github.com/user-attachments/assets/bcb43aa6-9d48-47bd-a8a6-1824c08adf7c" />

### Figure 4. Amino acid composition of the PLA2G15 protein sequence, showing the frequency of each standard amino acid.


<img width="505" height="232" alt="image" src="https://github.com/user-attachments/assets/f3d20fc0-09c3-4736-96f0-1f0b8fe49143" />

### Figure 5. RStudio project directory showing the R analysis script and the data, results, and figures folders created for the PLA2G15 lysosomal enzyme sequence analysis.


<img width="1366" height="715" alt="image" src="https://github.com/user-attachments/assets/bdf4f28f-d258-444e-80ee-199fb5af8012" />

### Figure 5. Amino acid composition of the PLA2G15 protein sequence. The bar graph shows the count of each amino acid in the 412-amino-acid protein. Leucine (L) was the most abundant amino acid, appearing 55 times, followed by glycine (G), with 34 occurrences.



<img width="1364" height="726" alt="image" src="https://github.com/user-attachments/assets/dc81949b-77cc-40c1-a72a-5abc2ba5e906" />

### Figure 6. Positions of potential N-glycosylation motifs in the PLA2G15 protein sequence. The graph shows the locations of four predicted N-X-S/T motifs along the 412-amino-acid protein sequence, with X representing any amino acid except proline.


## Answers to the Five Lab Questions

### 1. What does your enzyme normally break down inside lysosomes?

PLA2G15 encodes an enzyme involved in breaking down certain phospholipids and related lipid molecules in lysosomes.

### 2. What is the total length of your protein, and which amino acids are most common?

The analyzed protein was **412 amino acids** long. The five most common amino acids were leucine (L, 55; 13.35%), glycine (G, 34; 8.25%), proline (P, 31; 7.52%), valine (V, 31; 7.52%), and arginine (R, 23; 5.58%).

### 3. How many potential N-glycosylation motifs did you find? Where are they located?

The script detected **4 potential N-glycosylation motifs** matching the N-X-S/T pattern, where X is not proline. Their exact positions and motif sequences are recorded in `results/PLA2G15_motif_positions.csv`.

### 4. Why can glycosylation matter for lysosomal proteins? Does finding a motif prove the protein is glycosylated?

Glycosylation can help proteins fold correctly, remain stable, and move through the cell's sorting and transport systems. For many lysosomal enzymes, carbohydrate modifications are also important for delivery to lysosomes. However, finding an N-X-S/T sequence motif does **not** prove that a sugar is attached. This sequence analysis also does not determine whether the protein has a mannose-6-phosphate (M6P) tag.

### 5. What could happen in the cell if your enzyme did not work properly?

If PLA2G15 does not function properly, certain lipid molecules may not be broken down normally and could accumulate or be processed abnormally in cells. The exact consequences depend on the nature and severity of the enzyme defect. This sequence analysis does not measure enzyme activity or establish that a functional defect is present.

## References and Resources

- NCBI Protein: [PLA2G15, NP_036452.1](https://www.ncbi.nlm.nih.gov/protein/NP_036452.1)
- NCBI: [National Center for Biotechnology Information](https://www.ncbi.nlm.nih.gov/)
