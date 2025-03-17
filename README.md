# MovieMate

**MovieMate** is a modern, responsive movie directory application built with React, Vite, and Tailwind CSS. Powered by the TMDB (The Movie Database) API, MovieMate allows users to browse movies, view detailed information, and discover new cinematic favorites. Whether you're a movie enthusiast or just looking for your next watch, MovieMate offers a fast and intuitive experience.

Live Demo: [https://Arnav400.github.io/MovieMate](https://Arnav400.github.io/MovieMate)

## Features

- **Movie Exploration**: Browse popular, trending, and upcoming movies from the TMDB API.
- **Detailed Views**: Access movie details like synopsis, release date, ratings, and posters.
- **Responsive Design**: Enjoy a seamless experience across desktop, tablet, and mobile devices with Tailwind CSS.
- **Fast Development**: Built with Vite for lightning-fast builds and hot module replacement (HMR).
- **Optional Backend**: Integrates with Appwrite for user authentication and data persistence (optional).
- **Deploy Anywhere**: Easily deployable to GitHub Pages or other static hosting platforms.

## Tech Stack

- **Frontend**: React 18.3.1
- **Build Tool**: Vite 6.0.5
- **Styling**: Tailwind CSS (via `@tailwindcss/vite` 4.0.3)
- **API**: [TMDB API](https://www.themoviedb.org/documentation/api)
- **Backend (Optional)**: Appwrite 17.0.0
- **Utilities**: React-Use 17.6.0
- **Linting**: ESLint 9.17.0 with React, React Hooks, and React Refresh plugins
- **Deployment**: GitHub Pages (via `gh-pages` 6.3.0)

## Prerequisites

To run MovieMate locally, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v18 or higher recommended)
- [npm](https://www.npmjs.com/) (v9 or higher), or alternatively [pnpm](https://pnpm.io/) / [yarn](https://yarnpkg.com/)
- A [TMDB API Key](https://www.themoviedb.org/documentation/api) (sign up for free to obtain one)

## Installation

Follow these steps to set up MovieMate on your local machine:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Arnav400/MovieMate.git
   cd MovieMate
Install Dependencies:
bash

Collapse

Wrap

Copy
npm install
Configure Environment Variables:
Create a .env file in the root directory.
Add your TMDB API key:
text

Collapse

Wrap

Copy
VITE_TMDB_API_KEY=your_tmdb_api_key_here
Replace your_tmdb_api_key_here with your actual TMDB API key.
Start the Development Server:
bash

Collapse

Wrap

Copy
npm run dev
Open your browser and navigate to http://localhost:5173 to see MovieMate running.
Configuration
TMDB API: Ensure your API key is valid and has sufficient rate limits for your use case.
Appwrite (Optional):
Install the Appwrite SDK if you plan to use backend features.
Configure your Appwrite instance in src (e.g., in a config file or service):
javascript

Collapse

Wrap

Copy
import { Client } from 'appwrite';
const client = new Client()
  .setEndpoint('YOUR_APPWRITE_ENDPOINT')
  .setProject('YOUR_PROJECT_ID');
Update .env with Appwrite credentials if needed.
Available Scripts
In the project directory, you can run:

npm run dev: Starts the development server with hot reloading.
npm run build: Builds the app for production into the dist folder.
npm run preview: Serves the production build locally for testing.
npm run lint: Runs ESLint to enforce code quality and consistency.
npm run predeploy: Prepares the app for deployment by building it.
npm run deploy: Deploys the app to GitHub Pages.
Project Structure
text

Collapse

Wrap

Copy
MovieMate/
├── dist/              # Production build output
├── src/              # Source code
│   ├── main.jsx      # React entry point
│   └── ...           # Components, hooks, and utilities
├── public/           # Static assets (e.g., favicon)
├── .env              # Environment variables (not tracked by Git)
├── .gitignore        # Files and folders ignored by Git
├── eslint.config.js  # ESLint configuration
├── index.html        # HTML entry point
├── package.json      # Project metadata and dependencies
├── vite.config.js    # Vite configuration
└── README.md         # Project documentation
Usage
Launch the app with npm run dev.
Browse the movie catalog fetched from TMDB.
Click a movie to view its details.
Enjoy the clean, responsive UI styled with Tailwind CSS.
Deployment
MovieMate is pre-configured for GitHub Pages deployment:

Set Homepage:
Update the homepage field in package.json to your GitHub Pages URL:
json

Collapse

Wrap

Copy
"homepage": "https://yourusername.github.io/MovieMate"
Deploy:
bash

Collapse

Wrap

Copy
npm run deploy
The app will be built and pushed to the gh-pages branch.
Verify: Visit your GitHub Pages URL (e.g., https://yourusername.github.io/MovieMate).
For other hosting platforms, simply upload the contents of the dist folder after running npm run build.

Troubleshooting
API Key Issues: Ensure your TMDB API key is correctly set in .env and that it’s not expired.
Build Errors: Run npm install again to ensure all dependencies are installed.
CORS Errors: If fetching TMDB data fails, verify your API key and network settings.
Deployment Fails: Check your GitHub Pages settings and ensure the gh-pages branch is correctly configured.
Roadmap
 Add search functionality for movies.
 Implement user authentication with Appwrite.
 Allow users to save favorite movies.
 Add support for TV shows from TMDB.
 Enhance accessibility (a11y) compliance.
Contributing
We welcome contributions! To get started:

Fork the repository.
Create a feature branch (git checkout -b feature/your-feature-name).
Commit your changes (git commit -m "Add your feature").
Push to your branch (git push origin feature/your-feature-name).
Open a Pull Request.
Please adhere to the ESLint rules in eslint.config.js and include a description of your changes.

License
This project is licensed under the MIT License.

Acknowledgments
TMDB for their amazing movie data API.
Vite for a blazing-fast development experience.
Tailwind CSS for utility-first styling.
React for a powerful UI library.
Appwrite for open-source backend support.
Contact
Created by Arnav400. For questions, suggestions, or collaboration, feel free to open an issue or reach out via GitHub.

Happy movie browsing with MovieMate!
