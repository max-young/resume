# Rino.ai Work Achievements (2022–Present)

This document is the fact base for the German-market CV. It consolidates the
Rino.ai details already present in the locally generated CV and the positioning
in `German Job Search/german_plan.md`.

> Verification note: the supplied ChatGPT Project URL requires an authenticated
> ChatGPT session and could not be read from the current Codex environment.
> Confirm the exact fleet sizes, timing figures, incident definition and role
> title against the project before external use.

## Career positioning

**Senior Software Engineer — Autonomous Driving Operations, OTA & Fleet Platforms**

- 13+ years building production software and data systems, including 4+ years
  in autonomous driving.
- End-to-end ownership: field problem discovery, product/workflow design,
  architecture, full-stack implementation, deployment and operational support.
- Connects R&D, factory and fleet-operations teams rather than working on an
  isolated application layer.
- Strongest stack: Python, React/Next.js and Linux/DevOps; practical C++ and
  OpenCV in vehicle environments.

## 1. Fleet OTA and release platform

### Situation and scope

- Software and map distribution for thousands of autonomous vehicles.
- Map/software artifacts can reach hundreds of gigabytes.
- Vehicles operate over unreliable networks, making progress visibility,
  version consistency and failure recovery core requirements.

### Ownership and implementation

- Built an event-driven control plane with Flask, Celery and RabbitMQ and a
  Next.js operations frontend.
- Used MQTT/EMQX and WebSocket-based progress reporting to connect vehicle-side
  execution with the operations workflow.
- Implemented vehicle, series and version management, version-consistency
  controls and failure-handling workflows.

### Result

- Automated large-scale software and map deployment.
- Reduced average download time from hours to under 30 minutes.
- Made very large deployments operable under unreliable field-network
  conditions.

## 2. Vehicle calibration platform

### Situation and scope

- Factory and field calibration was a throughput bottleneck.
- The workflow has been used on hundreds of vehicles.

### Ownership and implementation

- Built an end-to-end workflow using Python, Shell, C++ and OpenCV.
- Converted field knowledge and manual steps into a repeatable platform used by
  factory and fleet teams.

### Result

- Increased factory throughput from 2–3 to 10+ vehicles per day.
- Reduced field calibration time from 0.5–1 day to under 30 minutes.

## 3. Fleet operations platform

### Situation and scope

- R&D and operations needed shared, standardised workflows for incidents and
  route delivery.

### Ownership and implementation

- Built the system with Flask, React and Ant Design.
- Productised cross-team workflows for incident management and new-route
  delivery.

### Result

- Helped reduce the operational incident rate from 13 to 7 per 10,000 km within
  six months.
- Supported delivery of dozens of new routes.

## 4. Linux fleet reliability and maintenance

- Automated fleet maintenance with rsync and systemd timers.
- Added disk-protection measures and remote-access tooling.
- Improved the reliability and maintainability of large-scale vehicle software
  operations.

## Resume-ready achievement bullets

- Built an event-driven OTA and release platform that automated software and map
  distribution to thousands of autonomous vehicles, reducing average download
  time from hours to under 30 minutes.
- Engineered deployments of software and map artifacts up to hundreds of
  gigabytes over unreliable networks, with live progress reporting, version
  controls and failure-handling workflows.
- Created a vehicle calibration platform used on hundreds of vehicles,
  increasing factory throughput from 2–3 to 10+ vehicles per day and reducing
  field calibration from 0.5–1 day to under 30 minutes.
- Delivered a shared incident and route-delivery platform for R&D and operations,
  helping reduce the operational incident rate from 13 to 7 per 10,000 km in six
  months and supporting dozens of new routes.
- Automated Linux fleet maintenance and disk protection using rsync and systemd,
  improving the reliability of vehicle software operations at scale.

## Facts to confirm before applying

- Official English job title at Rino.ai.
- Whether “thousands of vehicles” describes deployed, managed or supported
  vehicles.
- Whether “under 30 minutes” refers to transfer, installation or the complete
  deployment workflow.
- Whether “operational incident rate” or “accident rate” is the internally
  correct definition for the 13-to-7 metric.
- Whether public disclosure of EMQX, fleet scale, artifact size and the numeric
  results is permitted.
