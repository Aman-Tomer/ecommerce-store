## Instructions

1. Download on your system
2. Extract in a folder
3. Open with visual studio code

Commands:
    Create & activate a virtual environment once you've navigated to the project directory:
        py -m venv venv
        venv\Scripts\activate
    Install the required dependencies:
        pip install -r requirements.txt
    To start the application:
        py manage.py runserver


In core /settings.py, the configuration related to the Stripe API is commented out - just put your own details in here (not all of these are connected to the project): register on Stripe's website & go to "API Keys" link in the left sidebar on the dashboard page. Copy over your publishable & secret key data from there.  

# Stripe Payment
PUBLISHABLE_KEY = ''
SECRET_KEY = ''
STRIPE_ENDPOINT_SECRET = ''

# Admin login
1. http://127.0.0.1:8000/admin
2. username and password = admin
