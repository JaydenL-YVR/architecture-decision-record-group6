# Architecture Decision Record (ADR)

### Submitters

Jayden, Honglei, Parth, Prabal

- August Beats


## Change Log
Created: 2024-02-07
Updated: 2024-02-08

## Context

The design is architecturally significant as it determines the fundamental approach 
for developing the retail mobile app, which involves critical decisions impacting 
performance, user experience, and scalability. The high-level design approach includes 
selecting the app type, UI framework, backend language, permissions, data storage, 
and any additional frameworks or technology stacks.


## Proposed Design

Services
Native app development for optimal performance and user experience.
Utilization of React as the UI framework for its flexibility and extensive ecosystem.
JavaScript as the backend language for its compatibility with React and ease of development.
Permissions for gallery images, location service for delivery tracking, and notifications/alerts.
SQL+ for data storage to ensure relational database capabilities and robustness.

## Considerations

- Alternatives considered included cross-platform frameworks like React Native or Flutter, but native development was chosen for better performance and user experience.

## Decision

We agree to proceed with the following decisions:

- Native, web, or hybrid app - Native
- UI Framework - React
- Backend language - javascript
- Permissions - gallery images, location service for delivery tracking, and notification/alerts
- Data storage - SQL+ 

## Other Related ADRs



Format:

- \[None\]\(\) - Relevance


## References

ADR: https://github.com/joelparkerhenderson/architecture-decision-record?tab=readme-ov-file#how-to-start-using-adrs-with-git

Format:

- \[Title\]\(URL\)
