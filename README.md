# Kobby's First Blog Site

![Project Image](./static/assets/img/resized-home-bg.jpg)

**A simple and powerful Flask-based blog site where users can create, edit, and share their thoughts.**

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Database Configuration](#database-configuration)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Welcome to Kobby's Blog, a web application built with Flask, Bootstrap, and SQLAlchemy. This project allows users to create, edit, and delete blog posts. It features user authentication, comments, and admin-only functionalities.

## Features

- User registration and authentication.
- Create, edit, and delete blog posts.
- User comments on blog posts.
- Admin-only features for post management.
- Gravatar integration for user profile images.
- Responsive design using Bootstrap.

## Installation

1. **Clone the repository to your local machine:**

    ```bash
    git clone https://github.com/your-username/your-repository.git
    ```

2. **Set up a virtual environment:**

    ```bash
    python -m venv venv
    ```

3. **Activate the virtual environment:**

    - On Windows:

        ```bash
        .\venv\Scripts\activate
        ```

    - On macOS/Linux:

        ```bash
        source venv/bin/activate
        ```

4. **Install dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. **Create and apply database migrations:**

    ```bash
    flask db init
    flask db upgrade
    ```

2. **Configure environment variables, especially `DB_URI`, for your database connection.**

3. **Run the Flask application:**

    ```bash
    python main.py
    ```

Visit [http://localhost:5000](http://localhost:5000) in your web browser.

## Database Configuration

The application is configured to use SQLAlchemy as the database ORM. The database URI is set as an environment variable (`DB_URI`), providing flexibility to connect to different databases or use SQLite as the default.

```python
app.config['SQLALCHEMY_DATABASE_URI'] = os.environ.get("DB_URI", "sqlite:///posts.db")
```

## Contributing
Contributions are welcome! Feel free to open issues, suggest improvements, or submit pull requests. If you encounter any issues, please let us know.

## License
This project is licensed under the MIT License. You are free to use, modify, and distribute the code for your own projects.

