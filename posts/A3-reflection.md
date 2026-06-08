---

title: "A3 Reflection: Evaluating the Shen_ren.indie.music Web Prototype"
date: 2026-06-09
author: Yizhou Li
summary: "A final reflection on the performance, user experience, functional requirements, and development process of our web application prototype."
tags:

* A3 Reflection
* Web Prototype
* Evaluation
* User Experience

---

# A3 Reflection: Evaluating the Shen_ren.indie.music Web Prototype

## Introduction

For A2, our group developed **Shen_ren.indie.music**, a web application prototype for an independent music community platform. The website was designed around the idea of “sound rooms”, where users can browse music communities, discover curated playlists, read discussion posts, and access a personal profile. The final prototype includes Home, About, Browse, Community, Discover, and Profile pages.

My main contribution focused on the **Community**, **Discover**, and **Profile** pages. I worked on refining their visual layout, adding image assets, improving typography, adjusting navigation consistency, and making these sections feel more like complete parts of a real music community website. Throughout the process, I also helped make the pages more polished by improving card layouts, profile sections, music-related imagery, and the relationship between visual style and content.

This reflection evaluates the final prototype through performance, usability, accessibility, functional requirements, and future improvement planning. The evidence includes final page screenshots, a Lighthouse audit, a responsive layout check, and a scenario-based user walkthrough. The strongest part of the prototype is its clear visual identity and indie music community atmosphere. However, the evaluation also revealed limitations, especially around responsive navigation and the difference between prototype-level interactions and fully functional backend features.

---

## Evidence 1: Final Prototype Screenshots

The following screenshots show the final state of the main pages in the prototype.

<img src="/deco2017-blog/assets/a3-evidence/01-home.png" alt="Home page final screenshot" width="700">

<img src="/deco2017-blog/assets/a3-evidence/02-about.png" alt="About page final screenshot" width="700">

<img src="/deco2017-blog/assets/a3-evidence/03-browse.png" alt="Browse page final screenshot" width="700">

<img src="/deco2017-blog/assets/a3-evidence/04-community.png" alt="Community page final screenshot" width="700">

<img src="/deco2017-blog/assets/a3-evidence/05-discover.png" alt="Discover page final screenshot" width="700">

<img src="/deco2017-blog/assets/a3-evidence/06-profile.png" alt="Profile page final screenshot" width="700">

---

## Performance and Technical Behaviour

Overall, the prototype performed well as a local web application. The main pages loaded successfully, the navigation routes worked, and the image assets appeared correctly after being placed in the project’s static asset folders. The final site had a clear page structure, including `/`, `/about`, `/browse`, `/community`, `/discover`, and `/profile`, which made the core user journey easy to test.

The Community page was selected for the Lighthouse audit because it is one of the most complex pages in the prototype. It includes a hero section, a large image, a posting bar, discussion cards, tags, sidebar panels, and a closing call-to-action. Testing this page gave a useful indication of how the prototype behaves when visual content and structured interface components are combined.

One performance trade-off was the use of many images. Earlier versions of the website felt plain because they relied too heavily on black and white structure without enough visual atmosphere. Adding images made the Community, Discover, Browse, Home, and Profile pages feel more complete and more connected to the indie music concept. However, image-heavy pages can also increase loading demands. For a high-fidelity prototype, this was acceptable because the images helped communicate the final design direction. If the project were developed further, I would optimise these images by compressing them, resizing them to their display size, and using more efficient formats.

Technically, the prototype communicates the intended interaction model, but not every feature is fully implemented as production functionality. For example, the Community page includes a post input and Post button, while the Profile page includes account options such as Phone Number, Email, Settings, Privacy, Personal Bio, and Switch Account. These elements make the interface feel complete, but they are mainly prototype interactions rather than fully connected backend systems. This distinction is important because the final prototype successfully presents the intended product experience, while still leaving room for deeper technical development.

---

## Evidence 2: Lighthouse Audit

<img src="/deco2017-blog/assets/a3-evidence/09-lighthouse-community.png" alt="Lighthouse audit for Community page" width="700">

