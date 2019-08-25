# Add environment variables
Some important variables that are used throughout the app are kept in environments/environment.ts (developement) and environments/environment.prod.ts (production). Example of such variables are API keys, url's of Composer REST Server and django API etc.

In order for all the services to work properly, Configure the following keys before using application (IP's should include respective ports):
```typescript
// The file contents for the current environment will overwrite these during build.
// The build system defaults to the dev environment which uses `environment.ts`, but if you do
// `ng build --env=prod` then `environment.prod.ts` will be used instead.
// The list of which env maps to which file can be found in `.angular-cli.json`.

export const environment = {
  production: false,
  serviceUrl: 'composer-rest-server-ip',
  redirectUrl: 'frontend-ip/login',
  // Orcid information
  orcidUrl: 'https://sandbox.orcid.org/oauth/token',
  orcidClientId: 'orcid-client-id',
  orcidClientSecret: 'orcid-client-secret',
  orcidUserUrl: 'https://api.sandbox.orcid.org/v2.1/',
  // Github information
  githubClientId: 'githubclientid',
  githubClientSecret: 'githubclientsecret',
  githubApi: "https://github.com/login/oauth/access_token",
  githubUserApi: "https://api.github.com/user",
  jroBackendUrl: "django-ip",
  composerUrl: "composer-rest-server-ip"
};                                                                                                                                                             
```