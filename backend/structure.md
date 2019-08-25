# Structure
The following project structure has been followed while developing JRO frontend :
```markdown
- Root Folder
    - JROBackend/
        - keyconfig.py : Contains all the environment variables like API keys, Secret Key etc.
        - settings.py : Contains all the major configurations like database etc. for Django project.
        - urls.py : Contains the root url's of Django Project
    - media/ : Contains all the files of the project.
    - static/ : Contains all the static files like CSS, JS etc.
    - journal/
        - models.py - Contains the models, currently only UploadedResearchObject and GithubResearchObject
        - urls.py - Contains URL's for all the app functionality, All API endpoints can be found here
        - views/
            - auth/ - Contains mostly authentication related API views
            - github/ - Contains endpoints related to adding RO's to GitHub, IPFS and blockchain
            - ipfs/ - Contains endpoints related to adding uploaded files to IFPS and blockchain
```     

