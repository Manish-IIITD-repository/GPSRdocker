# GPSRdocker: A Docker-based Resource for Genomics, Proteomics and Systems Biology

[cite_start]Welcome to the official documentation for **GPSRdocker**, a comprehensive, lightweight, and isolated platform designed to provide a wide range of computational tools for bioinformatics researchers[cite: 1142, 1253]. This resource integrates over **65 standalone software packages** predominantly developed by Dr. Gajendra P.S. [cite_start]Raghava's group over the last two decades[cite: 1144, 1648].

**Official Website:** [https://webs.iiitd.edu.in/gpsrdocker/](https://webs.iiitd.edu.in/gpsrdocker/)  
[cite_start]**Docker Hub:** `raghavagps/gpsrdocker` [cite: 1280]

---

## Citation

Agrawal P, Kumar R, Usmani SS, Dhall A, Patiyal S, Sharma N, et al. (2019).  
**GPSRdocker: A Docker-based Resource for Genomics, Proteomics and Systems biology.** *bioRxiv* 827766.  
[cite_start][https://doi.org/10.1101/827766](https://doi.org/10.1101/827766) [cite: 1094]

---

## About the Platform

[cite_start]GPSRdocker addresses the challenges of traditional web-based services, such as internet speed limitations, computing power restrictions, and data security concerns[cite: 1136, 1203, 1209]. [cite_start]By utilizing **Docker containerization**, it provides a portable environment that ensures hardware/software compatibility and eliminates complex installation dependencies[cite: 1159, 1211, 1252].

The container is categorized into three main components:
1.  [cite_start]**General Scripts**: Small Perl and Python programs for generating features like protein composition[cite: 1152, 1154].
2.  [cite_start]**Supporting Software**: Integrated packages for data processing and model development, including PSI-BLAST, CD-HIT, WEKA, and $SVM^{light}$[cite: 1155, 1330].
3.  [cite_start]**Standalone Prediction Packages**: Core software for predicting functions or classes of biomolecules across six major categories[cite: 1156, 1342].

---

## Key Categories and Standalone Tools



[Image of protein structure prediction types]


### 1. Protein Structure Prediction
[cite_start]Tools to predict alpha/beta/gamma turns, transmembrane regions, and surface accessibility[cite: 1388].
* [cite_start]**ALPHApred**: Predicts alpha-turns using neural networks[cite: 1394].
* [cite_start]**SARpred**: Predicts real-value solvent accessibility[cite: 1394].
* [cite_start]**TBBpred**: Predicts transmembrane beta-barrel regions[cite: 1394].

### 2. Functional Annotation of Proteins
[cite_start]Methods for predicting subcellular localization and protein binding properties[cite: 1404, 1413].
* [cite_start]**ALGpred**: Predicts allergenic proteins and maps IgE epitopes[cite: 1423].
* [cite_start]**ESLpred2**: Advanced subcellular localization for eukaryotic proteins[cite: 1423].
* [cite_start]**RNApred**: Predicts RNA-binding proteins[cite: 1427].

### 3. Vaccinomics
[cite_start]Tools for immunogenomics and epitope-based vaccine design[cite: 1436, 1447].
* [cite_start]**abcpred**: Mapping B-cell epitopes using neural networks[cite: 1451].
* [cite_start]**ProPred / ProPred1**: Predicts MHC Class-II and Class-I binding sites[cite: 1451, 1455].
* [cite_start]**vaxinpad**: Designing peptide-based vaccine adjuvants[cite: 1455].

### 4. Genomics
[cite_start]Biomarker identification and genome annotation[cite: 1466, 1469].
* [cite_start]**cancercsp**: Gene expression-based biomarkers for renal cancer[cite: 1473].
* [cite_start]**desirm**: Designing highly efficient siRNAs[cite: 1477].

### 5. BioDrugs
[cite_start]In silico screening for bioactive drugs and therapeutic peptides[cite: 1502].
* [cite_start]**AntiCP**: Prediction and design of anticancer peptides[cite: 1509].
* [cite_start]**ToxinPred**: Predicting and designing toxic/non-toxic peptides[cite: 1509].
* [cite_start]**AntiTbPred**: Predicting peptides with bactericidal activity against *Mycobacterium*[cite: 1509].

### 6. Interactome
[cite_start]Study of molecular interactions among proteins and small molecules[cite: 1524, 1531].
* [cite_start]**ATPint / GTPbinder**: Identification of ATP and GTP binding sites[cite: 1535].
* [cite_start]**GlycoEP / GlycoPP**: Prediction of glycosylation sites in eukaryotes and prokaryotes[cite: 1535].

---

## Implementation & Usage

[cite_start]GPSRdocker provides a flexible platform that can run on any operating system or be ported to the cloud[cite: 1159].

### Basic Commands:
1.  [cite_start]**Pull the Image**: [cite: 1280]  
    `docker pull raghavagps/gpsrdocker`
2.  **Run the Container**: [cite: 1284]  
    `docker run -i -t raghavagps/gpsrdocker`
3.  **Install Software Packages**: [cite: 1285]  
    Inside the image, run: `/gpsr/gpsr_install.pl`

---

## Key Advantages
* [cite_start]**Data Security**: Standalone operation allows researchers to keep confidential data local[cite: 1610, 1611].
* [cite_start]**High Throughput**: Capable of processing large datasets that typically exceed webserver limits[cite: 1602].
* [cite_start]**No Internet Required**: Once the image is pulled, all tools function offline[cite: 1619, 1620].

---

## Contact & Support

**Prof. Gajendra P.S. [cite_start]Raghava** Head, Department of Computational Biology [cite: 1117]  
[cite_start]Indraprastha Institute of Information Technology (IIIT-Delhi), India[cite: 1107].  
[cite_start]**Email**: raghava@iiitd.ac.in [cite: 1115]

---

## License

[cite_start]This resource is available free for academic use under the **aCC-BY 4.0 International license**[cite: 1095, 1166].
