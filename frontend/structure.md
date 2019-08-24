# Structure
The following project structure has been followed while developing JRO frontend :
```markdown
- Root Folder
    - e2e (Tests)
    - angular.json (contains specified angular parameters)
    - package.json (contains angular package info)
    - src
        - assets (contains static assets required by the project)
        - fonts (contains fonts required by the project)
        - scss (contains scss files required by the project)
        - index.html (contains the meta tags of the home page)
        - environments
            - environment.ts (contains variables for developement environment)
            - environment.prod.ts (contains variables for production environment)
        - app
            - _nav.ts (All the data regarding navigation entries goes here)
            - app.component.ts (This is the root app component)
            - app.module.ts (this is root module)
            - app.routing.ts (this is root routing module, all new modules must be added here for routing to work)
            - containers
                - default-layout (this component contains nav bar etc. All other components are loaded under this)
            - jro (this contains all the components and services)
                - components (contains all components)
                    - auth (contains login component)
                    - dashboard (contains dashboard component)
                    - add (contains all the components which facilitate adding RO's)
                        - github (component for adding RO's from GitHub)
                        - upload (component for uploading RO's)
                    - enrich (contains components that facilitate enriching RO's)
                        - all (component that can 
```     