The Lighthouse audit was used as evidence for checking the technical behaviour of the Community page. It helped evaluate performance, accessibility, best practices, and SEO in a more structured way than simply judging the page visually. While Lighthouse does not represent the full user experience, it was useful for identifying whether the page loaded correctly and whether basic technical and accessibility considerations were present.

---

## User Experience and Accessibility

The user experience of the final prototype is strongest where the visual system is most consistent. Community, Discover, and Profile use similar colours, spacing, typography, image treatment, and navigation style. This makes the website feel more like one connected product rather than several unrelated pages. The black, off-white, and grey visual system also suits the underground music community concept.

The Community page communicates its purpose clearly. The heading “Where underground listeners talk” immediately explains that this page is for discussion. The posting bar provides a clear entry point for sharing a track, question, or recommendation. The post cards also use a clear hierarchy: avatar, username, room label, time, title, body text, tags, and actions. This makes the content easy to scan.

The Discover page works well because it supports music discovery through mood and atmosphere rather than only genre. Sections such as 3am recommendations, mood collections, editor picks, and tags make the website feel more specific and original. The Profile page also became stronger after adding Account Access, listening identity, saved playlists, recent activity, and image-based playlist cards. These sections make the profile feel like a real user centre rather than a simple static profile page.

For accessibility, the prototype has strengths and limitations. A positive decision was using **Inter** for important body text and content-heavy areas, because the decorative Doto font can be difficult to read at smaller sizes. I also added descriptive `alt` text to images in the pages I worked on, which supports users using screen readers and helps when images fail to load.

However, the responsive layout test revealed a significant usability issue. When the browser was narrowed, the main Community content remained mostly readable, but the top navigation became compressed and some elements overlapped. This could make the site difficult to use on smaller screens. This issue shows that the desktop version of the prototype is much stronger than the mobile version.

---

## Evidence 3: Responsive Layout Check

<img src="/deco2017-blog/assets/a3-evidence/07-responsive-community.png" alt="Responsive Community page screenshot" width="700">

<img src="/deco2017-blog/assets/a3-evidence/08-responsive-nav-issue.png" alt="Responsive navigation issue screenshot" width="700">

These screenshots show the responsive layout test. The main Community content still appeared, but the header navigation became crowded on a narrow screen. This evidence suggests that the prototype needs a dedicated mobile navigation solution, such as a hamburger menu, stacked navigation, or simplified profile/search layout.

---

## Evidence 4: Scenario-Based User Walkthrough

Because I did not have access to formal external participants during the final evaluation stage, I used a scenario-based walkthrough to simulate how different types of users might move through the prototype. The walkthrough focused on whether the main navigation, community features, discovery flow, profile access, and responsive layout were understandable.

| User Type                          | Task                                                           | Result                          | Observation                                                                                                                                                                                                             |
| ---------------------------------- | -------------------------------------------------------------- | ------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| User A: First-time visitor         | Understand what the website is about from the Home/About pages | Completed                       | The overall concept of an indie music community was understandable through the title, navigation, and visual style. However, a clearer short tagline could help new users understand the purpose faster.                |
| User A: First-time visitor         | Find the Community page                                        | Completed                       | The Community label in the top navigation was clear and matched the discussion purpose of the page.                                                                                                                     |
| User B: Indie music listener       | Find music recommendations or playlists                        | Completed                       | The Discover page clearly communicated music exploration through playlist images, mood collections, and tags such as 3am recommendations and Bedroom Noise.                                                             |
| User B: Indie music listener       | Browse sound rooms                                             | Completed                       | The Browse page supported the idea of exploring different sound rooms and music communities.                                                                                                                            |
| User C: Returning community member | Open Ethan Carter’s Profile page                               | Completed                       | The profile entry in the header was recognisable as the user account/profile area.                                                                                                                                      |
| User C: Returning community member | Find account/profile options                                   | Completed with minor hesitation | The Account Access pills were visible, but settings-related actions could be more clearly separated from the public profile content.                                                                                    |
| User C: Returning community member | Try to identify where to post a recommendation                 | Completed                       | The black posting bar on the Community page was visually prominent and clearly suggested a posting interaction. However, this function is still a prototype interaction rather than a fully functional backend feature. |
| Responsive layout check            | Use the Community page in a narrow browser window              | Partially completed             | The main content was still readable, but the header navigation became compressed and some elements overlapped.                                                                                                          |

