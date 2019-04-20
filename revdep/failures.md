# eegc

<details>

* Version: 1.8.1
* Source code: ???
* Date/Publication: 2018-12-21
* Number of recursive dependencies: 154

Run `revdep_details(,"eegc")` for more info

</details>

## In both

*   R CMD check timed out
    

*   checking Rd cross-references ... WARNING
    ```
    Missing link or links in documentation object 'barplotEnrich.Rd':
      ‘[DOSE]{barplot.enrichResult}’
    
    See section 'Cross-references' in the 'Writing R Extensions' manual.
    ```

*   checking installed package size ... NOTE
    ```
      installed size is 11.2Mb
      sub-directories of 1Mb or more:
        data  10.5Mb
    ```

*   checking R code for possible problems ... NOTE
    ```
    ...
    grnPlot: no visible global function definition for ‘legend’
    markerScatter: no visible global function definition for
      ‘colorRampPalette’
    markerScatter: no visible global function definition for ‘plot’
    markerScatter: no visible global function definition for ‘points’
    markerScatter: no visible global function definition for ‘lm’
    markerScatter: no visible global function definition for ‘abline’
    markerScatter: no visible global function definition for ‘text’
    markerScatter: no visible global function definition for ‘legend’
    Undefined global functions or variables:
      abline adjustcolor axis colorRampPalette control density dev.copy2pdf
      legend lines lm model.matrix p.adjust par phyper plot points quantile
      results text title treat
    Consider adding
      importFrom("grDevices", "adjustcolor", "colorRampPalette",
                 "dev.copy2pdf")
      importFrom("graphics", "abline", "axis", "legend", "lines", "par",
                 "plot", "points", "text", "title")
      importFrom("stats", "density", "lm", "model.matrix", "p.adjust",
                 "phyper", "quantile")
    to your NAMESPACE file.
    ```

# ELMER

<details>

* Version: 2.6.3
* Source code: ???
* Date/Publication: 2019-04-02
* Number of recursive dependencies: 209

Run `revdep_details(,"ELMER")` for more info

</details>

## In both

*   checking examples ... ERROR
    ```
    ...
    > 
    > data <- ELMER:::getdata("elmer.data.example")
    > pair <- data.frame(Probe = c("cg19403323","cg19403323", "cg26403223"),
    +                    GeneID = c("ENSG00000196878", "ENSG00000009790", "ENSG00000009790" ),
    +                    Symbol = c("TRAF3IP3","LAMB3","LAMB3"),
    +                    Raw.p =c(0.001,0.00001,0.001),
    +                    Pe = c(0.001,0.00001,0.001))
    > schematic.plot(data,
    +                group.col = "definition",
    +                group1 = "Primary solid Tumor",
    +                group2 = "Solid Tissue Normal",
    +                pair = pair,
    +                byProbe = "cg19403323")
    Searching for the 20 near genes
    Identifying gene position for each probe
    
      |                                                                            
      |                                                                      |   0%
      |                                                                            
      |======================================================================| 100%Error: GenomicInteractions package is needed for this function to work. Please install it.
    Execution halted
    ```

*   R CMD check timed out
    

*   checking for code/documentation mismatches ... WARNING
    ```
    Codoc mismatches from documentation object 'motif.enrichment.plot':
    motif.enrichment.plot
      Code: function(motif.enrichment, significant = NULL, dir.out = "./",
                     save = TRUE, label = NULL, title = NULL, width = 10,
                     height = NULL, summary = FALSE)
      Docs: function(motif.enrichment, significant = NULL, dir.out = "./",
                     save = TRUE, label = NULL, title = NULL, summary =
                     FALSE, width = 10, height = NULL)
      Mismatches in argument names:
        Position: 7 Code: width Docs: summary
        Position: 8 Code: height Docs: width
        Position: 9 Code: summary Docs: height
    ```

*   checking package dependencies ... NOTE
    ```
    Package suggested but not available for checking: ‘GenomicInteractions’
    ```

*   checking installed package size ... NOTE
    ```
      installed size is 83.5Mb
      sub-directories of 1Mb or more:
        doc  82.9Mb
    ```

*   checking dependencies in R code ... NOTE
    ```
    There are ::: calls to the package's namespace in its code. A package
      almost never needs to use ::: for its own objects:
      'getInfiniumAnnotation'
    ```

