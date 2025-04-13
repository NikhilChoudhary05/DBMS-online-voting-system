The Online Voting System is a full-stack web-based application that enables secure and transparent voting for users through a digital interface. This system eliminates the need for physical polling booths and paper ballots by digitizing the entire voting process. It is especially useful in academic, organizational, or small-scale elections where transparency, real-time results, and ease of use are crucial.

This project is developed using PHP for the server-side scripting, MySQL as the database management system, and HTML/CSS for the frontend user interface. The system allows voters to log in using their Voter ID, cast their vote for a preferred candidate, and ensures that duplicate voting is prevented by implementing one-vote-per-voter logic in the backend.

The application consists of three main modules:

Voter Registration & Verification Module:
Although registration is manual in this prototype, the database stores the name, gender, and Voter ID of eligible voters. During voting, the system cross-checks the Voter ID to ensure authenticity and eligibility.

Voting Module:
The voting form allows a voter to select a candidate from a dropdown menu and submit their vote. The vote is then recorded in the database. The backend logic ensures that:

Only registered voters can vote.

No voter can vote more than once.

Results Module:
A separate PHP page displays the live results of the election. It fetches data from the Votes table and displays the total number of votes received by each candidate. The data is grouped and counted using SQL queries, and results are presented in a tabular format.

📌 Key Features:

Simple, clean UI with HTML/CSS for easy user interaction.

Secure backend with PHP and prepared statements to prevent SQL injection.

MySQL relational database with two tables: Voters and Votes.

Vote casting with real-time validation and duplicate vote protection.

Live results visualization via grouped SQL queries.

📁 Folder Structure:

OnlineVotingSystem/
├── frontend/
│ └── index.html – Voting form
├── backend/
│ ├── config.php – Database connection
│ ├── vote.php – Voting logic and validation
│ └── results.php – Live vote count results
└── database/
└── votingsystem.sql – Exported MySQL schema and sample data

🗄️ Database Design:

Voters Table: Stores voter_id (primary key), name, and gender.

Votes Table: Stores vote_id (auto-increment), voter_id (foreign key), and vote_choice (candidate name).

👨‍🔧 Tools and Technologies Used:

VS Code – Development Environment

XAMPP – Localhost server with Apache and MySQL

PHP – Backend Scripting

MySQL – Database

HTML/CSS – Frontend Design

phpMyAdmin – Database Management

🧠 Learning Outcomes:

Understanding of full-stack web development.

Practical use of DDL, DML, DCL, and TCL SQL commands.

Implementation of database relationships using foreign keys.

Prepared statement usage in PHP for secure database operations.

Real-world application of relational database and user validation logic.

🚀 Future Enhancements:

Add login system with email/OTP authentication.

Admin dashboard for managing voters and candidates.

Graphical representation of results using Chart.js.

Responsive design using Bootstrap or Tailwind CSS.

Email confirmation or SMS notification after voting.

📝 Conclusion:

This Online Voting System is a compact, secure, and extendable project that reflects a real-world voting mechanism using modern web technologies. It demonstrates backend data validation, frontend form handling, SQL database manipulation, and real-time result calculation – making it an excellent project for academic submissions, portfolio showcases, or community elections.
