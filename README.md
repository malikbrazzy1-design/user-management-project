# User Management Portal

## Setup on Windows with XAMPP
1. Start Apache and MySQL in XAMPP Control Panel.
2. Open http://localhost/phpmyadmin, select the SQL tab, paste the contents of `sql.txt`, and click Go.
3. Extract this project into `C:\xampp\htdocs\user_management_project`.
4. In `Backend`, rename `dotenv` to `.env` (Windows command: `ren dotenv .env`). Update database credentials if needed.
5. In Command Prompt: `cd C:\xampp\htdocs\user_management_project\Backend`, then `npm install`, then `npm start`. Leave this terminal open.
6. Open http://localhost/user_management_project/Frontend/index.html.
7. Register an account, log in, and demonstrate all eight search modes (requirements 3-10).

## Security
All SQL values are parameterized using mysql2 prepared statements. Passwords are hashed with bcryptjs before storage and compared with bcryptjs on login. Password hashes are not included in search results. This is a classroom demo, not a production authentication system (no sessions or protected routes).

## GitHub partner demo
One partner creates the remote repository and pushes the project. The other partner clones it, changes the README or a style, commits, and pushes. The first partner runs `git fetch`, `git pull`, and shows the updated file. Do not commit `.env` or node_modules.

## Demo tip
`john` is dated 5 days ago, `sara` shares that date, `emma` is 2 days ago, and `alex` is today. Search after john, same day as john, never signed in, and today to demonstrate correct results. Register a new user to show live inserts and sign-in updates.

This project demonstrates user registration, secure login, database searches, and GitHub collaboration.
GitHub demonstration update.
Github demonstration update.
