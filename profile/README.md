# Harxer Public Projects
## Author: Harrison Balogh

Collection of web apps.

## Stack

All apps target ESModules, rather than CommonJS - including node runtime servers/services.
Services target Node>16 which provides native ESModule support. In some cases, babel is used in
the build process to transpile JS. In all cases, babel converts react components to pure JS.

Deploy scripts are specific to each repository and executed on a deployment server running
the HxDeployService. This service listens for GitHub webhooks on repository release events.
Due to hosted server memory limitations, most build/compile steps are executed locally and
included in a repo /dist dir for a deploy script to pull/download. 
