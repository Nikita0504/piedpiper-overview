# PiedPiper Chat

> ⚠️ **Project is under active development.** Most features are planned for implementation. Client applications are not yet developed.

A minimalist communication platform inspired by Discord, with an emphasis on a clean interface, modern stack, and extensibility. The application is designed for individual communication, messaging, calls, and basic profile customization.

## 📋 Project Description

PiedPiper Chat is a decentralized messaging and video calling system built on microservices architecture. The project uses a modern technology stack based on Kotlin and is designed with scalability and development convenience in mind.

## ✨ Key Features (Planned)

### 1. Authorization

- **Standard authentication** — login with username and password
- **OAuth integration** — login via Google account
- **Account linking** — ability to link multiple login methods to one user

### 2. Private Chats

- **Individual conversations** — create and manage private chats between two users
- **User statuses** — display current status (online, do not disturb, etc.)
- **Minimalist interface** — focus on simplicity and ease of use
- **Message history** — save and access complete conversation history

### 3. Calls

- **Audio and video calls** — between two participants in private chat
- **Smooth mode switching** — quick enable/disable of camera and microphone
- **Screen sharing** — ability to share screen with the other person
- **Camera streaming** — transmit video from device camera

### 4. Settings and Profile Customization

- **Profile editing** — change name, status, avatar
- **Custom image uploads** — free ability to upload your own pictures for profile decoration
- **Result preview** — preview profile appearance before publishing
- **Animated avatar support** — ability to use GIFs for animated profiles
- **Minimal settings** — functional privacy and notification management

## 🏗️ Project Architecture

The project consists of microservices, each responsible for a separate area of functionality:

### Microservices

- **[Auth Service](https://github.com/Nikita0504/piedpiper-auth-service)** — manages authorization, user authentication, and OAuth integration
- **[User Service](https://github.com/Nikita0504/piedpiper-user-service)** — manages user profiles, statuses, and settings
- **[Chat Service](https://github.com/Nikita0504/piedpiper-chat-service)** — processes private messages, manages conversation history, and WebSocket connections

Each microservice can scale independently and has its own database.

## 🛠️ Technology Stack

| Category | Technology | Description |
|----------|------------|-------------|
| **Language** | Kotlin (KMP) | Shared codebase for server and client logic |
| **Server** | Ktor | Asynchronous web server in Kotlin |
| **Communication** | WebRTC, WebSocket | For calls, streaming, and messaging |
| **Deployment** | Docker, Kubernetes | Containerization and orchestration |

### Why This Stack?

- **Kotlin Multiplatform (KMP)** — allows using shared code between mobile (Android/iOS), desktop, and web clients
- **Ktor** — lightweight and extensible framework for writing microservices in Kotlin
- **WebRTC** — standard for implementing audio/video calls and screen sharing
- **WebSocket** — protocol for real-time messaging with low latency
- **Docker and Kubernetes** — provide scalability, reliability, and ease of deployment

## 📦 Project Repositories

| Service | Repository | Status |
|---------|------------|--------|
| Auth Service | [piedpiper-auth-service](https://github.com/Nikita0504/piedpiper-auth-service) | 🚧 In development |
| User Service | [piedpiper-user-service](https://github.com/Nikita0504/piedpiper-user-service) | 🚧 In development |
| Chat Service | [piedpiper-chat-service](https://github.com/Nikita0504/piedpiper-chat-service) | 🚧 In development |

## 🚀 Getting Started

> ⚠️ **Documentation is being created**

### Requirements

- Kotlin 1.9+
- Docker and Docker Compose
- Java 17+

### Local Development

