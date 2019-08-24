# Installation
> Install jroBna file using tutorial mentioned in Pre-Requisites section.
## Backend
Install a Virtual Environment (replace <virtual-env-name> with name of your choice):
```shell
python3 -m pip install virtualenv
virtualenv <virtual-env-name>
source <virtual-env-name>/bin/activate
```
Now go to the JROBackend repo's root folder and install the dependencies:
```shell
pip3 install -r requirements.txt
```
All the confidential stuff (Secret Keys, API keys etc.) should be kept in a file called keyconfig.py inside the django project folder also named JROBackend (where settings.py resides).
```shell
cd /path/to/JROBackend/JROBackend/
touch keyconfig.py
vi keyconfig.py
```
Add the following content inside this file:
```python
SECRET_KEY = 'your django secret key'
SERVER = False # False for developement but SHOULD BE True for production.
DEBUG = True # True for developement but SHOULD BE False for production.

# Following keys are only needed if SERVER is True
DATABASE_NAME = "mysql-database-name" 
DATABASE_USER = "mysql-database-user"
DATABASE_PASSWORD = "mysql-database-password"
SERVER_ADDRESS = "https://yourwebaddress.com"
```
Run the following commands to get the project running:
```shell
cd JROBackend
python3 manage.py migrate
python3 manage.py runserver
```
This will start a developement server on localhost.
## Frontend
> Please keep in mind that Frontend (Angular) and Hyperledger Composer use different versions of node. Composer typically uses node v8.15.1. To install multiple versions of node, you need to have nvm (node version manager) installed. Follow these commands to do so :
```shell
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash
nvm --version # Should give some version number as output
```
Restart the terminal session for installation to take effect. Then use following commands to install latest node version.

The frontend code is writted in Angular 8. You will need to have Angular CLI installed, which can be done using :
```shell
$ nvm use node # To use latest node version
$ npm install -g @angular/cli
```
Now, we can run the developement server:
```shell
$ cd Journal-Of-Research-Objects-Frontend
$ npm install
$ ng serve
```
This should start a developement server at http://localhost:4200/