> “The prototype communicates a strong indie music community identity, and the main pages are easy to find. However, some polished interface elements feel like they should have deeper functionality, and the navigation needs a better responsive design for smaller screens.”

---

## Functional Requirements

The final prototype successfully communicates the main functional idea of an independent music community platform. The website includes pages for browsing, discovery, community discussion, and user profile management. This supports the original concept of a platform where users can explore music through rooms, moods, recommendations, and community activity.

The **Community** page meets the requirement of representing social interaction. It includes a posting area, discussion cards, tags, replies, saved counts, active members, trending topics, and community stats. These elements make the page feel like an active community space. However, the posting system is not fully functional because new posts are not actually stored in a database. This is a limitation, but it is acceptable for the current prototype stage because the interface clearly communicates the intended interaction.

The **Discover** page meets the requirement of supporting music exploration. It presents music through mood-based collections, playlist images, editor picks, and listening tags. This is one of the strongest parts of the prototype because it makes the project feel more specific than a general music website. It supports the idea that users can find music by atmosphere, memory, and context.

The **Profile** page meets the requirement of showing user identity and account-related features. It includes listening identity, favourite sound rooms, saved playlists, recent activity, and account access options. These features make the profile feel like a real user area. However, the account options are still prototype links rather than fully implemented settings pages.

Overall, the functional requirements were mostly achieved at the prototype level. The website demonstrates the intended structure and user flow, but the main limitation is that many interactions are not yet fully connected to backend logic. If this were continued as a production application, real posting, saving, search filtering, profile editing, and account management would need to be implemented.

---

## Critical Reflection and Lessons Learned

The most important lesson I learned from this project was that visual consistency is difficult in group work unless the team establishes a shared design system early. Because different people worked on different pages, the website initially had differences in font choices, spacing, image use, navigation layout, and card styling. When refining Community, Discover, and Profile, I realised how important reusable components are. A shared header, card system, typography scale, image ratio, and button style would have made the final prototype more consistent from the beginning.

I also learned that images can strongly improve the emotional quality of a website. Earlier versions of my pages felt too plain because they were mostly black and white. After adding images related to music rooms, late-night streets, underground venues, playlists, and profile identity, the pages felt more complete and more connected to the indie music theme. However, images also created new responsibilities. They needed consistent sizing, cropping, file naming, and placement. This taught me that visual polish is not just decoration; it affects layout, performance, and user understanding.

The responsive issue was another important lesson. On desktop, the website looks much stronger and more complete. However, when the window becomes narrow, the navigation does not adapt well. This showed me that responsive design cannot be treated as an afterthought. In a future project, I would plan mobile navigation earlier instead of trying to fit the desktop header into a smaller screen.

Finally, I learned that high-fidelity prototypes can create user expectations. When buttons and profile options look realistic, users may expect them to work fully. This is useful for communicating a product idea, but it also creates a gap between appearance and actual functionality. In future work, I would either implement deeper functionality or make prototype interactions clearer.

---

## Future Improvements

If I continued developing this project, I would prioritise four improvements.

First, I would redesign the responsive navigation. The current desktop header should become a mobile-friendly menu on smaller screens. This would solve the overlap problem and improve accessibility.

Second, I would implement real community posting. Users should be able to type a recommendation, submit it, and see it appear in the feed.

Third, I would improve Profile account functions. Phone Number, Email, Settings, Privacy, Personal Bio, and Switch Account should lead to actual account management screens or modals.

Fourth, I would optimise image assets. Compressing and resizing images would improve performance while keeping the strong visual style of the prototype.

---

## Conclusion

The final Shen_ren.indie.music prototype successfully communicates the concept of an indie music community platform. It includes a complete navigation structure, visually developed pages, community discussion content, music discovery sections, and a profile experience. The evaluation evidence showed that the desktop experience is mostly clear and usable, while the main limitations are responsive navigation and deeper backend functionality.

This project helped me understand that a web application is not finished only because it looks complete. It also needs to be tested for performance, usability, accessibility, and functional clarity. The strongest parts of the prototype are its visual identity and music community concept. The most important future improvements are mobile responsiveness, real interaction, and stronger backend support.
