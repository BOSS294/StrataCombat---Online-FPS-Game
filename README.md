##  Stratacombat Build 0.1 (Beta) Documentation

Welcome to the **Stratacombat** Build 0.1 (Beta) documentation. This build focuses exclusively on creating and refining the **UI/UX** for core lobby systems, player skins, account creation flows, and foundational database integration—laying the groundwork for future gameplay features.

## Introduction
Stratacombat is a web-based tactical round-based FPS emphasizing strategy and coordination. Build 0.1 (Beta) is dedicated to crafting the **front-end and back-end plumbing** for our foundational systems before implementing core gameplay mechanics.

##  Version Overview & Scope
- **Version**: 0.1 (Beta)
- **Release Date**: TBD
- **Status**: UI/UX prototype with back-end connectivity
- **Scope**:
  - Lobby interface design with multiple skin themes  
  - User account creation, login, and profile management  
  - MySQL database integration via phpMyAdmin for storing user data  
  - Placeholder matchmaking logic (UI only)

##  Initial UI/UX Features (Brief)
1. **Lobby Screen & Skins**: Responsive lobby page with theme selector (e.g., neon, modern, camo).  
2. **Account Creation & Login**: Registration form, email validation, password strength indicator, login page.  
3. **Profile Dashboard**: Display username, selected skin, basic stats placeholder.  
4. **Database Connectivity**: PHP scripts to create/read user records in MySQL via phpMyAdmin.  
5. **Navigation & Layout**: Consistent header, footer, and side menu components.

## Feature Details

### 1. Lobby UI/UX & Skins
- **Description**: Interactive lobby page where players wait for matches, chat, and choose visual themes.
- **Components**:
  - Theme selector dropdown (3 skins: neon, camo, digital)  
  - Chat box UI (front-end placeholder)  
  - Player list panel showing online users  
- **Flow**:
  1. User lands on `/lobby.html`  
  2. Chooses a skin → CSS variables update dynamically  
  3. Chat and ready-up buttons appear (non-functional for this build)

### 2. Account Creation & Authentication
- **Description**: Secure sign-up and sign-in flows to manage player credentials.
- **Components**:
  - Registration form: username, email, password, confirm password  
  - Login form: email, password  
  - Client-side validation: required fields, email format, password strength meter  
- **Flow**:
  1. User visits `/register.html`  
  2. Completes form → JS validation  
  3. Data POSTed to `register.php` → DB insert  
  4. Redirect to `/login.html` upon success


## Technical Architecture & Tech Stack
- **Frontend**: HTML5, CSS3 (Flexbox & CSS variables for theming), JavaScript (ES6)  
- **Backend**: PHP 8.x with PDO for secure DB interactions  
- **Database**: MySQL managed via phpMyAdmin  

## Next Steps & Roadmap
- **Build 0.2**: Integrate real-time lobby chat and basic matchmaking API  
- **Build 0.3**: Expand skin library and allow custom uploads  
- **Build 1.0**: Introduce core combat UI, match flow, and deploy voice chat  

