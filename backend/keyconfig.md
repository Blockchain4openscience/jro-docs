# Configuring keyconfig.py
Inside JROBackend/ folder in the project directory (same directory as settings.py), You will have to add a file - keyconfig.py
Paste the following content inside this, Replace <variable> with value for corresponding variable (without "<>").

```keyconfig.py
COMPOSER_REST_URL = '<COMPOSER_REST_SERVER_URL>' # Put the url of your rest server url without trailing '/' Example: 'http://localhost:3000'
IPFS_ADDRESS = '/ip4/127.0.0.1/tcp/5001/http' # Address for connection to IPFS, the default value is given here.

SECRET_KEY = '<SECRET_KEY>'
SERVER = False # True if you are running it on production server
DEBUG = True # False if you are running it on production server

SERVER_ADDRESS = "https://yourwebsite.com" # Comment out if running locally

# Following variables are only needed if SERVER=True
# In production, We want to use MySQL database instead of default SQLite (since its more robust)
DATABASE_NAME = "<db_name>" # MySQL database name 
DATABASE_USER = "<db_user>" # MySQL database user
DATABASE_PASSWORD = "<db_password>" # MySQL database user's password


```
