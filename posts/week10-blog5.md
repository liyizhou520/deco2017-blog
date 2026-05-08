---
title: Integrating APIs and Thinking About Deployment
date: 2026-05-09
author: YIZHOU LI
summary: Reflecting on deployment, API integration, error handling, caching, and secure API key management
tags:
  - week10
  - API
  - deployment
---
This week focused on deployment and external integrations, which helped me understand how a web application connects to the wider internet. Previous weeks focused on structure, data, and internal system design, but this week showed that an application also needs to communicate with external services, handle failure, and be prepared for real users.

One important concept was deployment. Running a project locally is very different from making it available online. Localhost only works on my own machine, while a deployed application needs hosting, HTTPS, and a reliable environment. This made me realise that deployment is not just the final step of a project, but part of the design and development process.

The lecture also explained CI/CD, which I had already used indirectly through the blog. When I push a markdown file to GitHub, GitHub Actions automatically builds and publishes the site. This helped me understand continuous deployment as a workflow where changes can be tested and published without doing every step manually.

Another key topic was APIs. An API allows one program to communicate with another program. In the tutorial, the weather API example showed how an application can request external data and then display it to users. For my A2 project, this makes me think about possible music-related integrations, such as pulling album information, artist metadata, or playlist data from an external API. However, this would need to add real value rather than being included just for novelty.

This week also introduced practical concerns around API use. External APIs can fail, return unexpected data, or become unavailable. Because of this, error handling is essential. Instead of allowing the app to crash, the system should fail gracefully and show a useful message to the user. Caching is also important because it reduces repeated API calls, improves performance, and helps avoid rate limits or quotas.

The final important issue was security. API keys and credentials should never be committed to a public repository. They should be stored in a configuration file that is excluded from Git. This is especially important because even deleting a key later does not fully remove it from commit history.

Overall, Week 10 helped me understand that web applications are not isolated systems. They depend on hosting, external services, network reliability, and secure configuration. Good design therefore includes not only interface and data structure, but also how the application behaves when connected to real services and real users.
