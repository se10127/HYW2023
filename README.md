# Template for HTML web pages
## Project setup
1. Clone or fork this repository. 
2. If you fork the repository, skip the next steps in this section.
3. Copy all the files in this repository to a new folder.
4. Create an empty repository on [GitHub](https://www.github.com)
5. In the new folder run:
   1. `git init`
   2. `git add .`
   3. `git commit -am "init"`
   4. `git remote add origin $URL_TO_YOUR_GITREPO`
   5. `git push -u origin main`

## Run locally
You need node js installed locally on your computer.
1. Run `npm install`
2. Run `npm run start` to start the app
3. Run `npm run dev` to start the server in develoment mode, the server will restart everytime you save a file.
4. Go to http://127.0.0.1:8080, you should see the html page.

## Dockerhub account
Go to [DockerHub](https://hub.docker.com/). Sign up for an account with your email address.

## Deploy on Code Engine
You need an account on Dockerhub to deploy the app on Code Engine. Make sure your github repository is public.
1. Search for Code Engine in the IBM Catalog
2. Press "Start creating" under "Start with source code"
3. Choose your project
4. Copy the url to your git repository under "Source code URL"
5. Set "Listening port" to 8080
6. Press "Build Details"
7. Enter the git branch name
8. Press Next and then Next again
9. Enter "https://index.docker.io/v1/" under "Registry server"
10. Press "Registry access secret" and create a new secret. Enter your Dockerhub credentials.
11. Press "Create"
