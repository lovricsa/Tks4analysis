# Tks4analysis

## Purpose
The objective of this R Markdown code is to reproduce the correlation, multiple logistic regression and principal component analysis steps in the publaction Tilajka et. al.

## Usage
Keep the organization of the folders and run the .Rmd file. 

## Credits
Help from Daniel Kiss is greatly acknowledged.

## Licence
The code is under GNU GPL-3 license (https://www.gnu.org/licenses/gpl-3.0.html).

## Session information
R version 4.3.1 (2023-06-16)

Platform: x86_64-pc-linux-gnu (64-bit)
Running under: Ubuntu 22.04.3 LTS

Matrix products: default
BLAS:   /usr/lib/x86_64-linux-gnu/blas/libblas.so.3.10.0 
LAPACK: /usr/lib/x86_64-linux-gnu/lapack/liblapack.so.3.10.0

locale:
```
 [1] LC_CTYPE=en_US.UTF-8       LC_NUMERIC=C               LC_TIME=hu_HU.UTF-8        LC_COLLATE=en_US.UTF-8     LC_MONETARY=hu_HU.UTF-8   
 [6] LC_MESSAGES=en_US.UTF-8    LC_PAPER=hu_HU.UTF-8       LC_NAME=C                  LC_ADDRESS=C               LC_TELEPHONE=C            
[11] LC_MEASUREMENT=hu_HU.UTF-8 LC_IDENTIFICATION=C   
```   

time zone: Europe/Budapest
tzcode source: system (glibc)

attached base packages:
```[1] stats     graphics  grDevices utils     datasets  methods   base     
```

other attached packages:
``` [1] class_7.3-22       umap_0.2.10.0      corrplot_0.92      readr_2.1.5        ggcorrplot_0.1.4.1 pROC_1.18.5        caret_6.0-94      
 [8] lattice_0.22-5     dplyr_1.1.4        tibble_3.2.1       ggplot2_3.4.4      openxlsx_4.2.5.2  
 ```

loaded via a namespace (and not attached):
```  [1] gridExtra_2.3        rlang_1.1.3          magrittr_2.0.3       e1071_1.7-14         compiler_4.3.1       png_0.1-8            systemfonts_1.0.5   
  [8] vctrs_0.6.5          reshape2_1.4.4       stringr_1.5.1        pkgconfig_2.0.3      crayon_1.5.2         fastmap_1.1.1        backports_1.4.1     
 [15] labeling_0.4.3       utf8_1.2.4           rmarkdown_2.25       prodlim_2023.08.28   tzdb_0.4.0           ragg_1.2.7           purrr_1.0.2         
 [22] bit_4.0.5            xfun_0.41            jsonlite_1.8.8       recipes_1.0.9        parallel_4.3.1       cluster_2.1.6        R6_2.5.1            
 [29] RColorBrewer_1.1-3   stringi_1.8.3        reticulate_1.35.0    ComplexUpset_1.3.3   limma_3.58.1         parallelly_1.36.0    rpart_4.1.23        
 [36] lubridate_1.9.3      bookdown_0.37        Rcpp_1.0.12          iterators_1.0.14     knitr_1.45           future.apply_1.11.1  base64enc_0.1-3     
 [43] Matrix_1.6-5         splines_4.3.1        nnet_7.3-19          timechange_0.3.0     tidyselect_1.2.0     viridis_0.6.5        rstudioapi_0.15.0   
 [50] yaml_2.3.8           timeDate_4032.109    codetools_0.2-19     listenv_0.9.1        plyr_1.8.9           withr_3.0.0          askpass_1.2.0       
 [57] evaluate_0.23        foreign_0.8-86       future_1.33.1        survival_3.5-7       proxy_0.4-27         zip_2.3.1            pillar_1.9.0        
 [64] rsconnect_1.2.1      checkmate_2.3.1      foreach_1.5.2        stats4_4.3.1         generics_0.1.3       vroom_1.6.5          hms_1.1.3           
 [71] munsell_0.5.0        scales_1.3.0         globals_0.16.2       apcluster_1.4.11     glue_1.7.0           Hmisc_5.1-1          tools_4.3.1         
 [78] dendextend_1.17.1    data.table_1.15.0    RSpectra_0.16-1      ModelMetrics_1.2.2.2 gower_1.0.1          locfit_1.5-9.8       grid_4.3.1          
 [85] tidyr_1.3.1          ipred_0.9-14         edgeR_4.0.15         colorspace_2.1-0     nlme_3.1-164         patchwork_1.2.0      htmlTable_2.4.2     
 [92] Formula_1.2-5        cli_3.6.2            textshaping_0.3.7    fansi_1.0.6          viridisLite_0.4.2    lava_1.7.3           gtable_0.3.4        
 [99] digest_0.6.34        htmlwidgets_1.6.4    farver_2.1.1         htmltools_0.5.7      lifecycle_1.0.4      hardhat_1.3.1        statmod_1.5.0       
[106] openssl_2.1.1        bit64_4.0.5          MASS_7.3-60.0.1   
```  
