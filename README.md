# RP1-project
Circuit Topology for the analysis of chromatin topology in patients with Tuberculosis

This project contains all the codes used for my master project. 
The accepted formats: For this pipeline .hic files were generated from raw sequence dataa using DLO-HiC-Tools from GangCaoLab(https://github.com/GangCaoLab/DLO-HiC-Tools) for the Ensemble data. Single Cell Hi-C data was already prepared in pairs txt. files.
Instructions: The analysis can only be completed with the use of genome_topology pipeline(https://github.com/barbaroo/genome_topology) and JuicerTools from aidenlab(https://github.com/aidenlab/JuicerTools).

1.Start the analysis with Bulk_paired for the Bulk/Ensemble data. This code will generate contact pairs files from HiC that can be later used for Circuit Topology analysis. In addition this code produces images of Hi-C.

2. Then run Sci_dataframes to generate different resolutions pairs txt. files of Single Cell Hi-C.

3. Follow up with Sci_CT_preparation where the pairs txt. files can be loaded and the Circuit Topology matrices will be calculated.

4. Next the Sci_CT_images creates distribution images, violinplots and calculates statistics.

5. In order to compare Circuit Topology with RNA sequence expression the code RNA_seq_dataframes can be used. This code generates dataframes to use in later analysis.

6. Vulcano_RNA generates different volcano plots per comparison. In this code we also calculated the most significant genes with the lowest p-value and highest lfc.

7. RNA_CT_correlation was used to compare the Circuit Topology matrice entangled to RNA sequence expression. This code calculates the significance and correlation value.
