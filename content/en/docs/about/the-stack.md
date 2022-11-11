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

As part of the BigCode project, we released and will maintain [The Stack](https://huggingface.co/datasets/bigcode/the-stack), a 3.1 TB dataset of permissively licensed source code in 30 programming languages. One of our goals in this project is to give the people agency over their source code by letting them decide whether or not it should be used to develop and evaluate LLMs, as we acknowledge that not all developers may wish to have their data used for that purpose.

Our first step to that end was to select code whose original license was compatible with training an LLM, specifically, open-source licenses without copyleft. You can find the list of [selected open-source licenses below]({{< relref "#licenses" >}}). In addition, we are giving developers the ability to have their code removed from the dataset upon request. The process for submitting and enacting removal requests will keep evolving throughout the project as we receive feedback and build up more data governance tools. The following FAQ presents the current state of this process, as well as the planned next steps. 

### How do I know if my data is in The Stack?
We have a developed a tool to help users understand whether their data is in The Stack. Check out [Am I in The Stack?](https://huggingface.co/spaces/bigcode/in-the-stack). 

### How can I request that my data be removed from The Stack?
In order to request that data from your repositories be removed from The Stack, we ask that you first fill out the [following form](https://forms.gle/6o2A6h3YcAuGYxtm7) with your GitHub username and the email address associated with your git activity. After submitting the form, we will invite you to a private repository on the BigCode organization and ask you to open an issue with the topic “remove my Github repositories from The Stack”. This will verify your Github username and we will mark all public repositories under your username for removal in the next dataset release cycle. The verification process is manual at the moment but we are looking into ways to fully automate it. 

The form also has a field for general feedback and motivation for requesting the removal; it is not required for the request, but we would be very grateful for any additional information to help inform future data policies.

### What data can I request be removed from The Stack?
Currently, you can request that we remove all public repositories under the provided username. In the coming months, we will be working on expanding the scope of data removal requests to address requests at a finer granularity (specific repositories, specific files) and to a greater range of contribution types (for example, based on whether a file or repository contains push events associated with your username according to [https://www.gharchive.org/](https://www.gharchive.org/)).

### Can I also prevent my data from being included in future versions of The Stack?
The removal request form will be used to validate removal requests and remove appropriate data. Validated requests and associated code pointers will also be stored in order to ensure that the code does not appear in future versions of The Stack.

### What happens to my data once I’ve requested its removal?
For as long as we are maintaining The Stack dataset, we will provide regular updates to the dataset to remove data that has been flagged since the last version. The current plan is to update the dataset every 3 months, although the schedule may change based on the volume of requests received. If we are not in a position to continue maintaining the dataset, we plan to stop distributing it in its current format and update its terms of use to limit its range of applications further, including for training new LLMs. Finally, we [require](https://huggingface.co/datasets/bigcode/the-stack#terms-of-use-for-the-stack) that people who download the dataset agree to use the most recent allowed version in order to incorporate the removal requests. 

### What is the license for The Stack dataset? {#licenses}
The Stack is a collection of source code from repositories with various licenses. Any use of code gathered in The Stack must abide by the code’s original license terms, including attribution clauses when relevant. To facilitate this, The Stack contains provenance information, including the source of the code and its license, for each data point.

The Stack was filtered to include only permissive licenses—i.e., those with minimal restrictions on how the software can be copied, modified, and redistributed e.g., MIT and Apache 2.0. Copyleft licenses such as GPL are not included as they have the requirement that the same rights be preserved in derivative works. [Some have argued](https://sfconservancy.org/blog/2022/feb/03/github-copilot-copyleft-gpl/) that a model trained with copyleft licensed data is considered derivative work.

The list of [SPDX license identifiers](https://spdx.org/licenses/) included in dataset are:
- MIT-0
- MIT
- MIT-feh
- Apache-2.0
- BSD-3-Clause
- BSD-3-Clause-Clear
- BSD-3-Clause-No-Nuclear-License-2014
- BSD-2-Clause
- CC0-1.0
- EPL-1.0
- MPL-2.0
- Unlicense
- ISC
- Artistic-2.0
- deprecated\_LGPL-3.0+
- deprecated\_LGPL-2.1+
- ECL-2.0
- SHL-0.51
- MPL-2.0-no-copyleft-exception

You can find the license distribution in [Table 2 of the supporting research paper](https://drive.google.com/file/d/17J-0KXTDzY9Esp-JqXYHIcy--i_7G5Bb/view). MIT and Apache 2.0 make up the majority of the released dataset. 

**IMPORTANT UPDATE 27/10** It was recently brought to our attention that licenses such as MPL, LGPL, and EPL were erroneously labeled as permissive when they are in fact [weak copyleft licenses](https://blueoakcouncil.org/copyleft). We will remove these weak copyleft license files from The Stack and release an updated version in the coming weeks. The weak copyleft-licensed data is only a small part of the overall dataset (below 0.5% of the Python subset), hence we expect the experimental findings of [the paper](https://drive.google.com/file/d/17J-0KXTDzY9Esp-JqXYHIcy--i_7G5Bb/view) to remain unchanged.
