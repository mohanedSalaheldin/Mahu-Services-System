
#  Services Management System - Mobile Client

This repository contains the mobile application frontend for the Services Management System (SMS). The project showcases a production-ready client architecture implemented using Flutter and Dart, emphasizing clean separation of concerns and cross-functional integration.

## Project Operational Status

The development of this commercial system was halted by management during its final phases due to project schedule shifts and external client adjustments. Consequently, this repository serves as a technical portfolio, architectural proof of concept, and documentation of the developed system components.

---

## My Architecture & Key Responsibilities

As the Lead Flutter Developer on this project, my scope of work covered the following areas:

- **Requirements and Technical Specifications:** Documented initial development baselines and aligned feature specifications with implementation constraints.
- **Architecture and Project Setup:** Structured the codebase according to Clean Architecture principles, establishing the separation between the core layers and independent features.
- **State Management:** Implemented predictable UI state cycles across all core workflows using the Cubit pattern.
- **API Integration:** Collaborated with the backend engineer to define RESTful API contracts, handling network data serialization, HTTP caching, and status synchronization with the Node.js and MongoDB backend.

---

## Technical Stack

- **Framework:** Flutter & Dart
- **State Management:** BLoC / Cubit
- **Networking:** Dio (REST API client with interceptors)
- **Local Caching:** Shared Preferences
- **Localization:** Built-in i18n support infrastructure

---

## Module Structure and Implementation Detail

The application organizes features independently to ensure components can be extended or updated in isolation:

```text
lib/
 ┣ core/              # Shared configurations, errors, utilities, and reusable components
 ┣ features/          # Decoupled functional modules
 ┃ ┣ auth/            # Authentication and session handling
 ┃ ┣ landing/         # Onboarding and main dashboard views
 ┃ ┗ user_booking/    # Multi-step service booking engine
 ┃   ┣ cubit/         # Reactive state controllers
 ┃   ┣ models/        # Domain data representations
 ┃   ┣ services/      # Business logic and network repositories
 ┃   ┗ views/         # High-fidelity UI layouts
 ┗ main.dart          # System entry point
````

---

## Development Status and Continuation Roadmap

To transition the current codebase into full production, the remaining integration path requires:

### Subscription Logic

Finalizing the data mapping between the subscription UI components and the remaining backend endpoints.

### Date Filtering

Enhancing the dynamic service filtering behavior to handle multi-zone date parameters.

### Local Database

Scaling up local storage to an embedded database schema (such as Hive or SQLite) as transactional data grows.

---

## Media and Visual Verification

### UI Showcase

> Insert high-quality application screenshots here to demonstrate layout fidelity.

### Functional Demos

* **Core System Workflow:** [Link to system recording or GIF]
* **API & State Integration Demo:** [Link to dynamic interactions recording or GIF]

---

## Developer

**Developed by Mohaned Salaheldin — Flutter Developer**

```
```
