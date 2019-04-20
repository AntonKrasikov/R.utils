# alphahull

<details>

* Version: 2.1
* Source code: https://github.com/cran/alphahull
* Date/Publication: 2016-02-15 13:47:04
* Number of recursive dependencies: 49

Run `revdep_details(,"alphahull")` for more info

</details>

## Newly broken

*   checking R code for possible problems ... NOTE
    ```
    areaahull: no visible global function definition for ‘evalWithTimeout’
    Undefined global functions or variables:
      evalWithTimeout
    ```

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
# R.cache

<details>

* Version: 0.13.0
* Source code: https://github.com/cran/R.cache
* URL: https://github.com/HenrikBengtsson/R.cache
* BugReports: https://github.com/HenrikBengtsson/R.cache/issues
* Date/Publication: 2018-01-04 16:55:43 UTC
* Number of recursive dependencies: 4

Run `revdep_details(,"R.cache")` for more info

</details>

## Newly broken

*   checking tests ...
    ```
     ERROR
    Running the tests in ‘tests/loadCache.R’ failed.
    Last 13 lines of output:
      + 
      +   data <- simulate(2.3, 3.0)
      +   data <- simulate(2.3, 3.5)
      +   data <- simulate(2.3, 3.0) # Will load cached data
      + 
      +   # Clean up
      +   file.remove(findCache(key=list(2.3,3.0)))
      +   file.remove(findCache(key=list(2.3,3.5)))
      + }
      Loaded cached data
      Generating data from scratch...ok
      Generating data from scratch...ok
      Error in file.remove(findCache(key = list(2.3, 3.5))) : 
        invalid first filename
      Execution halted
    ```

