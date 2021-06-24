# dp5_analysis

## Purpose
The objective of this R Markdown code is to reproduce the building of the 5 dietary patterns (DP5) obtained via Dirichlet Multinomial Mixture (DMM) models in *Cotillard at al., A posteriori dietary patterns better explain variations of the gut microbiome than individual markers in the American Gut Project, submitted to AJCN.* It also includes code for associations with 16S gut microbiome using DESeq2.

## Usage
Load all directories keeping the same organization and just run the .Rmd file after installing the require packages.

## Credits
Thank you to Mathilde Saccareau and Julien Tap (https://github.com/tapj) for their contributions.

## Licence
GNU GPL-3

## Session information
R version 4.0.3 (2020-10-10)

Platform: x86_64-w64-mingw32/x64 (64-bit)

Running under: Windows 10 x64 (build 19041)

attached base packages:
```
[1] parallel  stats4    stats     graphics  grDevices utils     datasets  methods   base     
```

other attached packages:
```
 [1] DESeq2_1.28.1               SummarizedExperiment_1.18.2 DelayedArray_0.14.1         Biobase_2.48.0              GenomicRanges_1.40.0       
 [6] GenomeInfoDb_1.24.2         phyloseq_1.32.0             vegan_2.5-6                 lattice_0.20-41             permute_0.9-5              
[11] reshape2_1.4.4              gtools_3.8.2                multcompView_0.1-8          compareGroups_4.4.5         DT_0.16                    
[16] matrixStats_0.57.0          effsize_0.8.1               dplyr_1.0.2                 scales_1.1.1                DirichletMultinomial_1.30.0
[21] IRanges_2.22.2              S4Vectors_0.26.1            BiocGenerics_0.34.0         fpc_2.2-8                   glue_1.4.2                 
[26] ggplot2_3.3.2              
```

loaded via a namespace (and not attached):
```
  [1] uuid_0.1-4             backports_1.2.0        systemfonts_0.3.2      plyr_1.8.6             igraph_1.2.6           splines_4.0.3         
  [7] crosstalk_1.1.0.1      BiocParallel_1.22.0    digest_0.6.27          foreach_1.5.1          htmltools_0.5.0        viridis_0.5.1         
 [13] fansi_0.4.1            memoise_1.1.0          magrittr_2.0.1         Rsolnp_1.16            cluster_2.1.0          Biostrings_2.56.0     
 [19] annotate_1.66.0        officer_0.3.15         prettyunits_1.1.1      colorspace_2.0-0       blob_1.2.1             rvest_0.3.6           
 [25] xfun_0.19              crayon_1.3.4           RCurl_1.98-1.2         jsonlite_1.7.1         genefilter_1.70.0      survival_3.2-7        
 [31] iterators_1.0.13       ape_5.4-1              kableExtra_1.3.1       gtable_0.3.0           zlibbioc_1.34.0        XVector_0.28.0        
 [37] webshot_0.5.2          kernlab_0.9-29         Rhdf5lib_1.10.0        prabclus_2.3-2         DEoptimR_1.0-8         DBI_1.1.0             
 [43] Rcpp_1.0.5             viridisLite_0.3.0      xtable_1.8-4           progress_1.2.2         bit_4.0.4              mclust_5.4.6          
 [49] truncnorm_1.0-8        htmlwidgets_1.5.2      httr_1.4.2             RColorBrewer_1.1-2     modeltools_0.2-23      ellipsis_0.3.1        
 [55] mice_3.11.0            farver_2.0.3           pkgconfig_2.0.3        XML_3.99-0.5           flexmix_2.3-17         nnet_7.3-14           
 [61] locfit_1.5-9.4         labeling_0.4.2         tidyselect_1.1.0       rlang_0.4.8            AnnotationDbi_1.50.1   munsell_0.5.0         
 [67] tools_4.0.3            cli_2.1.0              generics_0.1.0         RSQLite_2.2.1          ade4_1.7-16            broom_0.7.2           
 [73] evaluate_0.14          biomformat_1.16.0      stringr_1.4.0          yaml_2.2.1             knitr_1.30             bit64_4.0.5           
 [79] zip_2.1.1              robustbase_0.93-6      purrr_0.3.4            dendextend_1.14.0      nlme_3.1-150           xml2_1.3.2            
 [85] compiler_4.0.3         rstudioapi_0.13        geneplotter_1.66.0     tibble_3.0.4           stringi_1.5.3          HardyWeinberg_1.6.8   
 [91] gdtools_0.2.2          Matrix_1.2-18          multtest_2.44.0        vctrs_0.3.5            pillar_1.4.7           lifecycle_0.2.0       
 [97] data.table_1.13.2      bitops_1.0-6           flextable_0.5.11       R6_2.5.0               gridExtra_2.3          writexl_1.3.1         
[103] codetools_0.2-18       assertthat_0.2.1       MASS_7.3-53            chron_2.3-56           rhdf5_2.32.0           withr_2.3.0           
[109] GenomeInfoDbData_1.2.3 diptest_0.75-7         mgcv_1.8-33            hms_0.5.3              grid_4.0.3             tidyr_1.1.2           
[115] class_7.3-17           rmarkdown_2.5          base64enc_0.1-3       
```
