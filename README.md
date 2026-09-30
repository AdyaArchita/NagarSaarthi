# NagarSaarthi ♻️
**AI-Powered Citizen-Centric Smart Urban Waste Management System**

## Overview
NagarSaarthi is an AI-driven platform developed for the **Smart India Hackathon 2025**. It enables citizens and municipal authorities to collaboratively manage urban waste through intelligent reporting and real-time insights. Citizens can report waste issues with images and interact with the EcoSort Chatbot, while municipal authorities can monitor hotspots and ensure faster resolutions—driving cleaner, smarter, and more sustainable cities.

## Live Demo & Screenshots
🔗 **Live Demo:** [https://adyaarchita.github.io/NagarSaarthi](https://adyaarchita.github.io/NagarSaarthi)
📦 **Repository:** [AdyaArchita/NagarSaarthi](https://github.com/AdyaArchita/NagarSaarthi)

> **TODO:** Add screenshots of the Citizen Dashboard, Report Issue page, and Municipality Dashboard here.

## Key Features
- **Citizen Dashboard:** A dedicated portal for citizens featuring profiles, impact metrics, and community initiatives.
- **Smart Waste Reporting:** Users can report waste issues (`ReportIssue` component) with images for tracking and resolution.
- **EcoSort Chatbot:** An integrated conversational assistant (`EcoSortChatbot`) to guide users on smart disposal and waste categorization.
- **Municipality & Admin Dashboards:** Dedicated views for municipal authorities to monitor waste hotspots and manage operations.
- **Interactive Maps:** Integration with Leaflet (`react-leaflet`) for visualizing waste reports geographically.

## Tech Stack
**Frontend:**
- [React (v18)](https://react.dev/) - UI library
- [Vite](https://vitejs.dev/) - Build tool and development server
- [Tailwind CSS](https://tailwindcss.com/) - Utility-first styling framework
- [React Router DOM](https://reactrouter.com/) - Navigation and routing
- [Framer Motion](https://www.framer.com/motion/) - UI animations
- [Leaflet / React Leaflet](https://react-leaflet.js.org/) - Interactive maps

**Tools & Linters:**
- [ESLint](https://eslint.org/) - Code linting

**Deployment:**
- [GitHub Pages](https://pages.github.com/) - Hosted via `gh-pages`

## Project Structure
```text
NagarSaarthi/
├── public/                 # Static assets
├── src/                    # Source code
│   ├── assets/             # Images and icons
│   ├── pages/              # React components for all routes
│   │   ├── Admin/          # Admin dashboard view
│   │   ├── Citizen/        # Citizen dashboard, metrics, and profiles
│   │   ├── Home/           # Landing page and EcoSort Chatbot
│   │   ├── Login/          # Authentication pages
│   │   ├── ReportIssue/    # Waste reporting interface
│   │   └── MunicipalityDashboard.jsx # Municipality view
│   ├── App.jsx             # Main routing component
│   ├── main.jsx            # React application entry point
│   ├── index.css           # Global Tailwind CSS imports
│   └── App.css             # Additional global styles
├── eslint.config.js        # ESLint configuration
├── package.json            # Dependencies and npm scripts
├── tailwind.config.js      # Tailwind CSS configuration
└── vite.config.js          # Vite configuration
```

## Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) (v16 or higher recommended)
- npm or yarn

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/AdyaArchita/NagarSaarthi.git
   cd NagarSaarthi
   ```
2. Install dependencies:
   ```bash
   npm install
   ```

### Running Locally
To start the development server:
```bash
npm run dev
```
The application will be available at `http://localhost:5173/` (or whichever port Vite assigns).

## Available Scripts
- `npm run dev`: Starts the Vite development server.
- `npm run build`: Builds the app for production into the `dist/` folder.
- `npm run preview`: Previews the production build locally.
- `npm run lint`: Runs ESLint to check for code issues.
- `npm run lint:fix`: Runs ESLint and automatically fixes fixable issues.
- `npm run deploy`: Builds the app and deploys the `dist/` folder to GitHub Pages.

## Usage / Architecture
The application is a Single Page Application (SPA) built with React and Vite. Routing is handled by `react-router-dom` in `App.jsx`.
- **Citizens** start at the Home page (`/`), can log in (`/login`), and access the Citizen Dashboard (`/dashboard`) to view impact metrics and report issues (`/reportissue`).
- **Authorities** have dedicated routes (`/admin-dashboard` and `/municipality-dashboard`) to monitor and address reported waste issues.
- **Global Components:** The `EcoSortChatbot` is available globally across most routes (except login and FAQs) to assist users.

## Deployment
This project is configured to be deployed on GitHub Pages. To deploy a new version, simply run:
```bash
npm run deploy
```
This script will automatically run the build process (`predeploy`) and push the `dist/` directory to the `gh-pages` branch.

## Customization
- **Theme & Colors:** Modify `tailwind.config.js` to extend or change the color palette.
- **Routing:** Add or remove pages in `src/App.jsx`.
- **Base URL:** If changing the hosting location, update the `base` property in `vite.config.js` and the `homepage` URL in `package.json`.

## Roadmap / Known Limitations
> **TODO:** Implement actual backend integration and AI classification APIs, as the current repository primarily contains the frontend implementation.
> **TODO:** Add unit and integration tests.

## Contributing
Contributions, issues, and feature requests are welcome!

## License
> **TODO:** Verify and specify the exact license (currently `ISC` in `package.json`, but a `LICENSE` file is missing).

## Author
> **TODO:** Add author contact details or portfolio links.
