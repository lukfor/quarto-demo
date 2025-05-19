
# quarto-demo — Data Cleaning Pipeline with Report

This is a minimal, transparent example designed to help you build your own data cleaning pipelines with automated reporting. Ideal for research, reproducibility, and collaboration.

## 📂 Project Structure

```

quarto-demo/
├── data/
│   └── genotypes.vcf.gz # Input VCF and related genotype data
├── environment.yaml             # Conda environment definition
├── report.qmd           # Quarto report source
├── output/              # Directory for cleaned outputs and figures
└── README.md            # This file

````

## 🚀 How to Use

Follow these steps to set up the environment and generate the report.

### 1. Create Environment Using Micromamba

Make sure you have [Micromamba](https://mamba.readthedocs.io/en/latest/micromamba.html) installed.

```bash
micromamba create -f environment.yaml
````

### 2. Activate Environment

```bash
micromamba activate quarto-demo
````

### 3. Render the Report

After activating the environment:

```bash
quarto render report.qmd
```

This will produce a file named `report.html` in the same directory.

You can open the report in any modern web browser.


### 3. Render the Report with parameters

After activating the environment:

```bash
quarto render report-with-params.qmd -P input=myfile.vcf.gz
```

This will produce a file named `report-with-params.html` in the same directory.

You can open the report in any modern web browser.

## 📦 Requirements

All required packages are listed in `environment.yaml`. Key tools include:

* `quarto`
* `r-base` and required R packages
* Tools for handling VCF files


This is a minimal, transparent example designed to help you build your own data cleaning pipelines with automated reporting. Ideal for research, reproducibility, and collaboration.
