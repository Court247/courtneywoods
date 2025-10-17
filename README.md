# 👋 Hi! I'm Courtney Woods

Full stack developer passionate about art, gaming, design, and scalable applications. 

## 📑 Table of Contents

1. 🚀 [Featured Projects](#-featured-projects)
    - [ArtBook](#-artbook)
    - [Bank Web App](#banking-web-app)
    - [TopTier](#toptier)
    - [Lightweight Intrusion Detection System](#lightweight-intrusion-detection-system)
2. 🧰 [Skills & Tools](#skills)
3. 🌱 [Currently Learning]()
4. 💬 [About Me](#about-me)
5. 📫 [Contact](#contact)


## 🚀 Featured Projects

### 🎨 Artbook

***Overview:***

ArtBook is a full-stack social media application designed to give artists a space to share their work, connect with others, and build creative communities. Built as a monorepo, it integrates web, mobile, and backend services into one cohesive ecosystem.

***Key Features***

- User-generated content — artists can upload, caption, and share artwork.

- Comments & Likes — engagement features built into both posts and comments.

- Reposts & Follows — users can repost or quote-share art and follow other creators.

- Notifications — real-time alerts for likes, comments, follows, and reposts.

- Reporting & Admin Controls — moderation tools for safe, community-driven spaces.

- Cross-platform — single backend serving React (web) and Flutter (mobile) apps.

***Tech Stack***
| Layer              | Technology                       |
| ------------------ | -------------------------------- |
| **Backend**        | FastAPI (Python)                 |
| **Frontend (Web)** | React (JavaScript)               |
| **Mobile**         | Flutter (Dart)                   |
| **Database**       | MySQL (SQLAlchemy ORM)           |
| **Auth & Media**   | Firebase Auth & Firebase Storage |

***Architecture & Approach***

ArtBook is structured as a monorepo to maintain consistency and shared logic across platforms.

- Backend (FastAPI) — Handles REST API endpoints for users, posts, comments, and more. Firebase tokens are validated server-side for secure access.

- Frontend (React) — A responsive web interface for browsing, posting, and engaging with content.

- Mobile (Flutter) — Offers native performance and UI parity with the web experience.

- Database Layer (MySQL) — Normalized schema ensuring efficient relations between posts, users, comments, and notifications.

***My Role & Challenges***

I designed and implemented both the API layer and database schema, connecting the authentication and media layers through Firebase.

- Built reusable utility modules (firebase_auth, notifications, image_upload) to simplify integration.

- Managed authentication flow using Firebase Admin SDK and custom tokens.

- Implemented notification logic that prevents self-notifications and handles multiple event types.

- Set up scalable structure for future moderation and content-recommendation systems.

***Challenges:***

- Handling cross-platform environment variables (React, Flutter, and FastAPI needed distinct setups).

- Ensuring schema compatibility between MySQL tables and SQLAlchemy models.

- Implementing robust foreign-key relationships without breaking the ORM layer.

- Structured and optimized relational schemas for core entities (users, comments, reposts, likes, etc.), maintaining consistent data relationships and enabling reliable communication between backend services and frontend components.

***Outcome***

ArtBook demonstrates a production-style full-stack workflow: authentication, API design, data modeling, media handling, and cross-platform delivery.

It serves as both a technical case study and a real-world example of scalable app architecture for social platforms.

Plus it was alot of fun. 😉


***Links***

Repository: [ArtBook GitHub](https://github.com/Court247/ArtBook)

Tech Docs: README.md


### 🏦 Banking Web App

***Overview***

The Bank Web App is a full-stack financial management platform built with React and Spring Boot as a monorepo.
Its goal is to simulate essential banking operations such as account creation, user authentication, and transaction management, while demonstrating a clean separation between frontend (React) and backend (Spring Boot) architectures.

Currently in early development, this project serves as a foundation for secure, scalable financial web systems, focusing on RESTful design, modular structure, and seamless client-server communication.

***Core Features (Planned & Implemented)***
- User Interface (React):
Responsive frontend built with React and TypeScript, providing form handling and component-based views.

- RESTful API (Spring Boot):
A backend service that handles requests from the frontend, processes data, and returns responses via REST endpoints.

- Authentication System (Planned):
Secure login and account creation using JWT or Spring Security.

- Account Management (Planned):
View balances, track transactions, and simulate deposits or withdrawals.

- Data Persistence (Planned):
Integration with a relational database (MySQL or PostgreSQL) through Spring JPA.

***Tech Stack***
| Layer                  | Technology                              |
| ---------------------- | --------------------------------------- |
| **Frontend**           | React · TypeScript · Node.js · HTML/CSS |
| **Backend**            | Spring Boot · Java · Maven              |
| **Build Tools**        | npm · Maven                             |
| **Architecture**       | REST API · MVC                          |
| **Database (Planned)** | MySQL or PostgreSQL                     |

***My Role & Focus***

This project is an independent build where I am responsible for designing both the client and server layers, including:

- Structuring a modular React frontend with reusable components.
- Creating a Spring Boot API with endpoints for user and transaction data.
- Managing local environment setup with separate ports for client (3000) and server (8080).
- Preparing the system for integration with authentication and database persistence layers.

***Architecture Overview***
```
my-react-springboot-app/
├── client/          # React Frontend
│   ├── src/
│   │   ├── components/   # UI Components
│   │   ├── pages/        # Page Views
│   │   └── services/     # API calls
│   └── package.json
└── server/          # Spring Boot Backend
    ├── src/main/java/com/example/
    │   ├── controller/   # REST Controllers
    │   ├── model/        # Entities
    │   └── service/      # Business Logic
    └── pom.xml

```
***Learning Objectives***

This project is part of my ongoing effort to:

- Strengthen my Java + Spring Boot backend skills.
- Improve full-stack communication between React and Java services.
- Explore authentication, error handling, and API best practices.
- Prepare for database integration and deployment to the cloud.
- Improve capabilities in created RESTful API and having them communicate with front-end services like React. 

***Next Steps***

- Implement Spring Security for authentication
- Connect to MySQL for persistent data storage
- Add frontend transaction tracking dashboard
- Deploy the application using Docker or Render

***Outcome (So Far)***

Even at its early stage, the Bank Web App demonstrates a working React frontend communicating with a Spring Boot backend, proving my ability to integrate two different frameworks into one consistent stack — a key full-stack developer skill.

***Links***

- Repository: [Bank Web App (React + Spring Boot)](https://github.com/Court247/BankWebApp)
- Tech Stack: React · Spring Boot · TypeScript · Java
- Status: 🚧 In Development

### 🌟 TopTier

***Overview***
TopTier is a mobile app built with Flutter that helps users explore and compare character rankings and gear setups from popular gacha-style RPGs.
Originally developed as a practice project, it evolved into a well-structured reference tool integrating curated data and Firestore-backed content.

***Core Features***
- Character Browser — view hero rankings and key stats.
- Gear Recommendations — quick reference for optimal builds.
- Favorites System — mark and track preferred characters.
- Cloud Integration — Firestore-backed dataset with restricted access for testing.
- Modular Widgets — cleanly separated UI components and providers.


***Tech Stack***

| Category             | Tools                         |
| -------------------- | ----------------------------- |
| **Framework**        | Flutter (Dart)                |
| **State Management** | Provider (ChangeNotifier)     |
| **Database**         | Firebase Firestore            |
| **Platform**         | Android (emulator + physical) |


***What I Built & Learned***

TopTier was designed to help me deepen my understanding of state management, modular UI design, and real-world app structure in Flutter.

I implemented:

- A reusable `FavoritesProvider` class to manage in-memory user preferences.

- A tier-list browsing system with character cards and detail modals.

- Firestore integration with environment variable–based credentials for secure reads.

- Error handling, responsive layouts, and incremental UI updates using ChangeNotifier.

Through this project, I learned how to structure production-style Flutter apps, manage multiple environments, and prototype fast with Firebase integrations.

***Challenges & Takeaways***

- Managing Firestore security rules without exposing data publicly.

- Handling async state updates in complex widget trees.

- Creating a maintainable UI pattern that could scale if persisted data was added later.

- Implemented a system to streamline database updates by automating JSON data integration, reducing manual input when adding new characters.

TopTier taught me how to write and the importance of clean, modular Flutter code, and how to think about scalability even in small, experimental apps.

***Visual Preview***

<p align="center"> <img src="https://github.com/user-attachments/assets/ede20d23-9ab4-4e87-ba4c-5d427e208f97" width="200" height="355" alt="TopTier Screenshot 1" /> <img src="https://github.com/user-attachments/assets/e013f100-07d6-4cfc-821b-a491e8e4330d" width="200" height="355" alt="TopTier Screenshot 2" /> <img src="https://github.com/user-attachments/assets/554f46fa-1ab7-41f4-b166-fe76fe1d6e67" width="200" height="355" alt="TopTier Screenshot 3" /> </p>

***Outcome***

TopTier serves as a hands-on example of Flutter app design, data handling, and integration with Firebase.
It’s an ongoing experiment that combines UI design, data modeling, and mobile performance optimization — a key part of my growth in mobile development.

***Links***

Repository: [TopTier GitHub](https://github.com/Court247/TopTier2)

Contact: courtney.woodsjobs@gmail.com

### 🛡️ Lightweight Intrusion Detection System
***Overview:***

The Lightweight Intrusion Detection System (LIDS) was developed for the DEVCOM Analysis Center (DAC) to assist cyber analysts in performing Cyber Vulnerability Assessments (CVAs).
The project’s goal was to design a resource-efficient intrusion detection system capable of identifying and reporting malicious network activity without the heavy overhead of traditional IDS tools.

Unlike typical enterprise IDS solutions, LIDS minimizes dependencies and CPU load, making it suitable for lightweight deployments and constrained environments.

***System Architecture***

LIDS is composed of three integrated subsystems (agents) that collectively monitor, analyze, and report malicious network behavior:

| Agent                               | Description                                                                                                                                                |
| ----------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **LIDS Agent**                      | Local detection unit that monitors network packets on an analyst’s machine, detects intrusions, stores logs, and forwards alerts to the distributed agent. |
| **Lightweight Network IDS (LNIDS)** | Network-level agent that monitors traffic on a SPAN port, stores packets, and relays alerts to LIDS-D.                                                     |
| **LIDS-D (Distributed Agent)**      | Central aggregation server that receives alerts from multiple agents, stores data, and provides analysts with visualization and review capabilities.       |

Together, these agents form a distributed lightweight IDS framework that supports both CLI and GUI interfaces for flexibility in deployment.

***Core Features***

- Real-time detection of malicious network interactions
- Multi-agent communication between LIDS, LNIDS, and LIDS-D
- Low resource consumption and minimal dependencies
- Local and remote data storage for alerts and packet logs
- Dual interfaces — Command Line (CLI) and Graphical (GUI)
- Configurable whitelist system for safe-listed IPs and nodes
- Analyst dashboard for viewing network activity, alerts, and known vs. unknown devices

***Tech Stack***

| Layer                        | Technology                       |
| ---------------------------- | -------------------------------- |
| **Backend / Logic**          | Python 3.10                      |
| **Web Framework**            | Flask 2.0                        |
| **Frontend GUI**             | React 18                         |
| **Network Tools**            | Scapy · PyShark · Netifaces      |
| **Security & Parsing**       | Cryptography · DefusedXML        |
| **Visualization**            | Tabulate · JSON/XML parsing      |
| **Virtualization / Testing** | Docker · VMware · Linux Lite 6.6 |


***My Role & Contributions***

As part of Team #4: Code of Duty, my focus areas included:
- Developing Python modules for packet capture, parsing, and alert generation
- Implementing communication logic between LIDS agents and the LIDS-D distributed node
- Assisting in GUI component development and alert visualization using React and Flask
- Collaborating on Docker-based test environments to simulate multi-node networks
- Documenting installation, testing, and troubleshooting for deployment in lab environments

***Development & Testing***

- Implemented Docker-based network simulations to emulate analyst, attacker, and server nodes.
- Used Wireshark-compatible packet captures for validation via PyShark and Scapy.
- Validated detection accuracy under constrained resources to meet “lightweight” requirements.

***Challenges & Solutions***

| Challenge                                             | Solution                                                                |
| ----------------------------------------------------- | ----------------------------------------------------------------------- |
| Reducing processing overhead during packet inspection | Optimized Scapy and PyShark packet parsing with multithreading          |
| Secure inter-agent communication                      | Implemented encrypted socket channels via the `cryptography` module     |
| Visualizing multi-agent data in real time             | Built a React-based dashboard integrated with Flask for alert streaming |

***GUI Overview***

- ***Dashboard:*** Displays alerts by level, time, IP, port, and description
- ***Network Map:*** Shows known and unknown devices in real time
- ***Alerts View:*** Lists triggered detections and network anomalies
- ***Settings Page:*** Configures connections and restarts agents on update

***Outcome***

LIDS provides a functional proof-of-concept for a distributed, lightweight IDS that can detect malicious traffic across nodes with minimal resource consumption.
The project demonstrated my ability to work in a multi-disciplinary cybersecurity environment, integrating networking, software engineering, and visualization — while effectively collaborating and communicating within a diverse development team.

***Project Details***
- ***Team:*** Code of Duty (8 members)
- ***Role:*** Developer / Network Logic Contributor
- ***Client:*** DEVCOM Analysis Center (DAC)
- ***Tools:*** Python · Flask · React · Docker · VMware · Linux Lite
- ***Date:*** November 2023
- ***Link:*** [Lightweight Intrusion Detection System (Private Repo)](https://github.com/ChristianAlbertoGomez/CS4311_LIDS_4CodOfDuty_Fall2023)


## 🧰 Skills & Tools
***Languages***

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=openjdk&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-003B57?style=for-the-badge&logo=sqlite&logoColor=white)

***Frameworks & Libraries***

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)

***Databases & Backend Tools***

![MySQL](https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Firestore](https://img.shields.io/badge/Firestore-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![REST_API](https://img.shields.io/badge/REST_API-02569B?style=for-the-badge&logo=fastapi&logoColor=white)

***Dev Tools & Environments***

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![VMware](https://img.shields.io/badge/VMware-607078?style=for-the-badge&logo=vmware&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Android Studio](https://img.shields.io/badge/Android_Studio-3DDC84?style=for-the-badge&logo=androidstudio&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-0078D4?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

***Security & Networking***

![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![PyShark](https://img.shields.io/badge/PyShark-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scapy](https://img.shields.io/badge/Scapy-FFCC00?style=for-the-badge&logo=python&logoColor=black)
![Cryptography](https://img.shields.io/badge/Cryptography-4B8BBE?style=for-the-badge&logo=python&logoColor=white)
![Network_Security](https://img.shields.io/badge/Network_Security-006400?style=for-the-badge&logo=databricks&logoColor=white)

***Design & Frontend Tools***

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)

***Testing & Development***

![Unit Testing](https://img.shields.io/badge/Unit_Testing-6DB33F?style=for-the-badge&logo=junit5&logoColor=white)
![CI/CD](https://img.shields.io/badge/CI/CD-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Testing](https://img.shields.io/badge/Testing-Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

## 🌱 Currently Learning

- ***FastAPI*** for building modern, high-performance backend applications

- ***RESTful API*** design and integration across multiple services

- ***Spring Boot*** for scalable enterprise-level backend development

- ***API creation and routing*** within FastAPI and Spring Boot frameworks

- ***Connecting React frontends*** to backend APIs and routers for full-stack communication

## About Me

I’m a Full-Stack Software Engineer with a B.S. in Computer Science and a minor in Mathematics from the University of Texas at El Paso.
I’m passionate about designing and building scalable web and mobile applications, with a strong focus on backend architecture, API development, and full-stack integration.

I enjoy solving real-world problems through code, collaborating with others to bring ideas to life, and continuously learning new technologies.
When I’m not coding, you can usually find me gaming 🎮 or brainstorming my next project idea.

## Connect with me
- [💼 LinkedIn](https://www.linkedin.com/in/courtney-woods-1a1b5883/)  
- [📧 Email](mailto:courtney.woodsjobs@gmail.com)  
- [🌐 Portfolio (coming soon)](https://courtneywoods.me)