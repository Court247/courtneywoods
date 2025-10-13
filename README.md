# 👋 Hi! I'm Courtney Woods

Full stack developer passionate about art, gaming, design, and scalable applications. 

## 📑 Table of Contents

1. 🚀 [Featured Projects](#-featured-projects)
    - [ArtBook](#-artbook)
    - [Bank Web App](#banking-web-app)
    - [TopTier](#toptier)
    - [Lightweight Intrusion Detection System](#lightweight-intrusion-detection-system)
    - [Flavor App](#flavor-app)
2. 🧰 [Skills & Tools](#skills)
3. 🌱 [Currently Learning]()
4. 💬 [About Me](#about-me)
5. 📫 [Contact](#contact)


## 🚀 Featured Projects

### 🎨 Artbook

***Overview:***

ArtBook is a full-stack social media application designed to give artists a space to share their work, connect with others, and build creative communities. Built as a monorepo, it integrates web, mobile, and backend services into one cohesive ecosystem.

***🧠 Key Features***

- User-generated content — artists can upload, caption, and share artwork.

- Comments & Likes — engagement features built into both posts and comments.

- Reposts & Follows — users can repost or quote-share art and follow other creators.

- Notifications — real-time alerts for likes, comments, follows, and reposts.

- Reporting & Admin Controls — moderation tools for safe, community-driven spaces.

- Cross-platform — single backend serving React (web) and Flutter (mobile) apps.

***🧩Tech Stack***
| Layer              | Technology                       |
| ------------------ | -------------------------------- |
| **Backend**        | FastAPI (Python)                 |
| **Frontend (Web)** | React (JavaScript)               |
| **Mobile**         | Flutter (Dart)                   |
| **Database**       | MySQL (SQLAlchemy ORM)           |
| **Auth & Media**   | Firebase Auth & Firebase Storage |

***⚙️ Architecture & Approach***

ArtBook is structured as a monorepo to maintain consistency and shared logic across platforms.

- Backend (FastAPI) — Handles REST API endpoints for users, posts, comments, and more. Firebase tokens are validated server-side for secure access.

- Frontend (React) — A responsive web interface for browsing, posting, and engaging with content.

- Mobile (Flutter) — Offers native performance and UI parity with the web experience.

- Database Layer (MySQL) — Normalized schema ensuring efficient relations between posts, users, comments, and notifications.

***🧪 My Role & Challenges***

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

***💡 Outcome***

ArtBook demonstrates a production-style full-stack workflow: authentication, API design, data modeling, media handling, and cross-platform delivery.

It serves as both a technical case study and a real-world example of scalable app architecture for social platforms.

Plus it was alot of fun. 😉


***🔗 Links***

Repository: [ArtBook GitHub](https://github.com/Court247/ArtBook)

Tech Docs: README.md


### [Banking Web App](https://github.com/Court247/BankWebApp)

### 🌟 TopTier

***Overview***
TopTier is a mobile app built with Flutter that helps users explore and compare character rankings and gear setups from popular gacha-style RPGs.
Originally developed as a practice project, it evolved into a well-structured reference tool integrating curated data and Firestore-backed content.

***✨ Core Features***

- Character Browser — view hero rankings and key stats.

- Gear Recommendations — quick reference for optimal builds.

- Favorites System — mark and track preferred characters.

- Cloud Integration — Firestore-backed dataset with restricted access for testing.

- Modular Widgets — cleanly separated UI components and providers.


***🧰 Tech Stack***

| Category             | Tools                         |
| -------------------- | ----------------------------- |
| **Framework**        | Flutter (Dart)                |
| **State Management** | Provider (ChangeNotifier)     |
| **Database**         | Firebase Firestore            |
| **Platform**         | Android (emulator + physical) |


***🧠 What I Built & Learned***

TopTier was designed to help me deepen my understanding of state management, modular UI design, and real-world app structure in Flutter.

I implemented:

A reusable FavoritesProvider class to manage in-memory user preferences.

A tier-list browsing system with character cards and detail modals.

Firestore integration with environment variable–based credentials for secure reads.

Error handling, responsive layouts, and incremental UI updates using ChangeNotifier.

Through this project, I learned how to structure production-style Flutter apps, manage multiple environments, and prototype fast with Firebase integrations.

***🧭 Challenges & Takeaways***

Managing Firestore security rules without exposing data publicly.

Handling async state updates in complex widget trees.

Creating a maintainable UI pattern that could scale if persisted data was added later.

“TopTier taught me how to write clean, modular Flutter code — and how to think about scalability even in small, experimental apps.”

***📱 Visual Preview***

<p align="center"> <img src="https://github.com/user-attachments/assets/ede20d23-9ab4-4e87-ba4c-5d427e208f97" width="300" height="533" alt="TopTier Screenshot 1" /> <img src="https://github.com/user-attachments/assets/e013f100-07d6-4cfc-821b-a491e8e4330d" width="300" height="533" alt="TopTier Screenshot 2" /> <img src="https://github.com/user-attachments/assets/554f46fa-1ab7-41f4-b166-fe76fe1d6e67" width="300" height="533" alt="TopTier Screenshot 3" /> </p>

***🚀 Outcome***

TopTier serves as a hands-on example of Flutter app design, data handling, and integration with Firebase.
It’s an ongoing experiment that combines UI design, data modeling, and mobile performance optimization — a key part of my growth in mobile development.

***🔗 Links***

Repository: [TopTier2 GitHub](https://github.com/Court247/TopTier2)

Contact: courtney.woodsjobs@gmail.com

### [Lightweight Intrusion Detection System](https://github.com/ChristianAlbertoGomez/CS4311_LIDS_4CodOfDuty_Fall2023)

### [Flavor App](https://github.com/cmalcazar/FlavorApp)

## 🧰 Skills & Tools
![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/-React-61DAFB?logo=react&logoColor=black)
![Firebase](https://img.shields.io/badge/-Firebase-FFCA28?logo=firebase&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-336791?logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/-Git-F05032?logo=git&logoColor=white)

## Currently Learning

## About Me

I am a full stack software engineer. Recently graduated with my degree in Computer Science and a minor in math from the University of Texas at El Paso. I enjoy playing video games on my downtime or thinking up real world projects to work on.

I'm passionate about creating scalable web apps and mobile applications. 

## Contact