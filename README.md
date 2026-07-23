Friends dataset: fMRI data of naturalistic TV viewing and recall

This project includes data from...
- participants who viewed and recalled a two-part episode of Friends (season 1, ep 16-17)
- participants who rated pair-wise causality between events
- two groups of participants who performed event segmentation ('eventseg.zip'/'event_seg.ipynb')
 
The original published study investigated how causality (in narratives) affected behavioral recall and neural outcomes.

Files --
Behavioral:
- FriendsRecallScoring.xlsx: Recall information for fMRI participants. Imported into 'recallBehav.ipynb'.
- eventseg.zip. Contains event segmentation data from both groups. Unzip and point ‘event_seg.ipynb’ to its location.
- event_seg.ipynb. Imports stimulus information and event segmentation ratings and performs some analyses for Figure 5.
- ‘friendsSRMStoryBoard.xlsx’. Contains stimulus information for the independent stimulus (‘task-srm’). Technically, this is only used in the neural analysis section. 
- ‘friendsStoryBoard.xlsx’. Contains stimulus information for the main stimulus (‘task-view’). This is imported in both behavioral and neural analysis scripts.
- ratings.zip: Excel files with causality / importance ratings. Unzip and point accompanying .ipynb files to its location.
- recallBehav.ipynb. Imports recall information and integrates other measurements like causality ratings; performs analysis plotted in figure 2; outputs relevant files for neural analyses.

Neural:
- GSBS.ipynb. Code for running greedy state boundary search on SRMified neural data and creates some plots in figure 5.
- Import_all.ipynb. Imports fMRI data from fMRIPrep, performs pre-processing steps, save data ready for analysis.
- SRM.ipynb. Perform share response model analyses first on an independence stimulus (‘task-srm’) and then saves main data (‘task-view’) in correct format
- eventStatePatterns.ipynb. Performance event-based representational similarity analyses in figures 3-4. 

Please see individual scripts for more information about each analysis and the paper for more information in general.

Please contact James Antony (james.ward.antony@gmail.com) if you have any questions or observe irregularities in the data. 

Please also see the OpenNeuro folder for accompanying fMRIprepped data: 

Behavioral analyses can be run with data on here. To run new neural analyses, one would need to run Import_all on the OpenNeuro data and store appropriately, then use outputs in the later scripts.
