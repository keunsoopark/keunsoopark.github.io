---
layout: posts
title:  "How I earned Azure Data Engineer certification"
---

***This post is to suggest the efficient and practical way to prepare the exams for Azure Data Engineer certification based on my experience.***

Recently, I earn `Microsoft Certified: Azure Data Engineer Associate`:)  
Let me start the post with proving ~~showing off~~ my certification: 
![certificate](/assets/images/Azure-DE-KeunsooPark.png)  
[see credential](https://www.youracclaim.com/badges/f23898af-e81d-4749-9113-3d720a585716/linked_in_profile)  


## Keep yourself updated on the certification

This blog post is written based on the Microsoft's update on the exam at February 2020.  
I strongly recommend you to go their [dashboard](https://docs.microsoft.com/en-us/learn/certifications/azure-data-engineer) to keep yourself updated on the scope of the latest exam. (Click `Download certification skills outline` in the link.)  
I registered my first exam at the end of November, and took it at the middle of December. In a meanwhile, Microsoft updated the scope of exam, especially changed the name of their service (`Azure Data Warehouse` -> `Azure Synapse Analytics`), but I did not get any email notification about the change. I confronted the word, `Azure Synapse Analytics`, during the exam at the first time, and it makes me quite confused. :p  


## What are the benefits of having certification?  

My major motivation was to have a big picture on Azure cloud platform. When I decided to prepare for this certification, I already have worked with Azure platform over a year as both data engineer and DevOps engineer. Since I studied and used the services on demand, my knowledge and experience were quite scattered, and it makes me forgetting of the details easily. While I prepared for the exam, I got a better understanding on the Azure services, especially how different services are relevant each other and which service/configuration I have to use at the given use case.  

At the same time, you can highligh your CV, and having the certification can potentially make your company having better partnership with Microsoft: [reference](https://trainingsupport.microsoft.com/en-us/mcp/forum/all/benefits-to-my-company-to-have-a-microsoft-azure/e0380874-c2d5-454b-bfab-2b2606ca981c).  

So, why not? :)


## There are two exams

Uniquely, this certification requires the following two exams to earn. There are not a huge differences of the two exams, and even it is difficult to distinguish them and study separately, I recommend to prepare them together and take the exams as close as possible.

- Both exams cover the following Azure services (weights):
    - Storage services (40-45%)
        - `Azure Data Lake`
        - `Azure Cosmos Database`
        - `Azure Synapse Analytics` and `PolyBase`
        - `Azure SQL Database / Azure SQL Server`
        - `Azure Storage Account`
    - Data processing services (25-30%)
        - `Azure Data Factory`
        - `Azure Databricks`
        - `Azure Stream Analytics`
        - Basic knowledge on `Azure IOT Hubs` and `Azure Event Hubs`
    - Services for monitoring and security (30-35%)
        - `Azure Monitor`
        - `Azure Active Directory`
        - `Azure Key Vault`

- Implementing an Azure Data Solution (DP200)  

This exam focuses the detail information about each service, such as which partition is the best choice for the given situation or what is an appropriate sequnce of jobs for loading data to Azure Synapse Analytics from Blob storage.  

I recommend you to have enough hands-on experience, instead of memorizing the details only theoretically. You need to know quite details of each service, but at least, what I felt during the exam is Microsoft does not try to trick you. If you know, you can solve it, if you do not know, you cannot solve it. That is all.

A difference of two exams is DP200 covers monitoring and optimization of the services, while DP201 covers security and compliance instead.

- Designing an Azure Data Solution (DP201)  

This exam focuses design thinking of Azure data services, such as which data storage is the best to be used at the given situation. I felt this exam was way easier than DP200, but my score was lower than DP200. The problem is your score is calculated based on the relative evaluation - you must be better than others for the given exam sheet. So never be relaxed even though you feel the exam easy. It would not be easy only for you :p

I recommend you to get to know the concept and principle of each service - why Microsoft made different services, and what each service is meant to be used. Each service provide documentation and I recommend you to read `overview` and `concepts` section to get the relevant information.

There are also the [case studies](https://github.com/MicrosoftLearning/DP-201-Designing-an-Azure-Data-Solution) for this exam provided by Microsoft.


## Exam preparation strategies  

- If you are completely new for Azure services  

I do not think it is good idea for you to try `Associate` level of certifications then. The prerequisite of `Associate` level certification is `Fundamental` level, and I recommend to study for `Azure Fundamentals` certification first. I did not take the exam for it, but I quickly got through the materials for it. It covers very various and general knowledge on cloud platform, not only Azure specific. Many of them are written in very easy technical terminologies so that it is worth to read even for non-technical folk. If you will not take the exam for `Azure Fundamentals`, you do not need to try to remember all names of services.

[Learning documentation for `Azure Fundamentals` from Microsoft](https://docs.microsoft.com/en-us/learn/paths/azure-fundamentals/)

- If you have around a year of experience on Azure services

This was exactly me. I had quite enough experiences on Azure data storage services and batch processing services, but not stream processing services. So I tried to do many hands-on labs for them, which are from [Microsoft learning](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWuAzL). Reading all materials from Microsoft learning would be too time-consuming for you. I recommend to read them only for your weak points. 

Instead, I recommend you to watch courses and read the documentation for the services.
I took the course from [Linux Academy](https://linuxacademy.com/course/implementing-an-azure-data-solution-dp-200/), and it was quite time-efficient way to get through the information. The course is quite short, and focuses on what you need to know only. But the course does not cover all information you need to know. Especially, the practical exam from this course is only for checking the knowledge which you learned from this course, but the real exam would not look like that at all.  

For further knowledge, I recommend you to read the documentation for each services provided by Microsoft: [example](https://docs.microsoft.com/bs-latn-ba/azure/cosmos-db/?view=azuremediaservices-3.8.0.5). Every service has `Overview` and `Concepts` sections and they are what you must to read to understand both detail setup and design principle. 

At final, you need to try some proper practical tests to check what you are missing. See the `Useful links` section.

- If you have more experience  

I was not in this level as I started preparing for the exam. [Cathrine Wilhelmsen's blog](https://www.cathrinewilhelmsen.net/2019/05/29/preparing-taking-microsoft-exam-dp-200-implementing-azure-data-solution/) has also great guidelines, and I recommend to check this one as well.


## Useful links

Besides of the aforementioned [Microsoft learning](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWuAzL), [Linux Academy](https://linuxacademy.com/course/implementing-an-azure-data-solution-dp-200/), [Microsoft documentation](https://docs.microsoft.com/bs-latn-ba/azure/cosmos-db/?view=azuremediaservices-3.8.0.5), 

- [Azure Architectures](https://docs.microsoft.com/en-us/azure/architecture/architectures/)
    - Studying on the architecture examples is particularly useful for DP201.

- Test exams
    - [Link1](https://www.examtopics.com/exams/microsoft/dp-201/): The best comes the first! The exam sets are very similar with the real exam. There are some wrong answers, but there is `discussion` tab on each question, so you can find other people's complains on the wrong answer.
    - [Link2](https://www.whizlabs.com/microsoft-azure-certification-dp-201/practice-tests/?sscid=c1k3_mxvgr): It provides great exaplanation on the answers to each question.
    - [Link3](https://www.measureup.com/dp-201-microsoft-designing-an-azure-data-solution.html): If provides various and realistic exam patterns.
    - [Link4](https://www.dumpsolutions.com/DP-201-dumps/): The famous `dump`. But it is quite unmanaged, so I do not recommend it personally.
    - [Link5](https://eu1.mindhub.com/dp-200-microsoft-implementing-an-azure-data-solution-microsoft-official-practice-test/p/MU-DP-200): The official practice exam. Quite expensive, but it would be better than retaking exam...


## Exam patterns

You can find the official information on exam patterns [here](https://www.youtube.com/watch?list=PLahhVEj9XNTdZrAYjA7mq4bH1X5cTykpH&v=7CvYGpSVbkA&feature=emb_title).

The exams are around three hours each. It is divided into multiple sections (around from three to five). You can review the questions and your answers inside each section, but once you finish the section, you cannot go back. So please distribute your time well between sections.

There is a special session also, named `Repeated Answers Question`. Around three or four questions are repeated with the same situation but with different answer. You have to answer if the given answer makes sense or not, and there could be all makes sense or nothing makes sense. The reason why I particularly mention this type of section is once you answer, you cannot go back.

I have heard a `rumor` that Microsoft is supposed to add hands-on labs in the exam, but it was not shown in my case.  


## For more information

Please do not hesitate to contact me personally through my email or LinkedIn :) I love to hear the news about the exams and update my posts. But...


## NDA with Microsoft

As you start the exam, you must sign on the [Microsoft Exam Policy and Non-Disclosure Agreement](https://www.microsoft.com/en-us/learning/certification-exam-policies.aspx), which blocks you to share the detail information about exam questions and the answer. This also applies to me, so it is impossible for me to share all information.