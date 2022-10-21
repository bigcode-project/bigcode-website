---
title: "How we manage IP"
description: ""
lead: ""
date: 2020-11-16T13:59:39+01:00
lastmod: 2020-11-16T13:59:39+01:00
draft: false
images: []
menu:
  docs:
    parent: "about"
weight: 120
toc: true
---

We believe the soul of BigCode to be clear and transparent communication striving towards open collaboration. The project, therefore, runs under the following set of open and permissive licenses. 

**Code**. All inbound code contributions (e.g. for model training or dataset analysis) must be made under an [Apache 2.0 license](https://www.apache.org/licenses/LICENSE-2.0). All outbound code will be made available under the Apache 2.0 license. The Apache 2.0 license is the most commonly used open source license due to its permissive character and clarity regarding copyright and patents. 

**Documentation**. Documentation will be received and made available by the Project under the [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/). For the sake of clarity, “Documentation” means any material related to the project which is not: code, a machine learning model or related features, nor a dataset. For instance, “Documentation” can be -but not limited to- specifications; guidelines; blog posts; academic papers; etc.

**Machine Learning Models**. Any machine learning model and related features (e.g. checkpoints) resulting from the Project will be licensed under an [Open & Responsible AI License](https://www.licenses.ai/blog/2022/8/18/naming-convention-of-responsible-ai-licenses). OpenRAILs are licenses designed to permit free and open access, re-use, and downstream distribution of the Model and its derivatives while establishing a set of behavioral-use restrictions for which the model cannot be used, due to ethics-informed concerns and/or the technical limitations of the model as informed by its model card. 

**Datasets**. We value openness and transparency about the training data of LLMs and intend to release datasets whenever we have the rights to do so. We will also provide [data cards](https://arxiv.org/abs/2204.01075) for all datasets we release. We are aware of ongoing discussions around the data governance of LLMs and would like to research better processes for it. See, for example, below how we experiment with giving developers the possibility to have their data removed from The Stack.  

## Remove data from the Stack
As part of the BigCode project, we will release The Stack, a 3.1 TB dataset of permissively licensed source code in 30 programming languages. Although we have filtered the data for permissively licensed source code (i.e., with minimal restrictions on how the software can be copied, modified, and redistributed), we can imagine that some developers do not wish their code to be used for pre-training LLMs and, therefore, start experimenting with giving code creators the possibility to remove data from the dataset.  

We are still exploring how to implement processes for such removal requests. One open question is at which granularity level we can implement removal requests for individual contributors, i.e., whether we should remove the full repositories they have contributed to, the individual files, or the individual files they have "meaningfully" contributed to. For the time being, we ask developers to fill [**this form**](https://forms.gle/6o2A6h3YcAuGYxtm7) to better understand their needs and explore what is technically possible. 

## Contributions under a different license
We are flexible and understand that each individual contributor or contributing party might have its own interests besides the collective BigCode effort. In case you do not feel comfortable licensing some of your contributions to the project under the Apache 2.0, please get in touch with us. We will see how to work around and make everyone comfortable. Note that for contributions with a non-permissive license, our general policy is to put them in a separate Github repository living outside the BigCode organisation. 

<!-- ## No CLA or DCO
Unlike open-source projects such as [PyTorch](https://github.com/pytorch/pytorch/) and [TensorFlow](https://github.com/tensorflow/tensorflow), Big Code does not make use of a [Contributor License Agreement](https://www.apache.org/licenses/contributor-agreements.html) (CLA). We believe the main role of a CLA is to centralize the IP licensing management under a single legal entity. Since Big Code is not a legal entity, we do not use a CLA. This means that if, for example, Big Code wants to change the license of the project, we will need to reach consensus among all contributors. We also opted not to use a [Developer Certificate of Origin](https://developercertificate.org/).     -->

If you have any further questions regarding IP, please reach out at contact@bigcode-project.org. 