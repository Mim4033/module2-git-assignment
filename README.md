\# Django Todo App



A complete Todo web application built with Django, featuring a modern UI with Tailwind CSS.



\## Features



\- ✅ Create, Read, Update, and Delete tasks

\- ✅ Mark tasks as completed/active

\- ✅ Filter tasks by status (All, Active, Completed)

\- ✅ Set due dates for tasks

\- ✅ Add descriptions to tasks

\- ✅ AJAX toggle completion without page reload

\- ✅ Beautiful, responsive UI with Tailwind CSS

\- ✅ Django messages framework for user feedback



\## Tech Stack



\- \*\*Backend\*\*: Python + Django

\- \*\*Frontend\*\*: Django Templates + Tailwind CSS (via CDN)

\- \*\*Database\*\*: SQLite (for local development)

\- \*\*JavaScript\*\*: Minimal JS for enhanced UX (toggle completion)



\## Setup Instructions



\### Prerequisites



\- Python 3.8 or higher

\- pip (Python package manager)



\### Installation



1\. \*\*Clone or navigate to the project directory:\*\*

&nbsp;  ```bash

&nbsp;  cd /path/to/todo\_project

&nbsp;  ```



2\. \*\*Create a virtual environment (recommended):\*\*

&nbsp;  ```bash

&nbsp;  python3 -m venv venv

&nbsp;  source venv/bin/activate  # On Windows: venv\\Scripts\\activate

&nbsp;  ```



3\. \*\*Install dependencies:\*\*

&nbsp;  ```bash

&nbsp;  pip install -r requirements.txt

&nbsp;  ```



4\. \*\*Run migrations:\*\*

&nbsp;  ```bash

&nbsp;  python manage.py migrate

&nbsp;  ```



5\. \*\*Create a superuser (optional, for admin access):\*\*

&nbsp;  ```bash

&nbsp;  python manage.py createsuperuser

&nbsp;  ```



6\. \*\*Run the development server:\*\*

&nbsp;  ```bash

&nbsp;  python manage.py runserver

&nbsp;  ```



7\. \*\*Open your browser and navigate to:\*\*

&nbsp;  ```

&nbsp;  http://127.0.0.1:8000/

&nbsp;  ```



\## Project Structure



```

todo\_project/

├── manage.py

├── requirements.txt

├── README.md

├── db.sqlite3          # SQLite database (created after migrate)

├── todo\_project/       # Project settings

│   ├── \_\_init\_\_.py

│   ├── settings.py

│   ├── urls.py

│   ├── wsgi.py

│   └── asgi.py

├── tasks/              # Tasks app

│   ├── \_\_init\_\_.py

│   ├── models.py       # Task model

│   ├── views.py        # CRUD views

│   ├── forms.py        # Task form

│   ├── urls.py         # App URLs

│   ├── admin.py

│   ├── tests.py        # Unit tests

│   └── migrations/     # Database migrations

└── templates/          # HTML templates

&nbsp;   ├── base.html

&nbsp;   └── tasks/

&nbsp;       ├── task\_list.html

&nbsp;       ├── task\_form.html

&nbsp;       └── task\_confirm\_delete.html

```



\## Usage



\### Creating a Task



1\. Click the "+ New Task" button on the task list page

2\. Fill in the task title (required)

3\. Optionally add a description and due date

4\. Click "Create Task"



\### Managing Tasks



\- \*\*View Tasks\*\*: All tasks are displayed on the home page

\- \*\*Filter Tasks\*\*: Use the tabs (All/Active/Completed) to filter tasks

\- \*\*Toggle Completion\*\*: Click "Mark Complete" or "Mark Active" to toggle task status

\- \*\*Edit Task\*\*: Click the "Edit" button to modify a task

\- \*\*Delete Task\*\*: Click the "Delete" button and confirm deletion



\### Admin Interface



Access the Django admin panel at `http://127.0.0.1:8000/admin/` (requires superuser account).



\## Running Tests



```bash

python manage.py test

```



\## Development



\### Making Changes



1\. \*\*Model Changes\*\*: After modifying `models.py`, run:

&nbsp;  ```bash

&nbsp;  python manage.py makemigrations

&nbsp;  python manage.py migrate

&nbsp;  ```



2\. \*\*Static Files\*\*: This project uses Tailwind CSS via CDN, so no static file collection is needed for development.



\## License



This project is open source and available for educational purposes.



