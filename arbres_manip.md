---
title: "arbres_publics_manip"
author: "Isabel"
date: "01/10/2019"
output:
  html_document:
    keep_md:  true
  editor_options:
    chunk_output_type: console
---




Dans quel arrondissment de montréal y a-t-il le plus d'arbes ?
## Packages et importation des données


```r
library(tidyverse)
read_csv("arbres_publics.csv")
```

```
## # A tibble: 308,484 x 22
##    INV_TYPE EMP_NO ARROND ARROND_NOM Rue   COTE  No_civique Emplacement
##    <chr>     <dbl>  <dbl> <chr>      <lgl> <lgl> <lgl>      <chr>      
##  1 H             6      1 Ahuntsic … NA    NA    NA         Parterre G…
##  2 H             7      1 Ahuntsic … NA    NA    NA         Parterre G…
##  3 H             8      1 Ahuntsic … NA    NA    NA         Parterre G…
##  4 H             9      1 Ahuntsic … NA    NA    NA         Parterre G…
##  5 H            10      1 Ahuntsic … NA    NA    NA         Parterre G…
##  6 H            11      1 Ahuntsic … NA    NA    NA         Parterre G…
##  7 H            12      1 Ahuntsic … NA    NA    NA         Parterre G…
##  8 H            13      1 Ahuntsic … NA    NA    NA         Parterre G…
##  9 H            14      1 Ahuntsic … NA    NA    NA         Parterre G…
## 10 H            15      1 Ahuntsic … NA    NA    NA         Parterre G…
## # … with 308,474 more rows, and 14 more variables: Coord_X <dbl>,
## #   Coord_Y <dbl>, SIGLE <chr>, Essence_latin <chr>, Essence_fr <chr>,
## #   ESSENCE_ANG <chr>, DHP <dbl>, Date_releve <dttm>,
## #   Date_plantation <dttm>, LOCALISATION <lgl>, CODE_PARC <chr>,
## #   NOM_PARC <chr>, Longitude <dbl>, Latitude <dbl>
```

