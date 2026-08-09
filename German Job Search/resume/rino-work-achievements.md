Based on the work you’ve described across this project and the team-direction document, your achievements can be summarised around one major transition: **you moved from solving individual engineering problems to building infrastructure and platforms that enable autonomous-driving fleets to operate at scale.** Your team’s scope now centres on software, maps, configuration and calibration delivery, with an emphasis on unified management, safe delivery and large-scale fleet operations. 

### 1. Dramatically improved software delivery efficiency

One of your clearest measurable achievements is improving **SOTA/software deployment time from roughly 30 minutes to around 10 minutes on average — about a 67% reduction**.

This was not merely a speed optimisation. It reduced vehicle preparation time, shortened iteration cycles for development and testing, and increased the number of vehicles that could be updated within the same operational window.

At the same time, you increased the system’s maximum deployment capacity from approximately **200 vehicles to 5,000 vehicles**, a **25× increase in scale**.

Together, these two numbers tell a strong story:

> **Faster deployment, while simultaneously moving from hundreds to thousands of vehicles.**

### 2. Designed and built a fleet-scale FOTA platform

You drove the design and implementation of a **FOTA system for autonomous vehicles**, progressing it through multiple milestones and completing the M3/MVP stage for deployment.

The work went beyond a conventional OTA downloader. You considered the complete vehicle-side upgrade lifecycle, including distributed execution across TBOX/ADCU nodes, upgrade orchestration, failure recovery, power-loss safety, client architecture, server deployment and web-based management.

This represents a shift from maintaining scripts and individual deployment mechanisms towards establishing a **standardised software lifecycle-management platform**.

### 3. Built a foundation for unified vehicle software and data delivery

Your work gradually brought several previously separate engineering problems under one architecture:

* software/version deployment;
* high-definition/local-map distribution;
* vehicle configuration delivery;
* calibration-file management;
* vehicle-side execution and verification;
* service-health monitoring;
* interrupted transfer and recovery;
* version/state consistency.

This corresponds closely to the product direction you have identified: a unified delivery and operations platform for **software, maps, configuration and calibration across autonomous-driving fleets**. 

That is important because the achievement is not simply “implemented several tools”. You are building the **delivery infrastructure between cloud-side engineering systems and thousands of physical vehicles**.

### 4. Improved large-map distribution architecture

You worked extensively on one of the harder practical problems in autonomous-driving infrastructure: distributing very large map datasets to vehicles with limited disk space and unreliable network conditions.

You investigated and challenged several approaches, including:

* full-copy + incremental `rsync`;
* rsync-based diff distribution;
* OverlayFS-based old/new-map switching;
* incremental updates;
* interrupted-transfer recovery;
* storage-space optimisation;
* deployment progress and ETA accuracy.

More importantly, you were not merely implementing proposals handed to you. You evaluated their architectural consequences — disk consumption, atomicity, rollback capability, consistency, failure modes and operational complexity — and pushed towards a safer long-term solution.

### 5. Improved reliability and observability of vehicle deployment

You worked on making large-scale vehicle operations **observable rather than opaque**.

Examples include investigating accurate `rsync --info=progress2` progress calculation, interrupted-transfer behaviour, remaining-time inaccuracies and transfer-state semantics, as well as exploring lightweight monitoring of vehicle-hosted web services across several thousand vehicles.

This moves fleet operations towards the characteristics identified in your product positioning: **verifiable, recoverable and traceable delivery**, rather than merely “sending files successfully”. 

### 6. Standardised vehicle configuration and calibration management

You improved the engineering model around vehicle-specific and vehicle-series configuration, particularly camera/lidar intrinsic and extrinsic calibration files.

Your work included deciding how fixed model-level calibration data should be represented, automating retrieval and generation, integrating calibration repositories, and reducing manual handling.

This contributes to a broader result: vehicles receive not just the correct software version, but the **correct combination of software, maps, configuration and calibration data**.

### 7. Improved internal engineering infrastructure

You also worked on infrastructure that improves the team’s development efficiency, including:

* evaluating an internal Python package distribution mechanism;
* investigating GitLab PyPI Registry;
* improving deployment automation;
* comparing systemd timers with cron;
* managing long-running `rsync` processes;
* investigating distributed FRP architecture for bandwidth scaling;
* planning cloud deployment of backend and web services.

These initiatives reduce duplicated engineering work and make internal capabilities reusable instead of project-specific.

### 8. Started productising what was previously engineering tooling

A particularly significant change is that your work has increasingly become **product-oriented rather than tool-oriented**.

You have been defining and designing a vehicle-management platform, including web UI, product identity, icons, information architecture and a formal product positioning.

The emerging positioning is:

> **A unified delivery and operations-management platform for software, maps, configuration and calibration for autonomous-driving fleets.** 

You have also begun treating documentation as a product capability rather than distributing manually maintained PDFs, exploring a maintainable user-documentation system for multiple products.

### 9. Began transitioning from individual contributor to technical/product leader

Your organisational contribution has also changed.

As the team expanded to three people, you began transferring routine development and issue-resolution work to other engineers and shifting your attention towards:

* technical direction;
* architecture;
* project prioritisation;
* product definition;
* team responsibilities;
* long-term platform strategy.

This is an important achievement in itself: **your leverage is starting to come from systems and people, rather than the number of problems you personally fix.**

---

## Condensed performance-review version

A concise summary suitable for a promotion or annual review would be:

> Over the past period, I have focused on transforming autonomous-vehicle software delivery from individual engineering tools into a scalable fleet-management platform. I reduced average SOTA deployment time from approximately **30 minutes to 10 minutes** while increasing maximum deployment capacity from **200 to 5,000 vehicles**. I led the design and implementation of our FOTA platform, improved large-scale map distribution and recovery mechanisms, and standardised the management and delivery of vehicle software, maps, configurations and calibration data.
>
> In parallel, I improved deployment observability, reliability and internal engineering infrastructure, and helped establish the product direction for a unified autonomous-driving fleet delivery and operations platform. As the team expanded, my role also evolved from primarily hands-on development and issue resolution towards **architecture, product planning, technical decision-making and team leadership**.

The strongest promotion narrative is therefore not **“I completed many projects.”** It is:

**“I built the infrastructure that allowed the organisation to move from managing hundreds of vehicles manually to operating thousands of vehicles systematically, and I am now turning that infrastructure into a reusable product and team capability.”**
