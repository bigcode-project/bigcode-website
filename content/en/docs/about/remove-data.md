---
title: "Remove data from The Stack"
description: ""
lead: ""
date: 2020-10-06T08:49:31+00:00
lastmod: 2020-10-06T08:49:31+00:00
draft: false
images: []
menu:
  docs:
    parent: "about"
weight: 210
toc: true
---

As part of the BigCode project, we will release The Stack, a 3.1 TB dataset of permissively licensed source code in 30 programming languages. Although we have filtered the data for permissively licensed source code (i.e., with minimal restrictions on how the software can be copied, modified, and redistributed), we can imagine that some developers do not wish their code to be used for pre-training LLMs and, therefore, start experimenting with giving code creators the possibility to remove data from the dataset.  

We are still exploring how to implement processes for such removal requests. One open question is at which granularity level we can implement removal requests for individual contributors, i.e., whether we should remove the full repositories they have contributed to, the individual files, or the individual files they have "meaningfully" contributed to. For the time being, we ask developers to fill [this form](https://forms.gle/6o2A6h3YcAuGYxtm7) to better understand their needs and explore what is technically possible. 



