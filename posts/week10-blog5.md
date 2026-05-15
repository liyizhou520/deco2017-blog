---
title: Learning APIs and External Data
date: 2026-05-09
author: YIZHOU LI
summary: Reflection on using APIs, handling external data, and understanding graceful failure in applications.
tags:
  - apis
  - json
  - backend
---
This week introduced APIs and external data handling, which was probably one of the most technically challenging topics so far.

Before this tutorial, most of our project existed entirely inside our own system. However, APIs introduced the idea that applications constantly communicate with outside services and external data sources.

At first, the concept felt intimidating because there were many unfamiliar terms:

- JSON
- Fetch requests
- API endpoints
- Authentication
- Geocoding
- Caching
- Error handling

The tutorial focused heavily on understanding how data moves between systems.

One important lesson this week was graceful failure.

Instead of assuming APIs always work perfectly, we learned that applications should expect failure and respond carefully.

For example:

- The API might return invalid data
- The request may fail
- A city name may not exist
- The server may return an error

Using try/catch blocks made me realise that programming is not only about successful outcomes. Good systems are designed to survive mistakes and unexpected situations.

We also worked with weather APIs and geocoding APIs.

Although the tasks were guided step-by-step, I still found it difficult initially because I needed to understand both JavaScript logic and data structure at the same time.

One important moment for me was understanding JSON responses.

At first, large nested JSON objects looked confusing, but after analysing the structure more carefully, I started recognising patterns and understanding how applications extract specific values from API responses.

The caching section was also interesting because it introduced performance thinking.

Instead of repeatedly calling an API every single time, applications can temporarily store previous results to reduce unnecessary requests and improve speed.

This helped me understand that backend logic is not only about functionality but also efficiency.

Another valuable topic was API security and API keys.

The lecture emphasised that sensitive information should never be directly exposed inside public repositories. This made me more aware of responsible development practices.

Overall, this week shifted my understanding of websites again.

A website is not just a collection of pages anymore. It is a system constantly communicating with servers, APIs, databases, and users simultaneously.

Even though the concepts were difficult, I can now better understand how modern web applications actually operate behind the scenes.