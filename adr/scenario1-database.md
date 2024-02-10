# Architecture Decision Record (ADR)

### Submitters

Jayden, Honglei, Parth, Prabal

- August Beats


## Change Log
Created: 2024-02-07  
Updated: 2024-02-09

## Context

The design is architecturally significant as it determines the fundamental approach for developing the retail mobile app, which involves critical decisions impacting performance, user experience, and scalability. The high-level design approach includes selecting the app type, UI framework, backend language, permissions, data storage, and any additional frameworks or technology stacks.


## Proposed Design

Services Native app development for optimal performance and user experience. JavaScript as the backend language for its ease of development. Permissions for gallery images, location service, and notifications/alerts. MariaDB, SQLite for data storage to ensure relational database capabilities and robustness.

## Considerations

-	Alternatives considered included cross-platform frameworks like React Native or Flutter, but native development was chosen for better performance and user experience.

-	Consideration was also given to the permissions required for the app to access device features such as gallery images, location services for delivery tracking, and notifications/alerts.


## Decision

We agree to proceed with the following decisions:
-	Native, web, or hybrid app - Native, Swift for iOS, Kotlin for Android
-	UI Framework: SwiftUI for iOS, Native Components for Android
-	Backend language: JavaScript
-	Backend Framework: Node.js + Express.js
-	Permissions: Required for accessing gallery images, location services, and sending notifications/alerts
-	Data storage (Server Side): MariaDB
-	Data storage (Client Side): SQLite
-	Image storage: Google Cloud CDN
-	Analytics Service - Google Analytics
-	International: Local support from SwiftUI, Local support from Android

## Rationale
-	Native app: Chosen for optimal performance and user experience.
-	JavaScript: JavaScript is easy to use and has enough libraries to build the server-side program, it is easy to integrate with Database and third-party APIs.
-	Node.js + Express.js: They are the best choice to build a backend server using JavaScript.
-	Google Cloud CDN: CDN is an easy way to store static images, and we could write some code to implement lazy loading, compression, etc.
-	MariaDB: Chosen for reliability, scalability, and support for relational data models. It is also easy to use, and it is free.
-	SQLite: Chosen for the offline mode, to cache the customers’ order history, so they can check it to support offline mode.
-	Google Analytics: Chosen to track user behavior, the team could improve the app’s performance and user experience from the collected data.
-	Native App has local support for internationalization, we could simply use the supported features from the platform accordingly.


## Other Related ADRs

None

## References

ADR Template: 

EdgeX Foundry ADR.
[https://github.com/joelparkerhenderson/architecture-decision-record?tab=readme-ov-file#how-to-start-using-adrs-with-git](https://github.com/joelparkerhenderson/architecture-decision-record/blob/main/locales/en/templates/decision-record-template-by-edgex/index.md)https://github.com/joelparkerhenderson/architecture-decision-record/blob/main/locales/en/templates/decision-record-template-by-edgex/index.md

