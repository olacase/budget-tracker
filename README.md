# Budget Tracker Starter Code


### User Story
A Budget Tracker application that allows users to add expenses and deposits to their budget with or without a connection. When entering transactions offline, they should populate the total when brought back online.


## Table of contents

- [Installation](#Install)
- [Usage](#Usage)
- [Technologies](#Technologies)
- [Functionality](#Functionality)
- [Run](#Run)
- [Deploy](#Deploy)
- [Author](#Author)
- [License](#License)

# Installation
Download or clone repository
npm install to install the required npm packages to run

# Usage
Application will be invoked by using the following command:

node server.js

Open your browser and go to

https://budgetmonk.herokuapp.com/

User can add transactions as deposits or expenses by inputting the following:

Name of transaction
Transaction amount
For deposits - select Add Funds
For expenses - select Subtract Funds
The total amount is reflected as soon as funds are entered

The graph portrays the total funds over time by date entered for each transaction


 # Technologies
- HTML5
- CSS
- jQuery
- Express
- MongoDB
- Mongoose
- IndexedDB
- Bootstrap
# Functionality 

BUDGET-TRACKER Offline Functionality:
- Enter deposits offline
- Enter expenses offline

When brought back online:
- Offline entries should be added to tracker.

## *In order to achieve OFFLINE SUPPORT, a manifest file and a service worker file must be created.*

### Run 
- 1. On your VS Code clone the "https://github.com/olacase/Budget-Tracker.
- 2. Install all dependencies (see above)
- 3. Create a terminal on the Budget-Tracker folder and run:
    ```` bash
    mongod
    ````
- 4. Create another terminal on the same folder and run:
    ``` bash
    node server
    ```

### Deploy
- Follow the steps on how to deploy an app on heroku

1. Create a repository of your project in github. 
2. Clone that reporisitory to your VS Code using git:
``` bash
git clone "the link of the github repo"
```
3. In your project folder terminal create a heroku application using this command:
``` bash 
heroku create "name of your project"
```
4. Log in to your heroku account and look for your project in the DAHSBOARD. Go to the tabs located on top and click on DEPLOY. In the Deployement Method, click on the github icon to connect it to your github repository. Then on Automatic Deploy, click and enable automatic deploys

5. On the tabs on top, click Overview then on Installed add-ons click Configure Add-ons.

6. Since this project is build with MongoDB, search for mLab MongoDB in the Add-ons search. Make sure to select the "Sandbox-Free plan. Then provision it. 

7. Make sure that you have "process.env.MONGODB_URI" in your mongoose.connect under the server file. 

8. Try to add a code and push it to your github. It will automatically hook it to heroku. Now view your heroku app.


```



# Author
- Olamide Bello
- github: https://github.com/olacase
- email: olacase@gmail.com

# License
- none
