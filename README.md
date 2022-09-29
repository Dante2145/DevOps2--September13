# Instructions for Using GitHub for Group Project. <br>
## Links
[Link to Netlify Project](https://darling-longma-e101b4.netlify.app/dashboard).<br>
[Link to GitHub Repo](https://github.com/Dante2145/EasyRent-React) [<em>Note: Private Access</em>]<br>
[Link to GitHub Repo](https://github.com/sebprestele/financial-dashboard-fullstack)<br>
[Link to GitHub Repo](https://github.com/MorgDzh/Multifunctional-React-Dashboard)<br>
<br>
<em> Reminder to Daniel to change the Domain name in Netlify </em>

## GitHub
1. Open up your VSCode in a new folder on your local computer (i.e. C:\Users\Desktop\New Folder)
2. Within the new folder (i.e. C:\Users\Desktop\New Folder), open up a new terminal (Shortcut CTRL + SHIFT + ~)
3. <b>Optional but recommended</b> Type: git init. This will initialize the folder on your local computer and help track any changes on all the files within the folder. 
4. Type: git clone https://github.com/Dante2145/EasyRent-React. This will clone the Remote Repo onto your computer
5. Edit the files you want to on your local computer. <em> Notice: </em> that their will be <b>U, X, M, dots</b> next to files that you have edited.
6. To commit the changes to the GitHub Repo (So that the Netlify will render the changes to the website) you need to do the following in order:
* git add . (. means all files, you can also manually type out individual files. i.e. git add README.md index.js)
* git commit -m "<em>Type a detailed comment that reflects what changes you did to the repo</em>" e.g. git commit -m "Added index.js file to src folder"
* git push origin main (main is the number of the branch, commonly could be master).
<b>You have permission to access the Repo but any changes or commits, Daniel has to approve (Also figure out how)</b>


## Node 
After cloning from the GitHub Repo you will need to run in both the main folder as well as the client folder: 
> npm install

This will install all of the packages/dependencies/libraries on your local computer.

## Netlify
Nothing complicated needs to do be for Netlify. <br>
Ensure that you follow the steps above to Commit the changes to git. <br>

#### Problems you could face
* Build Production Failed. Mutliple issues with code. Attempt to run it locally and make sure the git Repo is the same as your cloned repo on your computer.
* Build Production Published but may not look like when you run it locally. 

## Heroku/MongoDB
Process of converting from Heroku to MongoDb has been successful, but the Database Structure has not been updated.
Nothing complicated needs to do be for Mongo. <br>
Ensure that you follow the steps above to Commit the changes to git. <br>

## MERN - React
After cloning and installing all the libraries, go to the terminal and go into the client folder
> cd C:\Desktop\Folder Name\client

and type

> npm start

This will run the REACT app and render the website locally via PORT 3000. 

## Folder Structure of GitHub Repo
This section details and explains what is inside each folder and what they do. <br>
* client - Contains all the frontend files for the website
    *  build - Don't touch this folder. This folder is packaged by REACT and Netlify will render the website from this folder.
    *  public - Contains 3 files, most important is index.html. This file contains the <b>meta</b> data. Such as meta and link and title tags. 
    *  src
        *  actions - Can't really explain what they do yet, Part of how REACT uses various functions to communicate to each other. These ones used for Authorization.
        *  components - Contain auth, dashboard, layout and private route, which contain files that basically render the individual pages or elements (such as sidebar and navbars) on the website/app
        *  images - Self explanatory, images for site. <b> TO CONSIDER MOVING TO AN ASSETS FOLDER</b>
        *  reducers - Reducers - Can't really explain what they do yet, Part of how REACT uses various functions to communicate to each other. These ones used for Authorization.
        *  utils - Authorization files.
        *  app.css - css file - currently empty - probably won't use
        *  app.js - File that renders the website components built in REACT.
        *  app.test.js - Autogenerated file when creating a new react app. <b>Cannot delete</b>
        *  index.js - Autogenerated file when creating a new react app. <b>Cannot delete</b>.
        *  serviceWorker.js - Autogenerated file when creating a new react app. Can consider deleting
        *  store.js
    *  .gitignore
    *  Readme.md
    *  package.json
* config - Contains configuration files. Contains passport.js (Authentication similiar to Auth0,<em>can be replaced by SingPass in the future</em>) and key.js (Sensitive information, similiar to .env file)
* models - Models are database schemas. Contains User.js which defines Database structure.
* routes/api - Contains users.js which POSTs information from login and registration pages.
* validation - Contains files login.js and register.js that are used for Data Validation (i.e. password match, password length, legitimate email)  on the respective frontend pages.
* .gitignore - Files that you have that you don't want to be accessible on gitHub. Usually used for API KEYs and sensitive information
* README.md - Read me file
* package.json - all the packages/libraries/dependencies that the <b>backend server</b> uses. You will see another package.json in the client folder, that is for the frontend
* server.js - backend server file, which connects to the database and contains the api routes.

#  Look forward for more details
new information coming soon
