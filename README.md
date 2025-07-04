# iDrosophila1: A genome-scale metabolic network model of *Drosophila melanogaster*

**Contributors:** [Muberra Fatma Cesur](https://orcid.org/0000-0003-2993-0634), [‪Arianna Basile‬](https://orcid.org/0000-0003-2461-5221), [‪Kiran Raosaheb Patil‬](https://orcid.org/0000-0002-6166-8640), [Tunahan Cakir‬](https://orcid.org/0000-0001-8262-4420)


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

•	The model is shared in MATLAB .mat, .xml (SBML), and .json formats, which are compatible with COBRA Toolbox model structure. Download the model from GitHub page or directly clone the repository (using GitBash or downloading the zipped files by left-clicking the 'Code' drop-down menu) to your local drive.

•	As follows, use MATLAB *load* and *save* functions to load and save the model in .mat format. For more information, please see https://sysbiogtu.github.io/.

		cd ./code
		model = load('iDrosophila1.mat');   % Load the model
		save('iDrosophila1.mat');   % Save the model

•	To read the model in SBML format, use *readCbModel* function provided by [COBRA Toolbox](https://opencobra.github.io/cobratoolbox/stable/).

		cd ./code
		model = readCbModel('iDrosophila1.xml');   % Read the model

  •	Example code for simulating *Drosophila* growth under the Holidic diet (HD) is available in the 'Example Growth Simulation' folder.
  
### **For citation, please use the following reference:**
Cesur, M. F., Basile, A., Patil, K. R., & Çakır, T. (2023). A new metabolic model of Drosophila melanogaster and the integrative analysis of Parkinson’s disease. Life Science Alliance, 6(8).