*   checking R code for possible problems ... NOTE
    ```
    ...
    getTFBindingSites: no visible global function definition for 'resize'
    getTFtargets: no visible binding for global variable 'TF'
    heatmapGene: no visible global function definition for
      'subsetByOverlaps'
    heatmapGene: no visible binding for global variable 'mae'
    motif.enrichment.plot: no visible binding for global variable 'y'
    motif.enrichment.plot: no visible binding for global variable 'x'
    motif.enrichment.plot: no visible binding for global variable 'z'
    motif.enrichment.plot: no visible binding for global variable 'upperOR'
    motif.enrichment.plot: no visible binding for global variable 'lowerOR'
    motif.enrichment.plot: no visible binding for global variable 'motif'
    motif.enrichment.plot: no visible binding for global variable 'OR'
    scatter: no visible binding for global variable 'value'
    scatter: no visible binding for global variable 'mae'
    scatter.plot: no visible binding for global variable 'ID'
    scatter.plot: no visible binding for global variable 'GeneID'
    Undefined global functions or variables:
      DistanceTSS FDR Gene GeneID Hugo_Symbol ID OR Probe Side Sides TF
      enriched_motifs ensembl_gene_id label lowerOR mae motif motif.target
      potential.TF.family potential.TF.subfamily pvalue resize
      subsetByOverlaps tf.target upperOR value x y z
    ```

# gdalUtils

<details>

* Version: 2.0.1.14
* Source code: https://github.com/cran/gdalUtils
* Date/Publication: 2018-04-23 03:23:04 UTC
* Number of recursive dependencies: 11

Run `revdep_details(,"gdalUtils")` for more info

</details>

## In both

*   R CMD check timed out
    

# psichomics

<details>

* Version: 1.8.2
* Source code: ???
* URL: https://github.com/nuno-agostinho/psichomics
* BugReports: https://github.com/nuno-agostinho/psichomics/issues
* Date/Publication: 2019-03-27
* Number of recursive dependencies: 220

Run `revdep_details(,"psichomics")` for more info

</details>

## Newly broken

*   checking whether package ‘psichomics’ can be installed ... ERROR
    ```
    Installation failed.
    See ‘/home/hb/repositories/R.utils/revdep/checks/psichomics/new/psichomics.Rcheck/00install.out’ for details.
    ```

## Newly fixed

*   checking examples ... ERROR
    ```
    ...
    +                                 840   NA i   female
    +                                  NA 1204 iv    male
    +                                  NA  383 iv  female
    +                                1293   NA iii   male
    +                                  NA 1355 ii    male")
    > names(clinical) <- c("patient.days_to_last_followup", 
    +                      "patient.days_to_death",
    +                      "patient.stage_event.pathologic_stage",
    +                      "patient.gender")
    > timeStart  <- "days_to_death"
    > event      <- "days_to_death"
    > formulaStr <- "patient.stage_event.pathologic_stage + patient.gender"
    > survTerms  <- processSurvTerms(clinical, censoring="right", event, timeStart,
    +                                formulaStr=formulaStr)
    > require("survival")
    Loading required package: survival
    > survfit(survTerms)
    Error in UseMethod("survfit", formula) : 
      no applicable method for 'survfit' applied to an object of class "c('survTerms', 'list')"
    Calls: survfit
    Execution halted
    ```

*   checking installed package size ... NOTE
    ```
      installed size is  8.1Mb
      sub-directories of 1Mb or more:
        doc   5.1Mb
    ```

## Installation

### Devel

```
* installing *source* package ‘psichomics’ ...
** libs
g++  -I"/usr/share/R/include" -DNDEBUG  -I"/home/hb/repositories/R.utils/revdep/library/psichomics/Rcpp/include"    -fpic  -g -O2 -fdebug-prefix-map=/build/r-base-3U0YWo/r-base-3.5.3=. -fstack-protector-strong -Wformat -Werror=format-security -Wdate-time -D_FORTIFY_SOURCE=2 -g  -c RcppExports.cpp -o RcppExports.o
g++  -I"/usr/share/R/include" -DNDEBUG  -I"/home/hb/repositories/R.utils/revdep/library/psichomics/Rcpp/include"    -fpic  -g -O2 -fdebug-prefix-map=/build/r-base-3U0YWo/r-base-3.5.3=. -fstack-protector-strong -Wformat -Werror=format-security -Wdate-time -D_FORTIFY_SOURCE=2 -g  -c psiFastCalc.cpp -o psiFastCalc.o
g++ -shared -L/usr/lib/R/lib -Wl,-Bsymbolic-functions -Wl,-z,relro -o psichomics.so RcppExports.o psiFastCalc.o -L/usr/lib/R/lib -lR
installing to /home/hb/repositories/R.utils/revdep/checks/psichomics/new/psichomics.Rcheck/psichomics/libs
** R
** inst
** byte-compile and prepare package for lazy loading
Error : object ‘evalWithTimeout’ is not exported by 'namespace:R.utils'
ERROR: lazy loading failed for package ‘psichomics’
* removing ‘/home/hb/repositories/R.utils/revdep/checks/psichomics/new/psichomics.Rcheck/psichomics’

```
### CRAN

