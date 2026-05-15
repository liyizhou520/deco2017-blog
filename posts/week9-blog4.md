---
title: Understanding Data Through DDD and ERD
date: 2026-05-02
author: YIZHOU LI
summary: Reflection on using DDD and ERD methods to organise website data and relationships.
tags:
  - database-design
  - DDD
  - ERD
---
This week completely changed how I think about websites.

Before this tutorial, I mostly focused on what users could visually see on the page. However, this week introduced Data Definition Documents (DDD) and Entity Relationship Diagrams (ERD), which made me realise how much invisible structure exists behind even simple interfaces.

At first, the process felt confusing.

We needed to examine our wireframes and identify every piece of information that would eventually require data behind it.

Suddenly, ordinary interface elements became much more meaningful.

For example, a single Sound Room card actually contains multiple pieces of data:

- Room title
- Description
- Creator
- Image
- Tags
- Creation date
- Navigation link

This forced me to stop thinking about the page as “just layout”.

Instead, I started thinking about systems and relationships.

While creating the DDD, we had to describe each attribute carefully and think about what kind of information the application actually needs in order to function properly.

One thing I found especially useful was separating entities clearly.

For our project, we identified entities such as:

- Users
- Sound Rooms
- Comments
- Tags
- Discussions

At first, I wanted to combine many things together because it felt simpler. But after learning about relationships and normalisation, I understood why separating entities creates a cleaner and more scalable structure.

The ERD stage was even more challenging.

Understanding one-to-many and many-to-many relationships required much more careful thinking than I expected.

For example:

- One user can create many Sound Rooms
- One Sound Room can contain many comments
- One tag can belong to multiple Sound Rooms

Without a proper structure, the data model quickly becomes messy.

This week also improved the way I think about HTML structure. Previously, some sections were designed mainly around appearance. Now I started considering whether the structure actually reflects meaningful data relationships.

Although database design initially felt very technical, I eventually realised it is closely connected to user experience. A poorly organised data structure eventually creates problems for navigation, scalability, and interaction.

By the end of the week, the project felt much more complete conceptually because we finally understood what information the system truly needed.