# Prosocial Conversations for Bridging Benchmark Dataset
This repository currently contains 11,973 comments that have been annotated for attributes that correlate with prosocial or constructive outcomes in online conversation. These attributes are: Reasoning, Curiosity, Respect, Compassion, Alienation, and Moral Outrage

This work is a collaboration among:
* Ruta Wheelock and Scott Friedman at [SIFT](https://www.sift.net/), a research and development consulting company that uses NLP and other technologies to make the information flow between humans and technology better for both sides, 
* Sonja Schmer- Galunder, Glenn and Deborah Renwick Leadership Professor in AI and Ethics at the [University of Florida](https://www.cise.ufl.edu/sonja-schmer-galunder/), and
* Zaria Jalan, Alyssa Chvasta, and Emily Saltz as part of the [Conversation AI](https://conversationai.github.io/)
project, a collaborative research effort at [Jigsaw](https://jigsaw.google.com) exploring ML as a tool for better discussions online, and

## Background

Current annotation practices pose many issues, ranging from Western-centric bias, poor working conditions, risks from exploitative power imbalance, and diverse representation among annotators. Within the machine learning community, a focus on data-hungry models and optimization for interrater reliability has led to a focus on data quantity over data quality. However, the process of data-labeling, especially when labeling more complex linguistic constructs like moral justifications of harms, intentionality or constructive conversations, is a highly qualitative task of induction and meaning, often requiring social and cultural knowledge of the context it is embedded in. Definitions for constructs that are theory-driven, albeit well informed in an academic sense, often clash with the intuitive understanding an annotator may have.

In a forthcoming paper, we will describe the results of our annotation work to address some of the problems mentioned above, describing qualitative and quantitative methods for increasing interrater reliability while improving conceptual understanding as well as taking the situatedness of annotation workers and their working conditions into consideration. We publish here the resulting benchmark dataset for assessing constructive conversations.

# Methods

## Curation and labeling

The dataset is composed of 11,973 comments from [Civil Comments](https://www.tensorflow.org/datasets/catalog/civil_comments), a publicly available dataset of comments from independent and international news sites that were created from 2015–2017. The data was labeled for six attributes: constructive, curiosity, respect, empathy, alienation, and moral outrage. Due to the low prevalence of these attributes, the data that was annotated was first scored by a proprietary model and then filtered by score to ensure a higher proportion of in-class comments. The data was sent to the 7 annotators in three batches which allowed for iterative data sampling improvements as time went on, and later batches of the data constrain the minimum and maximum text length and limit the amount of text dealing with Canadian politics by dropping the comments containing the terms “Trudeau” and “Canada”.  Additionally 698 examples were selected to include identity terms based on the Civil Comments identity labels.

## Definitions

| Label      | Definition |
| ----------- | ----------- |
| Reasoning      | Makes specific or well-reasoned points to provide a fuller understanding of the topic without disrespect or provocation.       |
| Curiosity   | Attempts to clarify or ask follow-up questions to better understand another person or topic.         |
| Respect   | Shows deference or appreciation to others, or acknowledges the validity of another person.        |
| Compassion   | Expressions of care and concern for others, understanding the feelings or viewpoint of others, including support or condolences.        |
| Alienation   | Portrays someone as inferior, implies a lack of belonging, or frames the statement in an us vs. them context.        |
| Moral outrage   | Anger, disgust, or frustration directed toward other people or entities who seem to violate the author’s ethical values or standards.        |

# Copyright and license

All data in this repository is made available under the Creative Commons Attribution
0 1.0 Universal license (CC0 1.0 DEED). A full copy of the license can be found
at https://creativecommons.org/publicdomain/zero/1.0/

# Bibliography

* [Bridging Systems: Open Problems for Countering Destructive Divisiveness across Ranking, Recommenders, and Governance](https://arxiv.org/abs/2301.09976)
* [Discussion Quality Diffuses in the Digital Public Square](https://arxiv.org/abs/1702.06677)
* [In conversation with Artificial Intelligence: aligning language models with human values](https://arxiv.org/abs/2209.00731)
* [Classifying Constructive Comments](https://arxiv.org/pdf/2004.05476.pdf)
* [Six Attributes of Unhealthy Conversations - ACL Anthology](https://aclanthology.org/2020.alw-1.15/#:~:text=Each%20comment%20is%20labelled%20as,%2For%20(6)%20an%20unfair)
* [Conversations Gone Alright: Quantifying and Predicting Prosocial Outcomes in Online Conversations](https://arxiv.org/abs/2102.08368)
* [Moral Conflict and Complexity: The Dynamics of Constructive Versus Destructive Discussions Over Polarizing Issues](https://www.researchgate.net/publication/228192389_Moral_Conflict_and_Complexity_The_Dynamics_of_Constructive_Versus_Destructive_Discussions_Over_Polarizing_Issues)
* [I Beg to Differ: A study of constructive disagreement in online conversations](https://arxiv.org/abs/2101.10917)
