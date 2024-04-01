---
title: "Datasets"
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

As part of the BigCode project, we released and will maintain [The Stack](https://huggingface.co/datasets/bigcode/the-stack), a 6.4 TB dataset of permissively licensed source code in 358 programming languages, along with a collection of datasets created through the course of research during the project. 

| Release    | Description                    |
| ---------- | ------------------------------ |
| v1.0       | Initial release of the Stack. Included 30 programming languages and 18 permissive licenses. Note: Three included licenses (MPL/EPL/LGPL) are considered weak copyleft licenses. The resulting near-deduplicated dataset is 3TB in size.    |
| v1.1       |  The three copyleft licenses (MPL/EPL/LGPL) were excluded and the list of permissive licenses extended to 193 licenses in total. The list of programming languages was increased from 30 to 358 languages. Also opt-out request submitted by 15.11.2022 were excluded from this version of the dataset. The resulting near-deduplicated dataset is 6TB in size.     |
| v1.2       | Opt-out request submitted by 09.02.2023 were excluded from this version of the dataset as well as initially flagged malicious files (not exhaustive). |

## Datasets and data governance tools released by BigCode
- [The Stack](https://huggingface.co/datasets/bigcode/the-stack): Exact deduplicated version of The Stack. 
- [The Stack dedup](https://huggingface.co/datasets/bigcode/the-stack-dedup): Near deduplicated version of The Stack (recommended for training). 
- [The Stack issues](https://huggingface.co/datasets/bigcode/the-stack-github-issues): Collection of GitHub issues. 
- [The Stack Metadata](https://huggingface.co/datasets/bigcode/the-stack-metadata): Metadata of the repositories in The Stack. 
- [Am I in the Stack](https://huggingface.co/spaces/bigcode/in-the-stack): Check if your data is in The Stack and request opt-out. 

One of our goals in this project is to give people agency over their source code by letting them decide whether or not it should be used to develop and evaluate LLMs, as we acknowledge that not all developers may wish to have their data used for that purpose. 

Our first step to that end was to select source code with permissive licenses, i.e. those with minimal restrictions on how the software can be copied, modified and redistributed. You can find the list of selected open-source licenses below. In addition, we are giving developers the ability to have their code removed from the dataset upon request. The process for submitting and enacting removal requests will keep evolving throughout the project as we receive feedback and build up more data governance tools. The following FAQ presents the current state of this process, as well as the planned next steps. 

### How do I know if my data is in The Stack?
We have a developed a tool to help users understand whether their data is in The Stack. Check out [Am I in The Stack?](https://huggingface.co/spaces/bigcode/in-the-stack). 

### How can I request that my data be removed from The Stack?
You can opt-out your repositories from [The Stack dataset](https://huggingface.co/datasets/bigcode/the-stack) by creating an issue in our [GitHub opt-out repository](https://github.com/bigcode-project/opt-out-v2) and listing the repositories you would like to exclude. We will then exclude those repositories in the next iteration of The Stack.  To initiate this process, you should first check if any of your repositories are actually in The Stack using the [Am I in the Stack app](https://huggingface.co/spaces/bigcode/in-the-stack).  

If you decide that you wish to have repos owned by you removed from The Stack, please [create an issue](https://github.com/bigcode-project/opt-out-v2/issues/new?assignees=&labels=&template=opt-out-request.md&title=Opt-out+request+for+USERNAME) so that we can verify that you are in fact the owner of the repositories requested for opt-out. 

If you are experiencing difficulty with this process, please email contact@bigcode-project.org. 

### What data can I request be removed from The Stack?
You can choose to request either (1) all repos, or (2) you can specify select repos that you own to be removed. You can also specify Commits and GitHub Issues to be removed as part of your opt-out request. More details about this process on [GitHub](https://github.com/bigcode-project/opt-out-v2).

### Can I also prevent my data from being included in future versions of The Stack?
The [removal request](https://github.com/bigcode-project/opt-out-v2) process will be used to validate removal requests and for processing of removal requests to remove opt-out data. Validated requests and associated code pointers will also be stored in order to ensure that the code does not appear in future versions of The Stack.

### What happens to my data once I’ve requested its removal?
For as long as we are maintaining The Stack dataset, we will provide regular updates to the dataset to remove data that has been flagged since the last version. The current plan is to update the dataset every 3 months, although the schedule may change based on the volume of requests received. If we are not in a position to continue maintaining the dataset, we plan to stop distributing it in its current format and update its terms of use to limit its range of applications further, including for training new LLMs. Finally, we [require](https://huggingface.co/datasets/bigcode/the-stack#terms-of-use-for-the-stack) that people who download the dataset agree to use the most recent allowed version in order to incorporate the removal requests. 

### What is the license for The Stack dataset? {#licenses}
The Stack is a collection of source code from repositories with various licenses. Any use of code gathered in The Stack must abide by the code’s original license terms, including attribution clauses when relevant. We faciliate this by provenance information for each data point. 

The list of SPDX license identifiers included in the dataset can be found [here](https://huggingface.co/datasets/bigcode/the-stack/blob/main/licenses.json). 
