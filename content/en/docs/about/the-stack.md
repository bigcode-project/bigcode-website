---
title: "The Stack"
description: ""
lead: ""
date: 2020-11-16T13:59:39+01:00
lastmod: 2020-11-16T13:59:39+01:00
draft: false
images: []
menu:
  docs:
    parent: "about"
weight: 210
toc: true
---

## Remove data from The Stack
As part of the BigCode project, we released The Stack, a 3.1 TB dataset of permissively licensed source code in 30 programming languages. Although we have filtered the data for permissively licensed source code (i.e., with minimal restrictions on how the software can be copied, modified, and redistributed), we can imagine that some developers do not wish their code to be used for pre-training LLMs and, therefore, give developers the possibility to have their data removed from the dataset.  

We are still experimenting how to process such removal requests. We currently ask users to provide their Github username and email address associated with git commits, and subsequently remove the following data:
* All repositories under the provided Github account
* Public repositories that the provided email-address or Github account pushed to. We remove all files that were affected by the commits of the push events.  Note that we rely on GHArchive for such push events and we can not garantuee that these event archives are complete. 
  
We ask developers to fill [**this form**](https://forms.gle/6o2A6h3YcAuGYxtm7) before January 1st, 2023 so that we have time to process the deletion requests. By adding your user details in this form we will also exclude the associated code in future releases of The Stack. 
