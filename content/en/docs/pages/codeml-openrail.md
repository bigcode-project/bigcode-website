---
title: "CodeML OpenRAIL-M 0.1 - FAQ"
description: ""
lead: ""
date: 2020-11-12T15:22:20+01:00
lastmod: 2020-11-12T15:22:20+01:00
draft: false
images: []
menu: 
  docs:
    parent: "pages"
weight: 620
toc: true
---

We are releasing the first set of BigCode models, which are going to be licensed under the CodeML OpenRAIL-M 0.1 license, as we initially stated here and in our membership form. The CodeML OpenRAIL-M 0.1 is an interim version of the license that is being drafted for the release of BigCode in March 2023. This license is an open and responsible AI license (OpenRAIL). 

## What is an OpenRAIL license?
Open Responsible AI Licenses (OpenRAIL) are licenses designed to permit free and open access, re-use, and downstream distribution of derivatives of AI artifacts, for research, commercial or non-commercial purposes, as long as the use restrictions present in the license always apply (including to derivative works). For more information, please access the RAIL Initiative post.

## Why Open?
The term “Open” is to indicate that the license enables royalty free access, downstream use and re-distribution of the licensed material, and distribution of any derivatives of it.

To be clearer, you can use any type of license or legal agreement you want to re-distribute the model or derivatives of it. This will be possible under the sole conditions of:
Embedding the license clauses related to the responsible use of the model 
And, that your legal agreement is consistent with the license clauses (i.e. Section 5, Attachment A).

See FAQ below: “Can you give me an example?”.

## Responsible?
Responsible AI licensing is a mechanism that is part of -and interacting with- a broader system of AI governance instruments and processes, such as Model Cards and regulations.

OpenRAIL licenses are designed to promote responsible downstream use and distribution of the model by including a set of use restrictions for which the model cannot be used. In the case of the CodeML OpenRAIL-M, the restrictions are mainly inspired by BigScience’s approach to the licensing of LLMs, and also include specific use cases where we believe code generation models could be used as a harmful instrument due to either the intent of the user or the technical limitations of the model.

## What does the “M” stand for?
“M” stands for “Model”, which is the artifact being licensed under this license and subject to use restrictions. See the naming conventions for RAIL Licenses post.

## Is this an Open Source license?
This is not an open source license according to the Open Source Initiative definition, because it has some restrictions on the use of the model. That said, it does not impose any restrictions on reuse, distribution, commercialization, or adaptation as long as the model is not being applied to use cases that have been restricted.

## What are we licensing?
We are licensing ML models developed under the BigCode project. Any source code relevant to the BigCode ML models is licensed under the Apache 2.0 license.

## Why should BigCode decide what is appropriate or not regarding the use of the model?
As creators of the models, we think about how our work could be used. We believe we should do as much as we can to prevent possible harms from our work while releasing it on an open basis, especially if there are possible use cases that are incompatible or inappropriate with the model performance and/or capabilities of it.

## Do use restrictions apply to Derivatives of the Model? 
Yes. The use restrictions in the RAIL licenses have been designed to be applicable in downstream licensing terms of any derivative versions of any of the BigCode models offered and/or released by a downstream user. The distribution and use of any Derivatives of the Model (as defined in the license) should be governed by -at minimum- the same use restrictions.

## Can you give me an example? 
Imagine a company that wants to use a BigCode model in order to develop a version of a coding assistant. The company accesses the model, modifies it, and finetunes it to be the technical backbone of the coding assistant app. Firstly, these actions will be governed by the RAIL license. Secondly, and worth noting, according to the terms defined in our RAIL License, this coding assistant app is considered a Derivative of the Model. Thus, the use of the app will be governed by the use restrictions defined in the RAIL license, and accordingly, when commercializing the new version of the Model by means of a commercial license (or any other type of legal agreement), the latter will have to integrate these use restrictions as part of the subsequent license and/or Terms of Use of the specific API-based coding assistant app.

## Does the license cover every harmful use case? 
No. We recognize that the list of use restrictions does not conceivably represent “everything” one could possibly do with our work. We focus on use cases that can be a source of concern.

## Is it possible for the licensor to remotely restrict the use of the models? If so, what does it mean? 
The models itself has no built-in mechanism for it to be restricted. However, if the model is hosted via an API, restricting access remotely can be possible as the API access key can be revoked.

## Do I have to disclaim that the outputed code snippets were generated by a model?
According to restriction (f) you cannot use the model to generate code or distribute code without intelligibly disclaiming that the code was generated by the model. What does this mean in practice? If you finetune a BigCode model, embed it into an app designed to be a code assistant, and plan to distribute the app as a SaaS, you should make it clear for users of your app that the code generated by it is generated by a model. It might sound obvious for you, but not for others, it is important to be transparent with your users. 

## What has been modified from the BigScience OpenRAIL-M license?
There are 4 modifications:

The Preamble has been adapted to code generation models.
- Complementary material (source code) is not licensed under this license but separately under an Apache 2.0 license.
- Clause 7 of the license no longer requires users to undertake reasonable efforts to use the last updated version of the Model, as is the case in the BigScience OpenRAIL-M license. 
- Attachment A includes a new restriction:
  Restriction (c) forbidding the use of the Model to generate and/or disseminate malware. We understand that “malware”, according to the NIST definition, already includes the intent of harm. For example, using a dataset composed of  source code, signature, or Indicators of Compromise (IOC) that are known to be malicious and finetune a BigCode model with it in order to enable the automated generation and/or distribution of malware or related code.

## What if I do not understand some of the restrictions in Attachment A of the license?
Community feedback is essential for us, we are grateful to receive it and answer any questions related to the license. Drafting use restrictions that everyone agrees on and understands for ML models is a challenge. There is a balance to be struck between restrictions being too generic, on the one hand, and restrictions being too narrow and not covering potentially harmful scenarios, on the other hand. We are open to your comments.

## What other RAILs are out there?
Since the release of the BLOOM RAIL license in May 2022, there has been a proliferation of RAILs based on either the structure and content of the latter or just the aim of promoting responsible use of ML models, as Meta does with its licenses for OPT-175, BB3, SEER. Other RAIL licenses based on the BLOOM RAIL have been released, such as BigScience OpenRAIL-M, CreativeML OpenRAIL-M, SIL RAIL-M 1.0, and OpenRAIL++M. 

## Is there more information?
Yes! Please have a look at the RAIL Initiative FAQ.

## What if the model outputs code snippets belonging to an already existing repository under a permissive license? What about providing attribution and license notice?

Besides the opt out tool and process we developed for the community (“Am I in the Stack?”), we are currently working on tools enabling users to identify whether the code generated by the model belongs to a code repository, in order for the user to be able to inspect licensing requirements and comply with them when using and distributing the code.


