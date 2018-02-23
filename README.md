<p align="center"> 
<img src="https://github.com/larawierenga/Qoala-T-under-construction/blob/master/Figures/KoalaFramework-Logo%20copy%202.jpg" width="25%" height="25%"> 
</p> 

# Qoala-T (Under construction)
  
### *A supervised-learning tool to assess accuracy of manual quality control of automatic segmented MRI data*

Version (1)   21 feb 2018 <br />
Qoala-T is developed in the [Brain and development research center](https://www.brainanddevelopmentlab.nl) by [Lara Wierenga](https://www.brainanddevelopmentlab.nl/index.php/people/post-docs/181-post-doctoral-researchers/273-lara-wierenga) and [Eduard Klapwijk](https://www.brainanddevelopmentlab.nl/index.php/people/post-docs/181-post-doctoral-researchers/287-eduard-klapwijk)
<br />

About
-----
Qoala-T is a supervised learning tool that asseses accuracy of manual quality controled T1 imaging scans and their automated neuroanatomical labeling processed in FreeSurfer. It is particularly intended to use in developmental datasets. 
This package contains data and R code as described in Klapwijk et al., (in prep). The protocol of our in hosue developped manual QC procedure can be found [here](https://github.com/larawierenga/Qoala-T-under-construction/blob/master/Github_Qoala-T_Manual_QC.pdf)  

### Running Qoala-T
- To be able to run Qoala-T T1 MRI images should be processed in [FreeSurfer V6.0](https://surfer.nmr.mgh.harvard.edu/fswiki/DownloadAndInstall). 
- Next run [stats2table_bash_qoala_t.sh](https://github.com/larawierenga/Qoala-T-under-construction/blob/master/stats2table_bash_qoala_t.sh) to create an input file for the Qoala-T tool. 


### A. Predicting scan Qoala-T score by using Braintime model
- Open [Qoala_T_step4_validation_novel_data_github.R](https://github.com/larawierenga/Qoala-T-under-construction/blob/master/Qoala_T_A_model_based_github.R) and follow the instructions.
- With this R script Qoala-T scores for a dataset are estimated using a supervised learning model. This model is based on 784 T1-weighted imaging scans of subjects aged between 8 and 25 years old (53% females). The manual quality assesement is descibed in the Qoala-T manual [Qoala_T_manual](https://github.com/larawierenga/Qoala-T-under-construction/blob/master/Qoala_T_Manual.pdf).
- An example output file showing the Qoala-T score of each scan is displayed below. This figure shows the number of included and excluded predictions. The grey area represents the scans that are recommended for manual quality assesment. <br /> <br /> 
![Example output file](https://github.com/larawierenga/Qoala-T-under-construction/blob/master/Figures/Figure_Rating_model_based_simulated_data_step4%20copy.jpg "Example output") <br /> 


### B. Predicting scan Qoala-T score by rating 10% of your data
- Open [Qoala_T_step2_10perc_github.R](https://github.com/larawierenga/Qoala-T-under-construction/blob/master/Qoala_T_B_subset_based_github.R) and follow the instructions.
- With this R script an inhouse developped manual QC protocol can be applied on a subset of the dataset (e.g. 10%, the larger the set, the more reliable the results).  <br /> <br />
A flowchart of these processes can be observed in A and B below. <br /> 
![FlowChart](https://github.com/larawierenga/Qoala-T-under-construction/blob/master/Figures/Flowchart_github.jpg "FlowChart")

Support and communication
-------------------------
If you have any question or suggestion don't hesitate to get in touch:
<l.m.wierenga@fsw.leidenuniv.nl> or <e.t.klapwijk@fsw.leidenuniv.nl>


Citation
--------
**When using Qoala-T please include the following citation:**

Klapwijk, E.T., van de Kamp, F., Meulen, M., Peters, S. and Wierenga, L.M. (in prep). *Qoala-T: A supervised-learning tool to assess accuracy of manual quality control of automated neuroanatomical labeling in developmental MRI data.*


Authors
-------
Eduard T. Klapwijk, Ferdi van de Kamp, Mara van der Meulen, Sabine Peters, and Lara M. Wierenga

<br />
<br />
Copyright (C) 2017 Lara Wierenga - Leiden University, Brain and Development Research Center<br />
All rights reserved

----


