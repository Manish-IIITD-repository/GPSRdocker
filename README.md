# GPSRdocker: A Docker-based Resource for Genomics, Proteomics and Systems Biology

Welcome to the official documentation for **GPSRdocker**, a comprehensive, lightweight, and isolated platform designed to provide a wide range of computational tools for bioinformatics researchers. This resource integrates over **65 standalone software packages** predominantly developed by Dr. Gajendra P.S.Raghava's group over the last two decades.

**Official Website:** [https://webs.iiitd.edu.in/gpsrdocker/](https://webs.iiitd.edu.in/gpsrdocker/)  
**Docker Hub:** `raghavagps/gpsrdocker`

---

## Citation

Agrawal P, Kumar R, Usmani SS, Dhall A, Patiyal S, Sharma N, et al. (2019).  
**GPSRdocker: A Docker-based Resource for Genomics, Proteomics and Systems biology.** *bioRxiv* 827766.  
[https://doi.org/10.1101/827766](https://doi.org/10.1101/827766)

zenodo:-(https://doi.org/10.5281/zenodo.20066828)

---

## About the Platform

GPSRdocker addresses the challenges of traditional web-based services, such as internet speed limitations, computing power restrictions, and data security concerns.By utilizing **Docker containerization**, it provides a portable environment that ensures hardware/software compatibility and eliminates complex installation dependencies.

The container is categorized into three main components:
1.  **General Scripts**: Small Perl and Python programs for generating features like protein composition.
2.  **Supporting Software**: Integrated packages for data processing and model development, including PSI-BLAST, CD-HIT, WEKA, and $SVM^{light}$.
3.  **Standalone Prediction Packages**: Core software for predicting functions or classes of biomolecules across six major categories.

---

## Key Categories and Standalone Tools



[Image of protein structure prediction types]


### 1. Protein Structure Prediction
Tools to predict alpha/beta/gamma turns, transmembrane regions, and surface accessibility.
* **ALPHApred**: Predicts alpha-turns using neural networks.
* **SARpred**: Predicts real-value solvent accessibility.
* **TBBpred**: Predicts transmembrane beta-barrel regions.

### 2. Functional Annotation of Proteins
Methods for predicting subcellular localization and protein binding properties.
* **ALGpred**: Predicts allergenic proteins and maps IgE epitopes.
* **ESLpred2**: Advanced subcellular localization for eukaryotic proteins.
* **RNApred**: Predicts RNA-binding proteins.

### 3. Vaccinomics
Tools for immunogenomics and epitope-based vaccine design.
* **abcpred**: Mapping B-cell epitopes using neural networks.
* **ProPred / ProPred1**: Predicts MHC Class-II and Class-I binding sites.
* **vaxinpad**: Designing peptide-based vaccine adjuvants.

### 4. Genomics
Biomarker identification and genome annotation.
* **cancercsp**: Gene expression-based biomarkers for renal cancer.
* **desirm**: Designing highly efficient siRNAs.

### 5. BioDrugs
In silico screening for bioactive drugs and therapeutic peptides.
* **AntiCP**: Prediction and design of anticancer peptides.
* **ToxinPred**: Predicting and designing toxic/non-toxic peptides.
* **AntiTbPred**: Predicting peptides with bactericidal activity against *Mycobacterium*.

### 6. Interactome
Study of molecular interactions among proteins and small molecules.
* **ATPint / GTPbinder**: Identification of ATP and GTP binding sites.
* **GlycoEP / GlycoPP**: Prediction of glycosylation sites in eukaryotes and prokaryotes.

---

## Implementation & Usage

GPSRdocker provides a flexible platform that can run on any operating system or be ported to the cloud.

### Basic Commands:
1.  **Pull the Image**:  
    `docker pull raghavagps/gpsrdocker`
2.  **Run the Container**:  
    `docker run -i -t raghavagps/gpsrdocker`
3.  **Install Software Packages**:  
    Inside the image, run: `/gpsr/gpsr_install.pl`

---

## Key Advantages
* **Data Security**: Standalone operation allows researchers to keep confidential data local.
* **High Throughput**: Capable of processing large datasets that typically exceed webserver limits.
* **No Internet Required**: Once the image is pulled, all tools function offline.

---

## Contact & Support

**Prof. Gajendra P.S. [cite_start]Raghava** Head, Department of Computational Biology  
Indraprastha Institute of Information Technology (IIIT-Delhi), India.  
**Email**: raghava@iiitd.ac.in 

---

## License

This resource is available free for academic use under the **aCC-BY 4.0 International license**.
