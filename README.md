# Jules-Art-Portfolio
A self-hosted art portfolio website for my girlfriend :)

## Jules Art Portfolio - Website Architecture

### Tech Stack

Operating System - Ubuntu Server
Web Server - Nginx
Database - MySQL
Backend - Flask
Frontend framework - Vue.js 

### Front End Design

Page 1 : Landing page

- About me
-> Interests and Goals blurb
-> Link to Pinterest
-> Contact button

- Art Gallery
-> Favorites
-> For Sale
-> Other Works

- Vision Board (photos & links)
-> ** Capturing the aesthetic of Jules ** 

### File Hierarchy Setup
```
jules-vue-app/
├── .node_modules/       # Installed dependencies (git-ignored)
├── public/              # Static assets served directly to the root
│   └── favicon.ico      # Browser tab icon
├── src/                 # Main application source code
│   ├── assets/          # Static assets compiled by the bundler
│   │   ├── logo.svg     
│   │   └── main.css     # Global styles
│   ├── components/      # Reusable UI building blocks
│   │   ├── base/        # Generic components (buttons, inputs)
│   │   │   └── BaseButton.vue
│   │   └── common/      # Global layout blocks
│   │       ├── TheNavbar.vue
│   │       └── TheFooter.vue
│   ├── composables/     # Vue 3 Composition API stateful logic hooks
│   │   └── useAuth.js   
│   ├── router/          # Page routing configuration
│   │   └── index.js     
│   ├── stores/          # State management (Pinia or Vuex)
│   │   └── counter.js   
│   ├── views/           # Full-page components mapped to routes
│   │   ├── HomeView.vue 
│   │   └── AboutView.vue
│   ├── App.vue          # Root component of the application
│   └── main.js          # JavaScript entry point initializing Vue
├── .gitignore           # Specifies files untracked by Git
├── index.html           # Main HTML shell file
├── package.json         # Project metadata and dependencies script
├── README.md            # Project documentation
└── vite.config.js       # Bundler configuration settings
```