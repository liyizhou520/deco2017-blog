---
title: From Interface Design to Data Structures
date: 2026-05-02
author: YIZHOU LI
summary: Understanding how wireframes translate into data structures through DDDs, ERDs, and relational thinking
tags:
  - week9
  - DDD
  - ERD
---
This week introduced a major shift in how I understand design, moving from interface-focused thinking to data-driven system design. Previously, I approached wireframes mainly as visual representations of layout and interaction. However, I now understand that every element in a wireframe represents a commitment to data, and must be supported by a structured backend.

One key concept is that “every box is a promise”. A simple UI element such as a product card or a discussion post implies the existence of multiple data attributes, such as title, image, metadata, and relationships with other entities. This realisation highlights that design decisions directly impact how data must be defined and organised.

The introduction of Data Definition Documents (DDDs) provided a structured way to identify and describe these data requirements. By listing attributes, descriptions, and example values, DDDs help translate abstract designs into concrete data needs. During this process, I found that certain attributes felt uncomfortable, particularly when dealing with lists or repeated values. This discomfort often revealed hidden entities that needed to be separated into their own structures.

This naturally led to the development of Entity Relationship Diagrams (ERDs), which visualise how different entities connect. Rather than focusing on individual pieces of data, ERDs emphasise relationships, which are central to how systems function. Concepts such as one-to-many and many-to-many relationships demonstrate that data does not exist in isolation, but as part of a network of connections.

Understanding many-to-many relationships was particularly important, as they require the creation of junction tables to maintain proper structure. This prevents redundancy and ensures data integrity. It also reinforces the idea that good system design depends on carefully modelling relationships rather than simply storing information.

The introduction of SQL joins further demonstrated how these relationships operate in practice. Once data is separated into different tables, joins are required to reconstruct meaningful information. This highlights the importance of designing clear and logical relationships at the data level.

Overall, this week has fundamentally changed how I approach design. Instead of focusing only on what users see, I now consider what data structures are required to support those interactions. This shift from visual design to system thinking will be essential when developing more complex and scalable applications in the future.
