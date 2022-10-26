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

The Stack contains over 3TB of permissively-licensed source code files covering 30 programming languages crawled from GitHub. The dataset was created as part of the BigCode Project, an open scientific collaboration working on the responsible development of Large Language Models for code (code LLMs). The Stack serves as a pre-training dataset for creating code LLMs, i.e., code-generating AI systems which enable the completion and synthesis of code, both from other code as well as from natural language descriptions. See the [supporting datacard](https://huggingface.co/datasets/bigcode/the-stack) for more information. 

## Infographic



## Remove data from The Stack
We can imagine that some developers do not wish their code to be used for pre-training LLMs and, therefore, give developers the possibility to have their data removed from the dataset.  

We are still experimenting how to process such removal requests. We currently ask users to provide their Github username, and subsequently remove the following data:
* All repositories under the provided Github account
* 
  
We ask developers to fill [**this form**](https://forms.gle/6o2A6h3YcAuGYxtm7). By adding your user details in this form we will also exclude the associated code in future releases of The Stack. 

## FAQ

