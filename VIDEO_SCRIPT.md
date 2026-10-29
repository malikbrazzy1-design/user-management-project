# Demonstration video outline (5–8 minutes)

1. Introduce: “This is our user management application built using HTML, CSS, JavaScript, Express, and MySQL.” Show the webpage.
2. Show phpMyAdmin > web_app > Users. Explain primary key username, bcrypt password hash, registerday, and nullable signintime.
3. Register a NEW user with a unique username and password of 8+ characters. Refresh phpMyAdmin to show the inserted row.
4. Sign in using that NEW account. Show that the signintime column is updated. Try a wrong password and show rejection. Explain that `?` placeholders in prepared statements prevent SQL injection and bcrypt checks the hash.
5. Demonstrate each of the eight search modes. Use john for after/same day; search salary 40000–90000 and age 20–40. Show result counts and database rows.
6. Explain how each search maps to a SELECT statement in sql.txt (LIKE, BETWEEN, JOIN, IS NULL, CURDATE).
7. Show GitHub: first partner creates remote repository and pushes. Second partner clones, edits README, adds, commits, pushes. First partner fetches and pulls; show git log.
8. Finish by showing sql.txt and summarizing that all ten functions work.

NOTE: Only describe GitHub operations actually performed. Never commit .env or node_modules. Demo seed passwords are not guaranteed to be usable; use a freshly registered user for login.
