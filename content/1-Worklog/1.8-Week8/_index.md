---
title: "Week 8 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---
<!-- {{% notice warning %}} 
⚠️ **Note:** The following information is for reference purposes only. Please **do not copy verbatim** for your own report, including this warning.
{{% /notice %}} -->


### Week 8 Objectives:

* Overhaul core system functionalities and stabilize AWS S3 media integrations.
* Audit and resolve critical state management bugs in notifications and social features.
* Achieve feature parity between local development and the production environment for post management functionalities.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Cloud Storage Integration (Media Fix):** <br> - Investigated and debugged the AWS S3 video upload failure. <br> - Fixed multipart upload configurations and ensured correct MIME type handling to successfully restore video uploading capabilities. | 06/08/2026 | 06/08/2026 | https://github.com/pht1412/Mini-Social-Network |
| 3 | **State Management & Data Mapping:** <br> - Notification System: Refactored the notification lifecycle to resolve the "stuck unread" state bug, ensuring proper read/unread status updates. <br> - Social Features: Debugged and fixed the API response/state management issue that caused the user's friend count to incorrectly display as zero. | 06/09/2026 | 06/09/2026 | https://github.com/pht1412/Mini-Social-Network |
| 4 | **UI/UX Bug Scrub (Mini Game Module):** <br> - Audited the Mini Game module to identify UI anomalies. <br> - Patched UI glitches by recovering missing image assets and resolving cross-browser typography/font rendering issues. | 06/10/2026 | 06/10/2026 | https://github.com/pht1412/Mini-Social-Network |
| 5 | **Feature Migration & Environment Parity:** <br> - Synchronized post management features from the local environment to the production server. <br> - Successfully integrated, configured and tested the "Edit Post" and "Delete Post" API endpoints and UI components on the deployed environment. | 06/11/2026 | 06/11/2026 | https://github.com/pht1412/Mini-Social-Network |
| 6 | **Team meeting and study:** <br> - Study, work and team meeting at AWS office. | 06/12/2026 | 06/12/2026 | |


### Week 8 Achievements:

* System Stability: Restored full multimedia capabilities by resolving the AWS S3 video upload pipeline issues.
* User Experience (UX): Eliminated critical state anomalies in the notification system and UI rendering bugs within the Mini Game module, significantly improving user satisfaction.
* Deployment Parity: Successfully migrated essential CRUD operations (Edit/Delete posts) to the cloud, ensuring operational consistency between local and production environments.

<figure align="center">
  <img src="/images/1-Worklog/1.8-Week8/1.png"  width="100%">
  <figcaption><a href="https://github.com/pht1412/Mini-Social-Network/commit/51d501ed9195d001235a081be0397c355852ca82">Picture 1: Commit code for project Mini Social Network</a></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.8-Week8/2.png"  width="100%">
  <figcaption><i>Picture 2: Read/unread status of notifications works correctly</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.8-Week8/3.png"  width="100%">
  <figcaption><i>Picture 3: Friend count displays correctly</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.8-Week8/4.png"  width="100%">
  <figcaption><i>Picture 4: Mini Game UI with correct images and fonts</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.8-Week8/5.png"  width="100%">
  <figcaption><i>Picture 5: Edit post UI</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.8-Week8/6.png"  width="100%">
  <figcaption><i>Picture 6: Delete post UI</i></figcaption>
</figure>

<figure align="center">
  <img src="/images/1-Worklog/1.8-Week8/7.png"  width="100%">
  <figcaption><i>Picture 7: Study, work and team meeting at AWS office</i></figcaption>
</figure>