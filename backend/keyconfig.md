# Configuring keyconfig.py
Inside JROBackend/ folder in the project directory (same directory as settings.py), You will have to add a file - keyconfig.py
Paste the following content inside this, Replace <variable> with value for corresponding variable (without "<>").

```keyconfig.py
SECRET_KEY = '<SECRET_KEY>'
SERVER = False # True if you are running it on production server
DEBUG = True # False if you are running it on production server

SERVER_ADDRESS = "https://yourwebsite.com" # Comment out if running locally

# Following variables are only needed if SERVER=True
# If SERVER=True, Django makes use of MySQL database instead of default SQLite (since its more robust and suited for production)
DATABASE_NAME = "jrodb" # MySQL database name 
DATABASE_USER = "jrouser" # MySQL database user
DATABASE_PASSWORD = "!N*-5m74?@-!V9EW" # MySQL database user's password
```
