# iDrosophila1: A genome-scale metabolic network model of *Drosophila melanogaster*

**Contributors:** [Muberra Fatma Cesur](https://www.gtu.edu.tr/en/personel/356/1558/display.aspx), [‪Kiran Raosaheb Patil‬](https://www.mrc-tox.cam.ac.uk/staff/kiran-patil), [Tunahan Cakir‬](https://www.gtu.edu.tr/en/personel/356/2201/display.aspx)


The latest version of iDrosophila1 is shared here, which is a genome-scale metabolic network model for *Drosophila melanogaster*. The reconstruction process of iDrosophila1 is detailed below:

<p align="center"><img src="https://github.com/SysBioGTU/iDrosophila/blob/main/Figures/Flowchart_GitHub.jpg" width="730">


**Common curation steps** refer to the revisions (name standardization, the curations of metabolic redundancy, stoichiometric consistency, and missing/incomplete components), which were commonly applied to the orthology-based draft *Drosophila* model and *Drosophila*-specific KEGG-MetaCyc network in the reconstruction process. Note that each model component was carefully examined in the model curation step.

> The metabolic content of iDrosophila1 model is summarized in the following table. In addition, the model contains eight intracellular compartments (cytosol, nucleus, golgi apparatus, mitochondria, mitochondrial intermembrane space, endoplasmic reticulum, lysosome, and peroxisome).
	
<div align="center">
	
   | Organism                        | Reactions             | Metabolites            | Genes                 | Model Version        |
   |:-------------------------------:|:---------------------:|:----------------------:|:---------------------:|:--------------------:|
   | _Drosophila melanogaster_       |          8,230        |           6,990        |         2,388         |       1.1.0          |		

</div>

### **Model Installation**

•	The model is shared in MATLAB .mat format, which is compatible with COBRA Toolbox model structure. Download the model from GitHub page or directly clone the repository (using GitBash or downloading the zipped files by left-clicking the 'Code' drop-down menu) to your local drive.

•	As follows, use MATLAB load() and save() functions to load and save the model in .mat format.

		cd ./code
		model = load(‘iDrosophila1.mat’);   % Load the model
		save('iDrosophila1.mat');   % Save the model

### **For citation, please use the following reference:**
Cesur, M. F., Patil, K., Cakir, T. (2022). A genome-scale metabolic model of Drosophila melanogaster for integrative analysis of brain diseases. bioRxiv, doi: https://doi.org/10.1101/2022.08.22.504778.
