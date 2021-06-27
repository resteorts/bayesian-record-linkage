# Some of Bayesian Entity Resolution

## Speakers

Rebecca C. Steorts, Assistant Professor, Duke University 
https://resteorts.github.io/

## Contributors

Brenda Betancourt, Assistant Professor, University of Florida
(Former Foerster-Bernstein Postdoctoral Fellow, Duke University)
https://www.brendabc.net/

Andee Kaplan, Assistant Professor, Colorado State University 
(Former Postdoctoral Scholar, Duke University)
http://andeekaplan.com/

Neil Marchant, Postdoctoral Fellow, University of Melbourne 
https://github.com/ngmarchant

Olivier Binette, PhD Student, Duke University

Brian Kundinger, PhD Student, Duke University 



## Abstract

Very often information about social entities is scattered across multiple databases.  Combining that information into one database can result in enormous benefits for analysis, resulting in richer and more reliable conclusions.  Among the types of questions that have been, and can be, addressed by combining information include: How accurate are census enumerations for minority groups? How many of the elderly are at high risk for sepsis in different parts of the country? How many people were victims of war crimes in recent conflicts in Syria? In most practical applications, however, analysts cannot simply link records across databases based on unique identifiers, such as social security numbers, either because they are not a part of some databases or are not available due to privacy concerns.  In such cases, analysts need to use methods from statistical and computational science known as entity resolution (record linkage or de-duplication) to proceed with analysis.  Entity resolution is not only a crucial task for social science and industrial applications, but is a challenging statistical and computational problem itself. In this short course, we first provide an overview and introduction to graphical Bayesian entity resolution. Second, we provide a deep dive into commonly used methods in the literature and evaluation metrics. Third, we propose a joint blocking and entity resolution approach for Bayesian resolution (dblink) that scales to millions of records, demonstrating its success on both synthetic and real applications. Finally, we provide a live demo of the dblink approach and answer questions from the audience regarding the field in general. 

### I. An Overview of Entity Resolution

Speaker: Rebecca C. Steorts

Very often information about social entities is scattered across multiple databases.  Combining that information into one database can result in enormous benefits for analysis, resulting in richer and more reliable conclusions.  Among the types of questions that have been, and can be, addressed by combining information include: How accurate are census enumerations? How many people were victims of war crimes in human rights conflicts? In most practical applications, however, analysts cannot simply link records across databases based on unique identifiers, such as social security numbers, either because they are not a part of some databases or are not available due to privacy concerns.  In such cases, analysts need to use methods from statistical and computational science known as entity resolution (record linkage or de-duplication) to proceed with analysis.  Entity resolution is not only a crucial task for social science and industrial applications, but is a challenging statistical and computational problem itself. In this talk, I provide an overview and introduction to entity resolution. I discuss collaborations throughout my career to date, highlighting case studies, and impactful insights. 

Slide Deck: https://github.com/resteorts/bayesian-record-linkage/blob/main/01-overview-er/01-overview-er.pdf

### II. A Deep Dive Into Entity Resolution 

Speaker: Rebecca C. Steorts

In this part of the workshop, I will review the terminology used in entity resolution. In addition, I will describe computational speeds ups used that are known as blocking. Next, I will review the most commonly used entity resolution methods in the literature. I will review evaluation metrics that are used. Finally, I will present a small example to illustrate how such evaluation metrics are used in practice and comparisons can be made to existing methods in the literature. 

Slide Deck: 


### III. End to End Entity Resolution

Speaker: Rebecca C. Steorts

While there have been many Bayesian record linkage methods proposed in the literature, none of these methods scale to industrial sized data sets. In fact, none of these methods scale to data sets beyond 10,000 records using a joint model to our knowledge. In this section of the workshop, I introduce distributed methods for Bayesian entity resolution (dblink). More specifically, we give an overview of a recent method of Marchant, et. al (2021), which proposes the first scalable and distributed end-to-end Bayesian model for entity resolution, which propagates uncertainty in blocking, matching, and merging. In addition, several contributions are made including: (i) incorporating probabilistic blocking directly into the model through auxiliary partitions; (ii) support for missing values; (iii) a partially-collapsed Gibbs samper; and (iv) a novel perturbation sampling algorithm  that enables fast updates of the entity attributes. In this workshop, we will present dblink in a more simple setting for intuition, and provide intuition for computational speed ups. Finally, I illustrate experimental results on dblink, which show that d-blink can achieve significant efficiency gains—in excess of 200×—when compared to existing methodology. 

Slide Deck: 


### IV. Demo and Questions

Speaker: Rebecca C. Steorts

In this part of the workshop, I will provide a demo of dblink. 

Steorts has been funded by an NSF CAREER Award and a Sloan Research Award. The ideas of this tutorial are of the researchers and not of the funding organization. 
