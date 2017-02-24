# GNPS-Trinity workflow combines LC-MS feature detection, molecular networking, and in silico annotation

## DESCRIPTION
This workflow is jointly developed by the Dorrestein's Lab (UC San Diego), Theodore Alexandrov's lab (EMBL), and Sebastian Boecker's lab (Jena University) that aims at bringing together LC-MS feature detection tools (OpenMS, Optimus workflow), in silico annotation (Sirius3, CSI:FingerID), and molecular networking (GNPS, http:/gnps.ucsd.edu).

The key improvements offered by the GNPS-Trinity workflow are:
+ (1) mapping back the intensity of the LC-MS feature detected across samples as pie-chart diagram directly into the molecular networks for semi-quantitative purpose,
+ (2) discriminating isobaric compounds, 
+ (3) mapping the in silico annotation generated by Sirius3 and CSI:FingerID into the molecular networks.

The GitHub contains the scripts and instructions of the workflow allowing to combine the outputs of Optimus, Sirius and GNPS, and to visualize the result into Cytoscape. The workflow has been designed by Louis-Felix Nothias (Dorrestein Lab UCSD) and the scripts coded by Madeleine Ernst (Dorrestein Lab and Copenhagen University). They are available as Knime workflows and Jupyter notebooks.

IMPORTANT: IT IS NOT RECOMMENDED TO USE MORE THAN 300-500 SAMPLES.

## YOUTUBE VIDEO TUTORIAL FOR GNPS-TRINITY ##
Please refer to this video: https://www.youtube.com/watch?v=zDcY7iuvyQY

## INSTALLATION ##
GNPS-TRINITY WORKFLOW (in Knime, recommended):
+ Install Knime and Optimus workflow. See Optimus GitHub for installation [use Express installation procedure] https://github.com/alexandrovteam/Optimus. 
+ Download the GNPS_TRINITY_v_0.1_2016.12.07.zip and import the workflow in Knime. Refer to the tutorial video for instructions https://www.youtube.com/watch?v=zDcY7iuvyQY. 
+ Download you will have to install R https://cran.r-project.org/. -For Windows, R should be installed in the folder "C:/ProgramFiles/R" or path specified accordingly.

See the [obsolete] documentation on GNPS for more instructions https://bix-lab.ucsd.edu/display/Public/GNPS+Trinity+workflow.

### OPTIONAL FEATURES ###
- GNPS-TRINITY WORKFLOW (in Jupyter notebook): Download the Jupyter workflow and change the filename according to your input file.
- GENERATE A GROUP MAPPING FROM A METADATA TABLE: Download the Generate_GroupMapping_file_from_Metadata_table_v_0.1_2016.12.07.zip, and use it to create a GNPS_group_mapping_file.txt using a metadata_table.csv.

### Optimus workflow ###
Optimus workflow is a LC-MS feature analysis tool using OpenMS, developed by Ivan Protsyuk at Theodore Alexandrov group at EMBL https://github.com/alexandrovteam/Optimus.

### Sirius and CSIFingerID for in silico MS/MS annotation ###

Sirius3 a new java-based software framework for discovering a landscape of de-novo identification of metabolites using single and tandem mass spectrometry developed by Kai Dührkop and Sebastian Boecker at Jena University. This tool uses isotopic pattern, analysis and fragmentation tree to calculate candidate molecular formula, and now also integrates CSI:FingerID to generate candidate structures https://bio.informatik.uni-jena.de/software/sirius/.

### License
The content of this project is licensed under the GNU GENERAL PUBLIC LICENSE 3, see LICENSE.md.

### Citation:
Sharing and community curation of mass spectrometry data with Global Natural Products Social Molecular Networking. Nature Biotechnology 34, 828–837 (2016) doi:10.1038/nbt.3597 http://www.nature.com/nbt/journal/v34/n8/full/nbt.3597.html
