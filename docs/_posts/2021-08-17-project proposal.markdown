---
layout: post
title:  "3. Project proposal"
date:   2021-08-17 11:59:00 +0700
categories: jekyll update
---
# Project proposal

## Overview:

My project is about creating a grammatical correction engine with Vietnamese texts as Grammarly has done with English. I wanted to create an engine that can correct grammar mistakes, typos, incorrect word choices and incorrect position of accents in Vietnamese texts. I intended that this service could be delivered over the Internet such as the case with Grammarly or it could be provided as a software package to run locally on a machine such as with the current service offered in Microsoft Word.

## Motivation:

I thought of this idea when I heard a friend complaining that he had to proofread papers as a part of his part-time job. I then started to wonder if there is a way to automate this time-consuming task of checking for grammatical mistakes and typos and make the job of proofreader easier as they now can focus more on the content. This product has potential as even native speaker of a language can make mistakes, therefore, having something that can automatically suggest, and correct language mistake will have a market as Grammarly has proven.

## Description:

If you are a student or rather anyone working often with English documents, you are often familiar with Grammarly. Grammarly is a service that, from documents, tags and suggest corrections to grammar, typos, and word choices. I plan to replicate this service, but instead of doing this with English documents, I plan to do this with Vietnamese documents. This task could be defined as a translation task in Natural language processing. By using the source document as the source language, it could be “translated” into standard Vietnamese. The system should be able to tag the changes has been done to the source document and identify what kind of change is it. Then from the tags, I can derive my features. The features are:

* Identification of grammatical mistakes. 
* Identification of typo. This includes incorrect placement of accents, mistake in use of “vần” such as “ch”, “tr” 
* Suggestion for more appropriate word choices in the context.

I planned to deploy this service in 2 ways. First, I will have a website that allows user to upload documents in which it could be analyzed, and the user can get the result immediately. Another method that I planned to deploy this application is to release addons for applications such as Google Docs or Microsoft Word. This allowed the user to get correction for their documents as they work on it. An additional method that this app could be deployed that I will investigate is as an API. Users can make an API call with the text that should be analyzed, and the service will return the analyzed text that has the suggestion tags.

## Tools and Technologies:

I planned to base my project on the GECToR – Grammatical Error Correction: Tag, Not Rewrite project by Grammarly (arXiv:2005.12592v2 [cs.CL]). By using their framework which runs on PyTorch which is a machine learning platform, I would be able to reduce my workload to adapting the tagging system to the specifics of Vietnamese. I would also have to create a new dataset for training as there is no commonly available dataset to train the models with Vietnamese language features and quirks. For the front end of this product, I planned to use C# to be a cross platform front end for this application. For the training of the models and the delivery of the services, I intended to use cloud service providers to provide the computing power as well as distribution of the product. 

## Skill required:

My project needs an advanced understanding of Natural Language Processing and Machine Learning.  I will also need to create a front end for the user to be able to use the product. There should not be any special needs of hardware as cloud computing providers can provide the computing power that I need like high performance computers to train models and high availability servers and content delivery network to deliver the service.

## Outcome

I don’t intend for this project to solve any great problem of our society. Rather, I oriented my project to save people’s time. Therefore, I am contributing to solving the problem of our society by allowing people to focus more on solving problem rather than spending that time on some mundane tasks such as correcting grammar mistakes. Another outcome of this project is that I am able to satisfy my passion in making a project involving machine learning.