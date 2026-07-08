---
title: "Week 10 Worklog"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.10. </b> "
---
<!-- {{% notice warning %}} 
⚠️ **Note:** The following information is for reference purposes only. Please **do not copy verbatim** for your own report, including this warning.
{{% /notice %}} -->


### Week 10 Objectives:

* Expand the social interaction capabilities by implementing a comprehensive multi-reaction system for comments.
* Enhance the real-time messaging experience by integrating a dynamically themed, native emoji picker.
* Stabilize frontend UI rendering by resolving layout shifts, component clipping, and optimizing component weight.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Backend Architecture & Async Stability:** <br> - Migrated the comment interaction system from a single 'like' to a multi-reaction model (LIKE, LOVE, HAHA, WOW, SAD, ANGRY). <br> - Optimized database operations utilizing JPA Projections to accurately fetch reaction counts while preventing N+1 query inefficiencies. <br> - Diagnosed and resolved a LazyInitializationException within the asynchronous NotificationService by eagerly fetching required User entities prior to publishing events. <br> - Integrated react-reactions library to supply Facebook-style icons for both Post and Comment components. | 06/22/2026 | 06/22/2026 | https://github.com/pht1412/Mini-Social-Network |
| 3 | **Frontend UX, Chatbox & UI Stabilization:** <br> - Integrated emoji-picker-react into the messenger chat input, ensuring dynamic synchronization with the global Dark/Light theme and seamless Unicode text appending. <br> - Eliminated the UI layout shift ("wobbly effect") during hover states by implementing fixed-size wrappers and utilizing MUI <Popover> with disableScrollLock={true} to prevent viewport freezing and container clipping. <br> - Refactored the CommentReactionButton by replacing bloated MUI Button components with lightweight Typography elements to restore layout proportions. <br> - Implemented a showDevelopmentAlert utility using SweetAlert2 with conditional prop spreading to gracefully handle "coming soon" features in menus. | 06/23/2026 | 06/23/2026 | https://github.com/pht1412/Mini-Social-Network |

### Week 10 Achievements:

* Backend Robustness: Hardened the asynchronous notification pipeline by successfully circumventing Hibernate session boundary limitations (LazyInitializationException).
* Enhanced Interactivity: Successfully shipped a fully functional multi-reaction system for comments and an intuitive, theme-aware emoji picker for the real-time chatbox.
* UI/UX Polish: Delivered a seamless, jitter-free frontend experience by resolving layout shifts, optimizing component rendering weights and implementing graceful fallbacks for upcoming features.

<figure align="center">
  <img src="/images/1-Worklog/1.10-Week10/1.png"  width="100%">
  <figcaption><a href="https://github.com/pht1412/Mini-Social-Network/commit/eefb219f23eda72d4004debeae9c65511771edfe">Picture 1: Commit code for project Mini Social Network</a></figcaption>
</figure>