+++
title = "Analisis Sensoris Menggunakan R (Bagian 1)"
date = "2018-09-19T11:36:00+07:00"
tags = ["sensoris", "analisis", "metode", "R"]
categories = ["tutorial"]
banner = "img/banners/work.jpeg"
+++

**Halo dan salam kenal!**

Tulisan perdana ini merupakan bagian awal dari seri 'Analisis Sensoris menggunakan R' yang akan rutin disajikan dalam situs [Sensolution.ID](https://sensolution.id). Seri tulisan ini akan membahas bagaimana cara menggunakan R untuk analisis sensoris tahap demi tahap dan disertai dengan contoh studi kasus. Oleh karena itu, sebagai permulaan kami akan memperkenalkan R secara singkat dan alasan penggunaannya untuk analisis sensoris kepada Anda.

## Apa itu R?
R merupakan bahasa pemrograman yang ditujukan khusus untuk statistik dan tersedia sebagai perangkat lunak bebas. R dapat dipasang dalam berbagai sistem operasi komputer, yaitu GNU/Linux, Windows, dan OS X. Anda dapat mengunduh R pada laman [ini](https://cran.r-project.org). Setelah dipasang di komputer, R dapat dijalankan melalui *terminal* atau *command line* (pada Windows juga dapat dijalankan melalui R GUI). Namun, kami merekomendasikan Anda untuk berinteraksi dengan R menggunakan IDE RStudio yang dapat diunduh melalui laman [ini](https://rstudio.com). Sama seperti R, RStudio juga dapat dipasang pada sistem operasi GNU/Linux, Windows, dan OS X.

![Tampilan RStudio](/img/blog/rstudio.png)

## Mengapa R?
Seperti disinggung pada bagian sebelumnya, R dirancang khusus untuk tujuan analisis statistik. Oleh karena itu, R sangat cocok digunakan untuk bidang ilmu sensoris yang notabene berkaitan erat dengan analisis statistik. Fitur-fitur dasar bawaan R sangat mumpuni digunakan untuk mengolah dan menganalisa data sensoris. Selain itu, R dilengkapi dengan paket *library* tambahan yang sangat komprehensif dan tidak jarang dirancang untuk disiplin ilmu tertentu. Termasuk untuk disiplin ilmu sensoris, terdapat beberapa paket yang sangat bermanfaat dan diantaranya dirancang khusus untuk analisis sensoris. Berikut adalah nama-nama paket di R beserta deskripsi resminya:

* `crossdes`

> *The crossdes package provides functions for the construction of of carryover balanced crossover designs. In addition contains functions to check given designs for balance.*

* `BradleyTerry2`

> *Specify and fit the Bradley-Terry model, including structured versions in which the parameters are related to explanatory variables through a linear predictor and versions with contest-specific effects, such as a home advantage.*

* `sensR`

> *Provides methods for sensory discrimination methods; duotrio, tetrad, triangle, 2-AFC, 3-AFC, A-not A, same-different, 2-AC and degree-of-difference. This enables the calculation of d-primes, standard errors of d-primes, sample size and power computations, and comparisons of different d-primes. Methods for profile likelihood confidence intervals and plotting are included.*

* `FactoMineR`

> *Exploratory data analysis methods to summarize, visualize and describe datasets. The main principal component methods are available, those with the largest potential in terms of applications: principal component analysis (PCA) when variables are quantitative, correspondence analysis (CA) and multiple correspondence analysis (MCA) when variables are categorical, Multiple Factor Analysis when variables are structured in groups, etc. and hierarchical cluster analysis.*

* `SensoMineR`

> *Statistical Methods to Analyse Sensory Data. SensoMineR: A package for sensory data analysis.*

Dalam konteks ilmu sensoris, paket `crossdes` bermanfaat dalam perancangan desain penelitian berdasarkan *William's Latin Square Design* untuk mengindari *carry-over effect*. Paket `BradleyTerry2` digunakan untuk analisis model Bradley-Terry dalam uji *multiple paired-preference*. Paket `sensR` bermanfaat untuk analisis uji pembeda/diskriminasi seperti uji segitiga, uji duo-trio, 2AFC, 3AFC, dan sebagainya. Paket `FactoMineR` untuk analisis multivariat dalam uji deksriptif. Serta paket `SensoMineR` untuk analisis metode sensoris mutakhir seperti *Free-Choice Profiling*, *Flash Profile*, *Sorting*, *Napping*, *Ideal Profile Method*, dan sebagainya.

### Cara memasang dan mengaktifkan paket di R

Sebelum dapat digunakan, paket-paket tersebut harus dipasang terlebih dulu pada R. Berikut merupakan cara untuk memasang paket-paket yang telah disebutkan sebelumnya pada R.

```r
install.packages("crossdes")
install.packages("BradleyTerry2")
install.packages("sensR")
install.packages("FactoMineR")
install.packages("SensoMineR")
```

atau

```r
install.packages(c("crossdes", "BradleyTerry2", "sensR", "FactoMineR", "SensoMineR"))
```

Setelah terpasang, paket-paket tersebut harus diaktifkan terlebih dahulu sebelum dapat digunakan. Adapun cara mengaktifkan paket-paket tersebut adalah sebagai berikut:

```r
library(crossdes)
library(BradleyTerry2)
library(sensR)
library(FactoMineR)
library(SensoMineR)
```

## Penutup
Sekian tulisan awal dalam seri 'Analisis Sensoris menggunakan R' ini. Pada tulisan selanjutnya akan dibahas cara menganalisa data sensoris menggunakan R dengan mudah. Nantikan tulisan kami selanjutnya!
