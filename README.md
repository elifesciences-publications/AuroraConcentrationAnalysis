# AuroraConcentrationAnalysis
Python codes to measure and analyze the intensity of INCENP-mCherry the location of NDC80 labeled with GFP

Data: Spinning-disk images of U2OS cells with mNeonGreen-labeled Nuf2 and mCherry-labeled INCENP

The following is the description of the codes:

1. track_pair_lineprofs.ipynb identifies kinetochores (using trackpy library), pair sister kinetochores based on the distance along and perpendicular to metaphase plate, and generates line profiles of 488 and 560 channel signals along lines crossing two sister kinetochores. Erroneous kinetochore pairs are detected and removed by comparing the mCherry intensity between two kinetochores and outside kinetochore pairs.  

2. Dist_vs_INCENP_avg.ipynb (1) imports the outputs from track_pair_lineprofs.ipynb and INCENP-mCherry images; (2) measures INCENP-mCherry intensities at NDC80; (3) normalizes the INCENP-mCherry intensity at NDC80 based on the INCENP-mCherry intensity at the midpoint between sister kinetochores and cytoplasmic background on cell-to-cell basis; and (4) averages the normalized intensities within groups of kinetochores with similar K-K distances. 

3. PlotAnalysisResults.ipynb generates plots of analysis results, and performs model fitting and statistical tests.

