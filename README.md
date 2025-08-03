
# 🧬 PSSM Matrix Generator for Nucleotide Sequences

This repository contains a Python script for generating **Position-Specific Scoring Matrices (PSSMs)** from aligned nucleotide sequences in FASTA format. These matrices can be used as informative feature sets for various bioinformatics and machine learning applications.

---

## 📌 What is a PSSM?

A **Position-Specific Scoring Matrix (PSSM)** (also known as PWM or profile matrix) captures how often each nucleotide appears at every position in a set of aligned sequences. These matrices highlight conserved regions and help encode biological significance into numeric form — ideal for machine learning tasks.

---

## 🧪 What This Script Does

✔️ Reads an aligned FASTA file of nucleotide sequences  
✔️ Calculates frequency of A, C, G, T at each aligned position  
✔️ Applies **log-odds scoring** using uniform background probabilities  
✔️ Adds **pseudocounts** to handle zero frequencies  
✔️ Outputs the final PSSM as a pandas DataFrame (easy to save/export)

> ✅ Currently supports **nucleotide sequences**  
> 🔄 Coming soon: **PSSM for protein sequences**

---

## 📂 Files in This Repository

- `pssm_matrix.ipynb` — Jupyter Notebook with the full code, explanations, and test run  
- `README.md` — This file  
- *(Optional)* `example_alignment.fasta` — Example input file (you can add your own)

---

## ▶️ How to Use

1. Clone the repository:

```bash
git clone https://github.com/yourusername/pssm-matrix-generator.git
cd pssm-matrix-generator
```

2. Install the required libraries (if not already installed):

```bash
pip install biopython pandas numpy
```

3. Open the Jupyter notebook:

```bash
jupyter notebook pssm_matrix.ipynb
```

4. You also need to have **Clustal Omega** or **MUSCLE** installed for performing Multiple Sequence Alignment.

Install Clustal Omega (example for Ubuntu):

```bash
sudo apt install clustalo
```

---
5. Replace the example FASTA file with your aligned sequence file.

---

## 📊 Output

The final output is a **PSSM** represented as a matrix:
- Rows: Sequence positions
- Columns: Nucleotides
- Values: Log-odds scores

## 📈 Applications

This script is useful for:
- DNA motif discovery
- Promoter region analysis
- Preparing ML-ready features for classification tasks
- Genomics research involving conserved sequence patterns

---

## 💡 Coming Next

- Support for **protein sequence PSSMs**
- CLI version of the script
- Export to CSV or NumPy array for direct ML integration

---

## 📬 Contact

Feel free to open issues or reach out via [LinkedIn](https://www.linkedin.com/) if you have questions or ideas to improve the script!

## 🧬 Author

**Shrushti Salunke**  
Working in consumer genomics with a passion for bioinformatics and biological data modeling.
>>>>>>> 789e009 (Add PSSM README.md file)
