Command Line Quiz Application

A command-line based quiz game built with Python and PostgreSQL.
Players can register, login, and test their knowledge by answering randomly selected questions from a database.
🚀 Features

    User registration and secure login (passwords hashed with bcrypt)

    Randomized quiz questions

    Add new quiz questions to specific topics

    Load bulk questions from a JSON file

    View existing questions by topic

    PostgreSQL database integration

🛠️ Tech Stack

    Python 3

    PostgreSQL

    psycopg2 (PostgreSQL database driver for Python)

    bcrypt (Password hashing)

⚙️ Setup Instructions

    Clone the repository:

git clone git@github.com:Fabi-DCI/command-line-quiz-db.git
cd command-line-quiz-db

    Install dependencies:

pip install psycopg2 bcrypt

    Database Setup:

    Create a PostgreSQL database named quiz_app.

    Create required tables: users, topics, and questions.

    (You will need to create the tables manually or with an SQL script.)

    Configure your database connection:

    Create a db_connection.py file (this file is ignored from Git).

DB_PARAMS = {
    "dbname": "quiz_app",
    "user": "your_username",
    "password": "your_password",
    "host": "localhost",
    "port": "5432"
}

    Run the Application:

python quiz.py

📖 How to Use

    Register as a new user.

    Login to your account.

    Start a quiz by selecting a topic and answering random questions.

    Add new questions manually to expand the quiz.

    View existing questions organized by topic.

    Bulk upload questions from a structured JSON file.

🔒 Security

    Passwords are hashed using bcrypt before storing them in the database.

    Database credentials are kept private and are not uploaded to GitHub.

✍️ Author

    Fabian Thamm