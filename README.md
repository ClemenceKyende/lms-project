# Learning Managment System

## Step 1: Project Setup

### Create a new directory for your project and navigate into it.
```bash
mkdir learning-management-app
cd learning-management-app
```
### Initialize a new Node.js project.
```bash
npm init -y
```
### Install necessary dependencies.
```bash
npm install express mysql ejs bcryptjs express-session express-validator
```

## Step 2: Set up the Backend

### Create a `server.js` file in your project directory.

### Create a MySQL database named `learning_management` 

#### Create users table
```bash
-- Create users table
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(255) UNIQUE,
    password VARCHAR(255),
    email VARCHAR(255) UNIQUE,
    full_name VARCHAR(255)
);
```

#### Create courses table
```bash
-- Create courses table
CREATE TABLE courses (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255)
);

-- Insert sample data into courses table
INSERT INTO courses (name) VALUES
('Introduction to HTML'),
('CSS Fundamentals'),
('JavaScript Basics');
```

#### Create leaderboard table
```bash
-- Create leaderboard table
CREATE TABLE leaderboard (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255),
    score INT
);

-- Insert sample data into leaderboard table
INSERT INTO leaderboard (name, score) VALUES
('John Doe', 100),
('Jane Smith', 90),
('Michael Brown', 85),
('Emily Jones', 80);
```

### Run the server.
```bash
node server.js
```

## Step 3: Frontend Setup

### Create an `index.html` file for the frontend.

### Create a `course-content.html` file for the course content.

### Create a `leader-board.html` file for the leader board.

### Create a `style.css` file to style your HTML.

### Create a `script.js` file to handle frontend interactions.

## Step 4: Testing
Open your web browser and navigate to http://localhost:3000.

# Hackathon Instructions
Finish up the project by: 
1. creating functionality for the logged in user to select their preferred courses.
2. store the selection in the database
3. create a page where the selected courses for each specific logged in user is displayed.
   
## Submission Guidelines
Fork this repository and clone it to your local machine. 
Create a new branch with your GitHub username (git checkout -b username). 
Complete the tasks. 
Commit your changes and push them to your forked repository. 
Submit a pull request to the main repository for review.

Happy hacking! 🚀

# Git and GitHub Assignment

## Summary

This repository was used for an assignment focusing on Git, GitHub, and open-source practices. Here’s a summary of the tasks completed:

1. **Cloned and Forked Repository**:
   - Cloned the [original repository](https://github.com/ClemenceKyende/lms-project.git) to my local machine.
   - Forked the repository to my GitHub account.

2. **Branch Management and Changes**:
   - Created a new branch `feature-update`.
   - Made changes to [`summary.md`](summary.md) to simulate feature updates.
   - Committed changes to `feature-update` branch.

3. **Conflict Handling**:
   - Created conflicts in [`summary.md`](summary.md) by modifying the same lines in different branches.
   - Resolved conflicts by manually editing `summary.md` to keep relevant changes.
   - Committed the resolved changes and merged back into `main` branch.

4. **GitHub Pages**:
   - Created [`index.html`](index.html) to enable GitHub Pages.
   - Verified the published page at [GitHub Pages](https://clemencekyende.github.io/lms-project/).

5. **Open Source Exploration**:
   - Explored open-source projects related to my interests on GitHub.
   - Opened an issue and engaged with the community in [lms-Project](https://github.com/ClemenceKyende/lms-project.git).

## Conclusion

This assignment provided hands-on experience with Git, GitHub, branch management, conflict resolution, GitHub Pages, and contributing to open-source projects.

Feel free to explore the repository and review the commits for a detailed history of actions taken during the assignment.

If you have any questions or feedback, please let me know!
