# Cancer-autoimmunity_meta-analysis
We conducted a meta-analysis on the relative abundance data of microbiome features collected from cancer and autoimmune diseases. 
We conducted the analysis following below steps. 
1. First, we calculated fold-change ratio (mean abundance in disease/mean abundance in control) from the relative abundance data (column name “foldchange”)
3. We collected p value, number of total samples data from the original studies.
5. We then calculated the standard error using the fold change ratio, p values and sample size according to this paper https://www.bmj.com/content/343/bmj.d2090.long using r package ‘dmetar’ (version 0.0.9000) Ref ). www.bookdown.org/MathiasHarrer/Doing_Meta_Analysis_in_R/ .
See r script 
4. Export the standard error data from r and paste it to the existing genus data file and make a new file name : “genus_se_calculated”
5. Make the file ready for analysis. 
See r scipt
5. We conducted the meta-analysis only on genera for which we found the relative abundance data in at least four studies. By this criteria, six genera had sufficient abundance data available in at least four studies.
