# Hospital Management System Deployment Plan

## Information Gathered
- **Backend**: Spring Boot app with MySQL database (localhost:3306, user: root, pass: root), exposes /auth/signup and /auth/login on port 8081. Uses JWT for auth.
- **Frontend**: React (Vite) app on port 5173, consumes backend APIs for login/signup, displays dashboard with hospital modules.
- **Environment**: Windows 11, repos cloned in d:/hospital-management-system (hospital-backend-jenkins and hospital-frontend folders).
- **Dependencies**: MySQL needs to be running; backend requires Maven; frontend requires Node.js/npm.
- **Jenkins**: Jenkinsfile present for CI/CD, needs GitHub repo URL updated to user's (https://github.com/Madireddysaikrishna/hospital-managment-system.git).
- **User's Repo**: Provided link for pushing code.

## Plan
1. **Setup Database**: Ensure MySQL is installed and running on localhost:3306 with root/root credentials.
2. **Run Backend**: Navigate to hospital-backend-jenkins, run Spring Boot app on port 8081.
3. **Run Frontend**: Navigate to hospital-frontend, install dependencies, run Vite dev server on port 5173.
4. **Verify Functionality**: Use browser to test signup, login, and dashboard access.
5. **Update Jenkinsfile**: Replace placeholder GitHub URL with user's repo link.
6. **Push to Git**: Set remote for backend repo to user's GitHub repo and push code.
7. **Submit Link**: Provide the GitHub repo link after push.

## Dependent Files/Steps
- MySQL service start.
- Backend: pom.xml for Maven build.
- Frontend: package.json for npm install.
- Jenkinsfile update for CI/CD.

## Followup Steps
- Test full flow locally.
- Push code to GitHub.
- If Jenkins deployment needed, configure Jenkins with updated Jenkinsfile.
