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

As part of the BigCode project, we are releasing and maintaining The Stack, a 3.1 TB dataset of permissively licensed source code in 30 programming languages. One of our goals in this project is to give the people who wrote this source code a choice as to whether or not it should be used to develop and evaluate LLMs, as we acknowledge that not all developers may wish to have their data used for that purpose.

Our first step to that end was to select code whose original license was compatible with training an LLM, specifically, open-source licenses without copyleft (the full list can be found in Appendix A of [the paper](TODO)). In addition, we are giving developers the ability to have their code removed from the dataset upon request. The process for submitting and enacting removal requests will keep evolving throughout the project as we receive feedback and build up more data governance tools. The following FAQ presents the current state of this process, as well as the planned next steps.

### How do I know if my data is in The Stack?
We are working on developing tools to help users visualize the status of their data in The Stack, including checking whether specific data is present in the latest version and whether it is already flagged for removal.

### How can I request that my data be removed from The Stack?
In order to request that data from your repositories be removed from The Stack, we ask that you first fill out the [following form](https://forms.gle/6o2A6h3YcAuGYxtm7) with your GitHub username and the email address associated with your git activity. We will then get back to you with simple follow-up instructions to verify your GitHub account. The form also has a field for general feedback and motivation for requesting the removal; it is not required for the request, but we would be very grateful for any additional information to help inform future data policies.

### What data can I request be removed from The Stack?
Currently, you can request that we remove any repository for which you have an Admin or Maintain role. In the coming months, we will be working on expanding the scope of data removal requests to address requests at a finer granularity (specific repositories, specific files) and to a greater range of contribution types (for example, based on whether a file or repository contains push events associated with your username according to https://www.gharchive.org/).

### Can I also prevent my data from being included in future versions of The Stack?
The removal request form will be used to validate removal requests and remove appropriate data. Validated requests and associated code pointers will also be stored in order to ensure that the code does not appear in future versions of The Stack.

### What happens to my data once I’ve requested its removal?
For as long as we are maintaining The Stack dataset, we will provide regular updates to the dataset to remove data that has been flagged since the last version. The current plan is to update the dataset every 3 months, although the schedule may change based on the volume of requests received. If we are not in a position to continue maintaining the dataset in the future, we plan to stop distributing it in its current format and update its terms of use to limit its range of applications further, including for training new LLMs. Finally, we [require](TODO) that people who download the dataset agree to use the most recent allowed version in order to incorporate the removal requests. 

### What is the license for The Stack dataset?
The Stack is a collection of source code from repositories with various licenses. Any use of code gathered in The Stack must abide by the code’s original license terms, including attribution clauses when relevant. To facilitate this, The Stack contains provenance information, including the source of the code and its license, for each data point.


