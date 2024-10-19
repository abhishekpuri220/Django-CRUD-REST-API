A simple Django REST API providing Create, Read, Update, and Delete (CRUD) functionality for a data model. Built using Django and Django REST Framework.

Features
Create new records
Retrieve a list of records or individual records
Update existing records
Delete records
Prerequisites
Ensure you have the following installed:

Python 3.x
Django
Django REST Framework
pip (Python package manager)
Git (optional, for cloning the repository)
Setup Instructions
Step 1: Clone the Repository
If you haven't cloned the project yet, run:

bash
Copy code
git clone https://github.com/abhishekpuri220/Django-CRUD-REST-API.git
cd simplecrudapi
Step 2: Create a Virtual Environment (Optional but Recommended)
Create a virtual environment to isolate the dependencies:

bash
Copy code
python -m venv venv
Activate the virtual environment:

Windows:
bash
Copy code
venv\Scripts\activate
macOS/Linux:
bash
Copy code
source venv/bin/activate
Step 3: Install Dependencies
Install the necessary dependencies using pip:

bash
Copy code
pip install -r requirements.txt
If there is no requirements.txt file, you can manually install Django and Django REST framework:

bash
Copy code
pip install django djangorestframework
Step 4: Configure Database
By default, the project is set up to use SQLite, Django’s built-in database. If you're using a different database, configure the settings in settings.py under the DATABASES section.

Step 5: Apply Migrations
Run the following command to apply the database migrations:

bash
Copy code
python manage.py migrate
Step 6: Create a Superuser (Optional)
To access the Django admin panel and manage data via the browser, create a superuser:

bash
Copy code
python manage.py createsuperuser
Step 7: Run the Server
Start the development server:

bash
Copy code
python manage.py runserver
Step 8: Access the API
Once the server is running, you can access the API at:

API root: http://127.0.0.1:8000/api/
Admin panel (optional): http://127.0.0.1:8000/admin/
API Endpoints
Here are some sample endpoints for the CRUD operations:

GET /api/users/ - Retrieve a list of users
POST /api/users/create/ - Create a new user
GET /api/users/<int:pk>/ - Retrieve a specific user
PUT /api/users/<int:pk>/ - Update a specific item
DELETE /api/users/<int:pk>/ - Delete a specific item
Built With
Django
Django REST Framework
License
This project is licensed under the MIT License - see the LICENSE file for details.
