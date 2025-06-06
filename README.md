# My Django Tech Blog

A simple blog application built with Django, created as a learning project. This blog allows users to create, read, update, and delete posts, as well as comment on posts.



## Features

*   User authentication (Login, Logout).
*   Create, Read, Update, Delete (CRUD) operations for blog posts.
*   Draft and Published states for posts.
*   Commenting system for posts.
*   Comment approval/moderation by authenticated users (e.g., post author or admin).
*   Basic styling with Bootstrap.


## Tech Stack

*   **Backend:** Python, Django (version X.X.X - *specify your Django version*)
*   **Database:** SQLite3 (for development)
*   **Frontend:** HTML, CSS, Bootstrap 4
*   **Version Control:** Git, GitHub

## Project Structure

A brief overview of the main directories and files:
mysite/
├── blog/ # Main blog application
│ ├── migrations/
│ ├── static/blog/css/ # App-specific static CSS (if any)
│ │ └── blog.css
│ ├── templates/blog/ # HTML templates for the blog app
│ │ ├── about.html
│ │ ├── base.html
│ │ ├── comment_form.html
│ │ ├── post_confirm_delete.html
│ │ ├── post_detail.html
│ │ ├── post_draft_list.html
│ │ ├── post_form.html
│ │ └── post_list.html
│ ├── init.py
│ ├── admin.py
│ ├── apps.py
│ ├── forms.py
│ ├── models.py
│ ├── tests.py
│ ├── urls.py
│ └── views.py
├── mysite/ # Project configuration
│ ├── init.py
│ ├── settings.py
│ ├── urls.py
│ └── wsgi.py
├── static/ # Project-wide static files
│ └── css/
│ └── blog.css # (Example: if your main CSS is here)
│ └── js/
│ └── blog.js # (Example: if you have global JS)
├── templates/registration/ # Templates for authentication (if you created them)
│ └── login.html
├── .gitignore
├── db.sqlite3 # (Usually gitignored, mention if not)
├── manage.py
├── README.md
└── requirements.txt


## Setup and Installation

To set up and run this project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/your-repository-name.git
    cd your-repository-name
    ```

2.  **Create and activate a virtual environment:**
    (Using `venv` which is built into Python 3)
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```
    (For Windows):
    ```bash
    python -m venv venv
    .\venv\Scripts\activate
    ```
    *(If you used Anaconda, provide those instructions, e.g., `conda create --name myblogenv python=3.10` and `conda activate myblogenv`)*

3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Apply database migrations:**
    ```bash
    python manage.py migrate
    ```

5.  **Create a superuser (optional, for admin access):**
    ```bash
    python manage.py createsuperuser
    ```
    Follow the prompts to create an admin account.

## Running the Application

1.  **Start the development server:**
    ```bash
    python manage.py runserver
    ```

2.  Open your web browser and navigate to `http://127.0.0.1:8000/`.
    *   The admin panel can be accessed at `http://127.0.0.1:8000/admin/` if you created a superuser.

## Key Learnings

*(This section is great for showing what you've learned)*
*   Setting up a Django project and understanding its structure.
*   Working with Django Models, Views (Class-Based Views and Function-Based Views), and Templates.
*   Implementing CRUD functionality.
*   User authentication and authorization (LoginRequiredMixin, @login_required).
*   Working with Django Forms.
*   URL routing and reversing URLs.
*   Using Django's ORM for database interactions.
*   Static file management.
*   Basic Bootstrap integration for styling.


## Future Enhancements 

*   Implement rich text editing for blog posts.
*   Add categories or tags for posts.
*   Implement search functionality.
*   Add pagination for post lists.
*   User profile pages.


## Contributing

If this were an open-source project, you would put contribution guidelines here. For a personal learning project, you can omit this or state:
"This is primarily a personal learning project. However, suggestions or feedback are welcome via issues."

