---
title: "Week 6 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---
<!-- {{% notice warning %}} 
⚠️ **Note:** The following information is for reference purposes only. Please **do not copy verbatim** for your own report, including this warning.
{{% /notice %}} -->


### Week 6 Objectives:

* Optimize database interaction and resolve critical backend performance bottlenecks within the Spring Boot (Data JPA) application.
* Implement the end-to-end lifecycle of the social Friend Request feature.
* Enhance the React frontend performance, specifically focusing on the Admin UI's data fetching, state management, and component rendering cycles.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Backend Optimization (JPA & Caching):** <br> - Analyzed query execution logs to identify performance bottlenecks in FeedService. <br> - Eliminated N+1 queries by implementing Pre-warm L1 Cache and batch fetching original posts/media via findByIdInWithMedia. | 05/25/2026 | 05/25/2026 | https://github.com/pht1412/Mini-Social-Network |
| 3 | **Backend Stability & Refactoring:** <br> - Resolved the Hibernate in-memory pagination warning (HHH000104) in PostRepository using @EntityGraph. <br> - Refactored PostService.mapToPostResponse to prevent infinite recursion (StackOverflow risks). <br> - Applied @Transactional(readOnly = true) to read operations and refactored toggleLike for graceful error handling. | 05/26/2026 | 05/26/2026 | https://github.com/pht1412/Mini-Social-Network |
| 4 | **Frontend - Social Features & Data Mapping:** <br> - Developed the dynamic Friend Request button on the user profile. <br> - Managed the complete friend request lifecycle states: Add Friend, Request Sent and Friends. <br> - Refactored PostManager.tsx to correctly map and consume Spring Boot's Page<T> JSON structure. | 05/27/2026 | 05/27/2026 | https://github.com/pht1412/Mini-Social-Network |
| 5 | **Frontend - Admin UI & Performance Optimization:** <br> - Implemented robust server-side pagination for the Admin UI using MUI TablePagination. <br> - Enhanced the Admin Dashboard to dynamically display interaction statistics and media previews. <br> - Optimized the React data fetching cycle using the useCallback hook to prevent infinite component re-renders. | 05/28/2026 | 05/28/2026 | https://github.com/pht1412/Mini-Social-Network |
| 6 | **Team meeting:** <br> - Team meeting at the coffee shop. | 05/29/2026 | 05/29/2026 | |


### Week 6 Achievements:

**Backend Performance & Stability:**
* Significantly improved query efficiency by eliminating N+1 problems using L1 Cache pre-warming and batch fetching.
* Successfully resolved the Hibernate in-memory pagination warning (HHH000104) by replacing JOIN FETCH with @EntityGraph.
* Hardened backend stability by mitigating StackOverflow risks during DTO mapping and reducing database lock contention using @Transactional(readOnly = true).
**Frontend UI/UX Enhancements:**
* Successfully shipped the dynamic Friend Request integration (Add, Sent, Friends state lifecycle) on user profiles.
* Upgraded the Admin Dashboard by implementing seamless server-side pagination (handling Spring Boot's Page<T> structure via MUI TablePagination) and adding media preview capabilities.
* Optimized React component lifecycle and eliminated infinite re-renders by strategically implementing the useCallback hook for data fetching.

<figure align="center">
  <img src="/images/1-Worklog/1.6-Week6/1.png"  width="100%">
  <figcaption><a href="https://github.com/pht1412/Mini-Social-Network/commit/b62e54e24524d1e2b0ed904ddf4e16408e3a0567">Picture 1: Commit code for project Mini Social Network</a></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.6-Week6/3.png"  width="100%">
  <figcaption><i>Picture 2: Admin UI with server-side pagination and media previews</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.6-Week6/4.png"  width="100%">
  <figcaption><i>Picture 3: Friend status on user profiles</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.6-Week6/2.png"  width="100%">
  <figcaption><i>Picture 4: Team meeting at the coffee shop</i></figcaption>
</figure>