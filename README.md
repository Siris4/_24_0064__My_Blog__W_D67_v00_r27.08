# Flask Blog Application

This is a simple blog application built using Flask, SQLAlchemy, and CKEditor. The application allows users to create, edit, and delete blog posts. It also includes user registration and login functionalities.

## Features

- **User Authentication**: Users can register, log in, and log out.
- **Create Posts**: Logged-in users can create new blog posts.
- **Edit Posts**: Logged-in users can edit their own blog posts.
- **Delete Posts**: Logged-in users can delete their own blog posts with a confirmation prompt.
- **Rich Text Editor**: CKEditor is used for the content of the blog posts.
- **Pagination**: Posts are paginated to display a limited number of posts per page.
- **Responsive Design**: The application uses Bootstrap for responsive design.

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/your-repository.git
Navigate to the project directory:

bash
Copy code
cd your-repository
Create and activate a virtual environment:

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install the dependencies:

bash
Copy code
pip install -r requirements.txt
Set up environment variables:
Create a .env file in the project directory and add your email credentials and secret key:

env
Copy code
SECRET_KEY='your-secret-key'
MY_FROM_EMAIL1='your-email@example.com'
PASSWORD='your-email-password'
THEIR_EMAIL2='recipient-email@example.com'
Initialize the database:
Delete the existing posts.db file if it exists, and then run the following command to create a new database:

bash
Copy code
flask db init
flask db migrate -m "Initial migration."
flask db upgrade
Usage
Run the Flask application:

bash
Copy code
flask run
Open your web browser and go to http://127.0.0.1:5000 to access the blog application.

Project Structure
bash
Copy code
├── instance
│   └── posts.db                # SQLite database file
├── static
│   ├── assets
│   │   ├── favicon.ico
│   │   └── img
│   ├── css
│   │   └── styles.css
│   └── js
│       └── scripts.js
├── templates
│   ├── about.html
│   ├── contact.html
│   ├── header.html
│   ├── footer.html
│   ├── index.html
│   ├── login.html
│   ├── logout.html
│   ├── new_post.html
│   ├── post.html
│   └── register.html
├── .env                       # Environment variables
├── .gitignore                 # Git ignore file
├── forms.py                   # WTForms for the application
├── main.py                    # Main Flask application
├── requirements.txt           # Project dependencies
└── README.md                  # Project documentation
Dependencies
Flask
Flask-Bootstrap
Flask-SQLAlchemy
Flask-CKEditor
Flask-Bcrypt
Flask-Login
Requests
WTForms
SQLAlchemy
Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgements
Flask
Bootstrap
CKEditor
SQLAlchemy