## Instructions

1. Download the project on your system
2. Extract in a folder
3. Open with visual studio code

### Commands  
Create & activate a virtual environment once you've navigated to the project directory:  
>py -m venv venv  
>venv\Scripts\activate
    
Install the required dependencies:  
>pip install -r requirements.txt

To start the application:  
>py manage.py runserver

### Stripe Payment  
To see the Stripe payment API in action, put your own Stripe account details for the following pertinent configuration options(commented out in core /settings.py, not all of these are connected to the project): register on Stripe's website & go to "API Keys" link in the left sidebar on the dashboard page. Copy over your publishable & secret keys data from there.  

PUBLISHABLE_KEY = ''  
SECRET_KEY = ''  
STRIPE_ENDPOINT_SECRET = ''

Wrt STRIPE_ENDPOINT_SECRET setting, utilize the terminal to run below command:  
>.\stripe listen --forward-to localhost:8000/payment/webhook/

### Admin login
1. http://127.0.0.1:8000/admin
2. username and password = admin