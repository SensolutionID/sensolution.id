+++
title = "Analisis Sensoris Menggunakan R (Bagian 1)"
date = "2018-09-19T11:36:00+07:00"
tags = ["sensoris", "analisis", "metode", "R"]
categories = ["tutorial"]
banner = "img/banners/work.jpeg"
+++

Halo dan salam kenal!

Tulisan perdana ini merupakan bagian awal dari seri 'Analisis Sensoris menggunakan R' yang akan rutin disajikan dalam situs [Sensolution.ID](https://sensolution.id). Seri tulisan ini akan membahas bagaimana cara menggunakan R untuk analisis sensoris tahap demi tahap dan disertai dengan contoh studi kasus. Oleh karena itu, sebagai permulaan kami akan memperkenalkan R secara singkat dan alasan penggunaannya untuk analisis sensoris kepada Anda.

## Apa itu R?
R merupakan bahasa pemrograman yang ditujukan khusus untuk statistik dan tersedia sebagai perangkat lunak bebas. R dapat dipasang dalam berbagai sistem operasi komputer, yaitu GNU/Linux, Windows, dan OS X. Anda dapat mengunduh R pada laman [ini](https://cran.r-project.org). Setelah dipasang di komputer, R dapat dijalankan melalui *terminal* atau *command line* (pada Windows juga dapat dijalankan melalui R GUI). Namun, kami merekomendasikan Anda untuk berinteraksi dengan R menggunakan IDE RStudio yang dapat diunduh melalui laman [ini](https://rstudio.com). Sama seperti R, RStudio juga dapat dipasang pada sistem operasi GNU/Linux, Windows, dan OS X.

## Mengapa R?
Seperti disinggung pada bagian sebelumnya, R dirancang khusus untuk tujuan analisis statistik. Oleh karena itu, R sangat cocok digunakan untuk bidang ilmu sensoris yang notabene berkaitan erat dengan analisis statistik. Fitur-fitur dasar bawaan R sangat mumpuni digunakan untuk mengolah dan menganalisa data sensoris. Selain itu, R dilengkapi dengan paket *library* tambahan yang sangat komprehensif dan tidak jarang dirancang untuk disiplin ilmu tertentu. Termasuk untuk disiplin ilmu sensoris, terdapat beberapa paket yang sangat bermanfaat dan diantaranya dirancang khusus untuk analisis sensoris. Berikut adalah nama-nama paket di R beserta kegunaannya dalam disiplin ilmu sensoris:

* `crossdes`
* `sensR`
* `FactoMineR`
* `SensoMineR`


### Cara memasang paket di R

Berikut merupakan cara untuk memasang paket-paket yang telah disebutkan sebelumnya pada R.
```r
install.packages("crossdes")
install.packages("sensR")
install.packages("FactoMineR")
install.packages("SensoMineR")
```

atau

```r
install.packages(c("crossdes", "sensR", "FactoMineR", "SensoMineR"))
```
