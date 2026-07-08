---
title: "Week 9 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---
<!-- {{% notice warning %}} 
⚠️ **Note:** The following information is for reference purposes only. Please **do not copy verbatim** for your own report, including this warning.
{{% /notice %}} -->


### Week 9 Objectives:

* Architect and deploy a highly scalable, multi-type reaction system capable of handling high concurrency.
* Optimize frontend rendering cycles, eliminate backend database bottlenecks, and harden API security against spam.
* Synthesize technical achievements and system architecture knowledge into a structured technical blog post.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Backend - Architecture & Concurrency Control:** <br> - Migrated reaction schema to a flexible JSON-based Map to support multi-reaction types without schema alterations. <br> - Optimized memory usage via JPQL Constructor Expressions (ReactionUserResponse) for direct DTO projections. <br> - mplemented in-memory buffer caching (ConcurrentHashMap + @Scheduled) to batch database writes and mitigate high concurrency bottlenecks. <br> - Resolved N+1 queries using batch fetching and HashMap lookups and implemented an actionLock mechanism to prevent API spam. | 06/15/2026 | 06/15/2026 | https://github.com/pht1412/Mini-Social-Network |
| 3 | **Frontend - UI/UX & Backend Debugging:** <br> - Resolved Hibernate type mismatches and patched false-positive 403 Forbidden errors in Spring Security filters. <br> - Implemented a "Hover to React" UI with optimized state management and debounced smart tooltips (400ms) to prevent local DDoS from rapid mouse hovers. <br> - Extracted ReactionListDialog for lazy loading, resolved avatar UI clipping issues and enabled seamless profile routing. | 06/16/2026 | 06/16/2026 | https://github.com/pht1412/Mini-Social-Network |
| 4 | **Documentation & Knowledge Sharing:** <br> - Outlined, drafted and structured technical content for blog post #2, detailing recent architectural optimizations and development experiences. | 06/17/2026 | 06/17/2026 | [Blog post #2 documentation](https://tinyurl.com/23f5rbm6) |
| 6 | **Team meeting:** <br> - Team meeting at a coffee shop. | 06/19/2026 | 06/19/2026 | |


### Week 9 Achievements:

* Scalability & Performance: Successfully shipped a highly extensible reaction mechanism. Dramatically improved application performance through batched database operations, direct DTO projections and frontend debouncing.
* System Stability & Security: Enhanced system security by resolving deep-rooted Spring Security anomalies and implementing application-level rate-limiting guardrails (actionLock).
* Technical Communication: Translated complex engineering solutions into accessible documentation by initiating the second technical blog post.

<figure align="center">
  <img src="/images/1-Worklog/1.9-Week9/1.png"  width="100%">
  <figcaption><a href="https://github.com/pht1412/Mini-Social-Network/commit/2b1ba7a331b68933efd01d062c91cd82f5e9cc2a">Picture 1: Commit code for project Mini Social Network</a></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.9-Week9/2.png"  width="100%">
  <figcaption><i>Picture 2: Post interaction feature with multiple emotion options</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.9-Week9/3.png"  width="100%">
  <figcaption><i>Picture 3: List of users who have interacted with the post</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.9-Week9/4.png"  width="100%">
  <figcaption><i>Picture 4: Comment section with commenter's name and profile picture</i></i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.9-Week9/5.png"  width="100%">
  <figcaption><i>Picture 5: Team meeting at a coffee shop</i></figcaption>
</figure></i></figcaption>
</figure>