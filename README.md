This is a portfolio website I built in June-July 2024. 
I have used Next.js 13, Payload CMS, MongoDB, and GraphQL.

This project is comprised of a cms application (the backend), and a web application (the frontend).
In order to get this running, you would first need to setup the cms.

The cms is missing an .env file in its src folder.
The .env file should have (1) a secret variable, and (2) a MongoDB uri (I used the community version for this project).
The .env file is referenced from the /src/server.ts file.

Once the .env file is properly configured, you can run the cms by:
1. running an npm install
2. running an npm serve

Once the CMS is setup to run, you can launch the frontend application. 
The frontend application requires the CMS to be setup since the build process uses SSR and makes requests to the CMS application.
