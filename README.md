# AuroraLineProfileAnalysis
Python codes to measure and analyze the intensity profiles of INCENP-mCherry along lines crossing two sister kinetochores labeled with GFP

Data: U2OS cells with GFP-labeled kinetochore and mCherry-labeled CPC complex

The following is the description of the codes:

1. lineprofAnalysis.ipynb identifies kinetochores (using trackpy library), pair sister kinetochores based on the distance along and perpendicular to metaphase plate, and generates line profiles of 488 and 560 channel signals along lines crossing two sister kinetochores. Erroneous kinetochore pairs are detected and removed by comparing the mCherry intensity between two kinetochores and outside kinetochore pairs.  

2. Dist_vs_INCENP_avg-ALL.ipynb averages the line profiles in different groups of kinetochore pairs with different ranges of K-K distance. It generates plots of the average line profiles, and charateristics of the average line profiles (e.g. peak intensity, width, total intensity, intensity at kinetochore) as a function of K-K distance.