```
* installing *source* package ‘psichomics’ ...
** libs
g++  -I"/usr/share/R/include" -DNDEBUG  -I"/home/hb/repositories/R.utils/revdep/library/psichomics/Rcpp/include"    -fpic  -g -O2 -fdebug-prefix-map=/build/r-base-3U0YWo/r-base-3.5.3=. -fstack-protector-strong -Wformat -Werror=format-security -Wdate-time -D_FORTIFY_SOURCE=2 -g  -c RcppExports.cpp -o RcppExports.o
g++  -I"/usr/share/R/include" -DNDEBUG  -I"/home/hb/repositories/R.utils/revdep/library/psichomics/Rcpp/include"    -fpic  -g -O2 -fdebug-prefix-map=/build/r-base-3U0YWo/r-base-3.5.3=. -fstack-protector-strong -Wformat -Werror=format-security -Wdate-time -D_FORTIFY_SOURCE=2 -g  -c psiFastCalc.cpp -o psiFastCalc.o
g++ -shared -L/usr/lib/R/lib -Wl,-Bsymbolic-functions -Wl,-z,relro -o psichomics.so RcppExports.o psiFastCalc.o -L/usr/lib/R/lib -lR
installing to /home/hb/repositories/R.utils/revdep/checks/psichomics/old/psichomics.Rcheck/psichomics/libs
** R
** inst
** byte-compile and prepare package for lazy loading
Creating a generic function for ‘colSums’ from package ‘base’ in package ‘psichomics’
** help
*** installing help indices
** building package indices
** installing vignettes
** testing if installed package can be loaded
* DONE (psichomics)

```
# TCGAbiolinks

<details>

* Version: 2.10.5
* Source code: ???
* URL: https://github.com/BioinformaticsFMRP/TCGAbiolinks
* BugReports: https://github.com/BioinformaticsFMRP/TCGAbiolinks/issues
* Date/Publication: 2019-03-20
* Number of recursive dependencies: 246

Run `revdep_details(,"TCGAbiolinks")` for more info

</details>

## In both

*   R CMD check timed out
    

*   checking dependencies in R code ... WARNING
    ```
    '::' or ':::' import not declared from: ‘purrr’
    There are ::: calls to the package's namespace in its code. A package
      almost never needs to use ::: for its own objects:
      ‘move’
    ```

*   checking installed package size ... NOTE
    ```
      installed size is 98.6Mb
      sub-directories of 1Mb or more:
        R      1.6Mb
        data   3.5Mb
        doc   93.3Mb
    ```

*   checking R code for possible problems ... NOTE
    ```
    ...
      ‘c3net’
    TCGAanalyze_networkInference: no visible global function definition for
      ‘minet’
    TCGAquery_recount2: no visible binding for global variable ‘rse_gene’
    TCGAtumor_purity: no visible binding for global variable ‘Tumor.purity’
    TCGAvisualize_SurvivalCoxNET: no visible global function definition for
      ‘dNetInduce’
    TCGAvisualize_SurvivalCoxNET: no visible global function definition for
      ‘dNetPipeline’
    TCGAvisualize_SurvivalCoxNET: no visible global function definition for
      ‘dCommSignif’
    TCGAvisualize_SurvivalCoxNET: no visible global function definition for
      ‘visNet’
    TCGAvisualize_oncoprint: no visible binding for global variable ‘value’
    readExonQuantification: no visible binding for global variable ‘exon’
    readExonQuantification: no visible binding for global variable
      ‘coordinates’
    Undefined global functions or variables:
      Tumor.purity barcode c3net clinical coordinates dCommSignif
      dNetInduce dNetPipeline exon knnmi.cross limmacontrasts.fit
      limmamakeContrasts minet portions rse_gene value visNet
    ```

