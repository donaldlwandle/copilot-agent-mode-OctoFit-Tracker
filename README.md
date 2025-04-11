# Build applications with GitHub Copilot agent mode

<!-- ![](https://github.com/donaldlwandle/copilot-agent-mode-OctoFit-Tracker/actions/workflows/0-start-course.yml/badge.svg?branch=main) -->
<img src="https://github.com/user-attachments/assets/8c45e716-1d95-473b-8923-dbbbf0f924b2" alt="octofit-tracker-app" width="30%" height="30%"/>

_Build an application with GitHub Copilot agent mode in less than an hour._

### Pull Request Summary: OctoFit Tracker Project

#### Overview:
This pull request introduces the **OctoFit Tracker** application, a fitness tracking platform designed for Mergington High School. The project is inspired by the Monafit Tracker app and includes a backend built with Django and a frontend developed using React. The app enables users to log activities, view leaderboards, manage teams, and track workouts.

---

#### Key Features:
1. **Backend (Django)**:
   - **Database Integration**: MongoDB is used as the database, configured via `djongo`.
   - **REST API**: Endpoints for users, teams, activities, leaderboard, and workouts.
   - **Management Command**: A `populate_db.py` script to seed the database with test data.
   - **CORS Support**: Configured to allow cross-origin requests from the frontend.
   - **Settings**: Includes environment-specific configurations for codespace URLs and localhost.

2. **Frontend (React)**:
   - **Components**: Includes `Activities`, `Leaderboard`, `Teams`, `Users`, and `Workouts` components.
   - **Navigation**: A Bootstrap-styled navigation menu for seamless navigation between components.
   - **Styling**: Enhanced UI with Bootstrap tables, buttons, headings, and modals.
   - **API Integration**: Fetches data from the Django backend using the codespace URL.

3. **Styling**:
   - **App.css**: Custom styles for background, text, tables, buttons, headings, links, and navigation menu.
   - **Logo and Favicon**: Added the `octofitapp-small` logo and a favicon for branding.

4. **Project Structure**:
   - **Backend**: Organized under backend with Django apps and management commands.
   - **Frontend**: Organized under frontend with React components and public assets.

---

#### Changes Made:
1. **Backend**:
   - Configured MongoDB in `settings.py`.
   - Created models, serializers, views, and URLs for core entities.
   - Added a `populate_db.py` script to seed the database with test data.
   - Updated `views.py` to use the codespace URL for API endpoints.

2. **Frontend**:
   - Created React components for `Activities`, `Leaderboard`, `Teams`, `Users`, and `Workouts`.
   - Integrated Bootstrap for styling and navigation.
   - Updated `App.js` to include a navigation menu and routes for all components.
   - Styled the app using `App.css` with custom colors and layouts.

3. **Assets**:
   - Added the `octofitapp-small` logo and favicon to the public directory.
   - Updated `index.html` to include the logo and favicon.

---

#### How to Test:
1. **Backend**:
   - Activate the Python virtual environment: `source octofit-tracker/backend/venv/bin/activate`.
   - Run migrations: `python3 manage.py makemigrations && python3 manage.py migrate`.
   - Seed the database: `python3 manage.py populate_db`.
   - Start the server: `python3 manage.py runserver 0.0.0.0:8000`.

2. **Frontend**:
   - Navigate to frontend.
   - Install dependencies: `npm install`.
   - Start the development server: `npm start`.

3. **Verify**:
   - Access the app at `http://127.0.0.1:8000/` or the codespace URL.
   - Test API endpoints using `curl` or Postman.
   - Navigate through the React app and verify data is fetched and displayed correctly.

---

#### Notes:
- The project is fully functional and styled for a seamless user experience.
- Future enhancements could include authentication, activity filters, and additional analytics.

Let me know if you need further details or adjustments!

[Review the GitHub status page](https://www.githubstatus.com/)

&copy; 2025 GitHub &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT License](https://gh.io/mit)
