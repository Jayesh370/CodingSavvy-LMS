<div align="center"><img src="https://raw.githubusercontent.com/Jayesh370/CodingSavvy-LMS/main/public/assets/Final_Logo.png](https://raw.githubusercontent.com/Jayesh370/LMS-System-React/main/public/assets/Final_Logo.png)" alt="Coding Savvy Logo" width="200"/></div>📖 AboutCoding Savvy is a comprehensive educational platform designed to guide users through their entire coding journey—from writing their first line of code to landing a dream job in the tech industry.This is a Full-Stack MERN-style application with a React frontend and a robust Node.js/Express backend, designed for modern, fast, and interactive development.🚀 Getting StartedPrerequisitesBefore you begin, ensure you have the following installed:Node.js (v18 or higher) - Download herenpm or yarn - Package managerGit - Version controlInstallation & SetupClone the repositoryBashgit clone https://github.com/Jayesh370/LMS-System-React.git
cd LMS-System-React
Setup Frontend DependenciesThe frontend application lives in the root directory.Bash# Install dependencies for React/Vite
npm install
Setup Backend DependenciesThe backend server lives in the backend/ directory.Bashcd backend
# Install dependencies for Node.js/Express
npm install
Configure Environment VariablesThe backend requires environment configuration.Bash# From inside the backend/ folder:
cp .env.example .env
# Open the new .env file and adjust variables (e.g., PORT, DB connection)
(Note: The frontend uses environment variables managed by Vite, typically for VITE_API_URL.)▶️ Running Frontend and Backend TogetherThe application requires both the frontend client and the backend server to be running simultaneously.1. Start the Backend ServerOpen a separate terminal tab or window. Navigate to the backend/ directory and start the server:Bash# In Terminal 1 (from LMS-System-React/backend)
npm run dev
The server will be running on http://localhost:5000 (or the port defined in backend/.env).2. Start the Frontend ApplicationIn your original terminal tab, navigate back to the root of the project and start the React development server:Bash# In Terminal 2 (from LMS-System-React)
npm run dev
The application will open in your browser at http://localhost:5173.🛠️ Tech Stack💻 Frontend (Root Directory)TechnologyPurposeVersionReactCore Frontend Framework19.1.1ViteBuild Tool & Dev Server7.1.2React RouterClient-side Routing7.8.2BootstrapCSS Framework5.3.8AOSScroll Animations2.3.4React IconsIcon Library5.5.0Available ScriptsDescriptionnpm run devStarts the development server (http://localhost:5173)npm run buildBuilds the app for production (dist/ directory)npm run previewPreviews the production buildnpm run lintRun ESLint for code quality🗄️ Backend (backend/ Directory)TechnologyPurposeNode.jsJavaScript RuntimeExpressWeb Application FrameworkHelmetHTTP Header SecurityCORSCross-Origin Resource SharingMorganHTTP Request LoggingDotenvEnvironment Variable ManagementNodemonDevelopment Auto-ReloadAvailable ScriptsDescriptionnpm run devStart dev server with nodemon (http://localhost:5000)npm startStart production server📂 Directory StructureLMS-System-React/
├── backend/                  # Node.js/Express Server
│   ├── src/
│   │   ├── config/           # App configuration (e.g., database)
│   │   ├── controllers/      # Business logic implementation
│   │   ├── middlewares/      # Error/Async handlers
│   │   ├── models/           # Database schemas (Mongoose)
│   │   ├── routes/           # API endpoints definition
│   │   └── utils/            # Utility functions (logger, etc.)
│   ├── package.json
│   └── .env.example
├── public/                   # Static assets (including Final_Logo.png)
├── src/                      # React Source Code
│   └── ...                   # (Your React components, logic, etc.)
├── package.json              # Frontend dependencies and scripts
└── ...                       # Frontend config files (.env, vite.config.js, etc.)
🤝 ContributingWe welcome contributions! Please follow these steps:Fork the repository (No need if you're one of the collaborators)Create a feature branch (git checkout -b feature/AmazingFeature)Commit your changes (git commit -m 'Add some AmazingFeature')Push to the branch (git push origin feature/AmazingFeature)Open a Pull Request
