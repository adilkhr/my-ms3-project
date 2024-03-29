# Milestone project 3: Building a jargon glossary/dictionary for a particular domain named COD Dictionary

![Main Mockup](README-files/mainmockup.png)

[Link to Live Website](https://adz-dictionary.herokuapp.com/)

[GitHub Repo](https://github.com/adilkhr/my-ms3-project)

***

## The purpose of the project

* To create an applicaition for users to look for definitions for words used in Call Of Duty warzone and understand what these terms mean in the game. I have allowed users to create an account so they can add their own definitions for new words. Users are able to update and delete their own i. I have used MongoDB to store the data and have used the framework Flask alongside HTML and custom CSS for the website's front-end.

***

## User Experience (UX)

## Strategy

### User Stories

#### First time visitor goals:

As a new user:

* I am looking to understand what certain words/terms mean for the game

* I want the site to be easy to navigate

* I want the the site to be responsive and work on any device

* I want to be able to create an account for the applicaiton to add new definitions

#### Existing User goals:

* I want to be able to sign up to add new definitions for words for others to see and understand what it means

* I would like to have a profile portal that is fully functional and working

* I want to be able to update i of words

* I want to be able to delete words i have created

#### Reasons for the website:

* To allow people who play call of duty to understand what terms that are used in the game mean 

* To allow experienced players to share new words/terms into the dictionary

## Scope
#### What a user may expect:

* Easy to navigate application

* A site that is visually appealing on all devices

* An option to register an account

* A search option to find a specific word/term that they have heard about while playing the game

* A log in feature to log in an add a new word to the dictionary

#### What a user may want:

* An option to edit a word (once they have created an account) that they have added into the dictionary if they want to update the meaning

* An option to delete a word (once they have created an account) that they added into the dictionary

* A access link to the official call of duty website

#### As a developer / business I expect:

* To provide an easy feature for users to register an account

* To provide an easy login page for users to log in once they have succesfully created their account

* To allow registered users to create new words with the definition and add them to the dictionary

* To also allow registered users to have the choice wether or not they would like to delete or edit their words created and added into the dictionary

## Structure

The website will consit of 3 pages for users that are not logged in,

* A home page which will contain: Dictionary of definitions, Search Bar to search the dictionary, About the website section 

* A log in page for exising users

* A Register page for new users

The website will consit of 4 pages for users that have an account and are logged in,

* A home page which will contain: Dictionary of definitions, Search Bar to search the dictionary, About the website section

* A profile page - which will display the users name to know that they are currently logged in

* An add word page - which will allow the logged in user to add a word into the dictionary

* An Edit word page - if a user has created a word, at the home page there will be and edit button for them on the word that they have created which will then take them to the edit word page

If a user is currently logged in, there will be a logout button for them at the navbar

***

## Database

### Database Schema:

I have used a non-relational database by using Mongo DB with a databse name of Jargon which contains two collections named word and users. 

The words collection will contain documents that will have three keys named: word_name(will contain a string value of the name of the word inputed by the user), word_description(will contain a string value of the definition of the word), and created_by(will contain a string value of the username that has inputed the word into the dictionary). Each word documented will have a ID which is similar to a primary key in a relational database like SQL.

The user collection will contain doccuments of the accounts created with the keys : username and password. Then username key will contain a string of the username created, and the password key will contain a string value of the password created but will not be visable, instead it will generate a random value such as "pbkdf2:sha256:260000$DTJwxoITI5MmjdWl$001c92d44c7655fade6513b3b54cdfae...", this keeps the users account privacy intact.

### Data Model:

The diagram below is the data model design of the site showcasing the architecture of the Web App. This displays the journeys users can take throughout the website.

![Data Model](README-files/ms3datamodel.jpg)

***

## Features

### Navigation Bar:

The navigation bar will be simple with the colors black and white, easy to use with the name of COD Dictionary which will have a home, log in and register pages for new users and users who are not logged in. When users log in, it will have a home, profile, addwords and a logout button. On smaller devices I have used a dropdown button to display the menu to make it fully responsive.

### Footer:

The footer will contain social media links for users to browse and connect with the site makers. The footer will have an about us section explaining more about the site. The footer will also contain a link to the offical call of duty page.

### Home:

Home page will include an image slider that will present text to the user to make it visually appealing. The dictionary is displayed to show the user all current words. If the user is the author of a word then two buttond will appear next to the word giving them the option to edit the word, or delete it. There is a search bar for users to search for words within the dictionary.

### Log in page:

A log in page for users who have already registered in the past to access their account by inputing their username and password into the log in form. It will also contain a carousel slide of images along with a quote underneath it.

### Register page:

A register page for new users to fill in the register form by inputting a username of their choice aswell as a password. It will also contain a carousel slide of images along with a quote underneath it.

### Profile page:

A profile page for users once they log in will be prompted to this page with their username showing aswell as a welcome image and welcome text. It will also have a link for the user to be directed to the add words page.

### Add words page:

A page for logged in users to add a new word with a definiton to the dicitionary for other users to see when they access the home page of the site. It will also contain a carousel slide of images along with a quote underneath it.

### Log out:

A button that will be located in the navbar for users who are logged in to log out once they are finished using the site.

### 

***

## Future Features 

* Customisable features for registered users to change color schemes of their profile and the site

* An option for registered users to add a profile image

* An option for registered users to delete their account

* An option for users to like words and submit word disputes

***

## Skeleton

### Wireframes:

Note: Wireframes for the desktop share similar strucuture for tablet

* Wireframes for desktop have been created and can be viewed [here](https://github.com/adilkhr/my-ms3-project/blob/main/wireframes/wireframesms3desktop.pdf)

* Wireframes for mobile phone have been created and can be viewed [here](https://github.com/adilkhr/my-ms3-project/blob/main/wireframes/wireframesms3phone.pdf)

### Mockup:

![Home Mockup](README-files/mockuphme.png)

![Log in Mockup](README-files/mockuplogin.png)

![Register Mockup](README-files/mockupreg.png)

![Home Mockup](README-files/mockupadd.png)

***

## Typography and color scheme

* For Typography I used google fonts to then apply the oswald font all round the site. I used the font-family of Bona Nova for the quotes that I have added on some of my pages

* The colour scheme used throughout the website were mainly white, black, and grey/blue grey. I kept the colour theme to a minimum as I felt there was no need to overcomplicate the site as it may distract users from the content and would not look visually appealing. Using materialize css throughout my project I used the color pallete they have to pick the colors used in my site, using the following: black, blue-grey darken 4, blue-grey darken 2 and blue-grey darken 1

***

## Technonologies Used

### Languages & Frameworks

* HTML5 - Mark-up language used to create the pages for site using semantic structure
* CCS3 - Cascading style sheet used to style the site, aswell as adding media queries to make it responsive for pretty much all devices
* Javascript - Programming language used to create functions working for the site
* Python - Programming language used to control backend development of the site
* Flask - Framework + Extensions
* [Materialize](https://materializecss.com/) - CSS Framework used for structure, buttons and some styling around the site, aswell as media functions for images
* [jQuery](https://jquery.com/) - Used for Materialize initialising
* [Gitpod.io](https://www.gitpod.io/) - Used for creating the workspace for writing the code. Using the command line terminal for commiting and pushing to GIT Hub
* [GitHub](https://github.com/) - Used for hosting repositories
* GIT - Used for pushing the code to repositories

### Front End

* [Google fonts](https://fonts.google.com/) - Used for the Font
* [Font Awesome](https://fontawesome.com/) - For the icons used

### Backend

* [MongoDB](https://account.mongodb.com/account/login?n=%2Fv2%2F60e4812e2528e83f16f7d2bc&nextHash=%23clusters) - Used as the database to store the users details, aswell as storing words created by users
* [Heroku](https://id.heroku.com/login) - Used to host the deployed project

### Planning

* [Balsamic Wireframes](https://balsamiq.com/) - Used to create the wireframe designs of the site
* Paint - Used to create the data model

### Flask

The application was built using the Flask Framework which is reliant on the jinja templating language. The application was written in python.

I used pip3 install Flask into the terminal to install flask. I used the standard port used for Flask applications which is "5000" and the IP set to "0.0.0.0".

Flask-PyMongo - For the applicaition to interact with the MongoDB database

Werkzeug - Used for providing security's, password_hash, check_password_hash

***

## Testing

### Supported Screens:

After using Materialize to build my pages and the use of CSS media queries styles, using the google inspect tool I was able to see that my site is supported for all screens with a width of 280px. I also did some testing by sending my website link to my friends and familys devices and they had seen no issues.

### Supported browsers:

The website link has been tested on Google chrome, Internet Explorer and Microsoft edge, Brave and Firefox and seem to be working fine.

### OS compatability:

Tested on iOS, Android 10, and Windows 10. - I asked a friend with an Android to test that it was working. Tested for responsiveness using Chrome DevTools.

### Peformance Testing:

* Tested on the Developer Tools Lighthouse

* I had family and friends test the site on different device to see if there were any major issues they was having when using or acessing the site and turns out they had found no major issues

### Testing User Stories:

#### New User

* I am looking to understand what certain words/terms mean for the game - Users can check for definition on the home page and by also using the searchbar to find a specific word

* I want the site to be very easy to navigate aswell. I want the the site to be responsive and work on any device - The user will have no problem acessing the site on either mobile or desktop as its responsive for both, and with mobile features implemented such as collapsable navbar. Site is very easy to use with clear layout and structure

* I want to be able to create an account for the applicaiton to add new definitions - The user is able to create an account at the register page with a username of their choice that is if the username has not already been taken, along with a password

#### Existing User

* I want to be able to sign up to add new definitions for words for others to see and understand what it means - The user can register an account at the register page, once they have created their account, they are then able to add new words into the dictionary at the add word page

* I would like to have a profile portal that is fully functional and working - When the user signs up they are prompted to the profile page higlighting their name aswell as a welcome message and image with also a shortcut link to add a new word into the dictionary

* I want to be able to update definitions of words - Users can edit any words that they have added into the dictionary when they are logged in at the home page, when clicking the edit button on the word, they are sent to an edit words page which they are then able to edit the word with a new definition or they can simply cancel the edit task and be sent straight back to the home page

* I want to be able to delete words i have created  - clicking on the delete button on the word that they have created will delete the word off the dictionary

### Code Validation:

* All my pages of the website was run through the [HTML Validator](https://validator.w3.org/#validate_by_input), because of flask being a templating language, the code when inputed was not showing the html code being valid, however I copied the html code om within DEV Tools, both by viewing page source and from within the inspect as HTML and passed it into the validators to check the validity which all pages showed validity

* The [CSS Validator](https://jigsaw.w3.org/css-validator/#validate_by_input) was used to check the validity of my CSS code which turned out to be all fine with no faults

* [jshint](https://jshint.com/) was used to check the validity of my javascript code which turned out to be all fine with no faults

* [Pep8 Online](http://pep8online.com/) was used to check for Pep8 compliances for my python file and test the validity of the code, which the code turned out to be all good

### Fixed bugs:

* I had an issue with my Navbar logo falling out of the navbar space for smaller screen sizes, but I was then able to resolve this issue by adding media queries and css styling to tackle this. 

* I had an issue with the dictionary words and edit and delete button falling out of place of the accordion which again was resolved by adding some media query codes in my css file. See the code bellow:

@media (max-width: 400px) {
    nav .brand-logo {
        font-size: 1.40rem !important;
        left: 25% !important;
        }
    .btn-small {
        width: 50px;
        font-size: 9px;
        }
    .wordname {
        font-size: 10px;
    }
}

* I had an issue with my footer not sticking to the bottom of my pages leaving white spacing underneath it, this was then solved by adding some css code to target the body of my base.html, see the code below:

body {
    display: flex;
    min-height: 100vh;
    flex-direction: column;
  }

***

## Deployment

### Configuration:

Bellow your imports you will need to configure your app.py file. You will need to import your local env.py for local environments.

Configure as follows:

if os.path.exists("env.py"):
    import env


app = Flask(__name__)

app.config["MONGO_DBNAME"] = os.environ.get("MONGO_DBNAME")
app.config["MONGO_URI"] = os.environ.get("MONGO_URI")
app.secret_key = os.environ.get("SECRET_KEY")

mongo = PyMongo(app)

To start your application, you will need to user the following at the bottom of your app.py file. You will need to ensure that debug=False prior to deployment.

        if __name__ == '__main__':
            app.run(host=os.environ.get('IP'),
                    port=int(os.environ.get('PORT')),
                    debug=False)

You will need to add a Procfile and ensure your requirements.txt are up to date. 
In your root folder in the terminal type - touch Procfile -  this will create a Procfile
Add the following with the following 
    web: python app.py

To install the requirements.txt use the following command in the terminal command line
    pip3 install -r requirements.txt

#### Local Environment:

Create env.py file in the same file system. In your route folder type - touch env.py - to create the file. 
Your virtual configurations should look similar to this. You will need to create a SECRET_KEY and input the IP and PORT settings. I used [Random Key Gen](https://randomkeygen.com/) which created a random key for me to use.

        import os

        # App config
        os.environ.setdefault("IP", "0.0.0.0")
        os.environ.setdefault("PORT", "5000")
        os.environ.setdefault("SECRET_KEY", "<Your secret key>")

        # MongoDB config
        os.environ.setdefault(
            "MONGO_URI", "mongodb+srv://<user>:<password>@<project>.af8bz.mongodb.net/<database>?retryWrites=true&w=majority")
        os.environ.setdefault("MONGO_DBNAME", "<database>")

### Adding and Committing files:

To add files to the repository, make sure to follow the steps bellow:

In the command line type -
        git add .  
        git commit -m "This is being committed"
        git push

To add all new files or modified file use " ."  - To add a single file, use the pathway to the file eg .base.html or assets/css/style.css
When committing make sure your comments are clear about what changes have been made and are not too long. 
initiating a git push will then send your work to the repository

### Deploying:

Requirements for deploying:
* MongoDB Account
* Heroku Account

Deploying to [Heroku](https://dashboard.heroku.com/)

* You will need to create an account with [Heroku](https://dashboard.heroku.com/)
* Once logged in click the create new app button
* Select the region that is closest to you and give the APP a name
* Set your deployment method to 'GitHub'
* Connect to GitHub and login
* Search for the repository you wish to deploy from
* You will need to head to settings and click 'Config Vars'
    * You will now need to set up your Configuration Vars the same way as you did for your env.py 
* Make sure you have set up your Procfile and you have updated the requirements.txt prior to deploying    
* Click the deploy tab and go to manual deploy
* Select the branch you wish to deploy and deploy the application on
* Once it is deployed you will be able to view the application
* You can set it to automatically deploy every time you push your code to the repository by enabling the Automatic deploys

### Forking

Forking the GitHub Repository

By forking the GitHub Repository, you can make a copy of the original repository in your own GitHub account. This means we can view or make changes without making the changes affecting the original.

* Log into GitHub and locate the GitHub Repository.
* At the top of the Repository there is a "Fork" button about the "Settings" button on the menu.
* You should now have a new copy of the original repository in your own GitHub account.
* You will need to install the requirements.txt using the following command the command line
        pip3 install -r requirements.txt
* You will need to set up your local environments and key value pairs for deployment

### Cloning 

Making a Local Clone

* Log into your GitHub then find the gitpod repository
* Under the repository name there is a button that says, "Clone or download". Click on this button.
* If cloning with HTTPS "Clone with HTTPS", copy this link.
* Open Gitbash
* Change the current working directory to the location where you want the cloned directory to be.
* Type git clone, and then paste the URL you copied earlier.

        $ git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY
        Press - Enter- Your local clone will be created.
        $ git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY
                > Cloning into `CI-Clone`...
                > remote: Counting objects: 10, done.
                > remote: Compressing objects: 100% (8/8), done.
                > remove: Total 10 (delta 1), reused 10 (delta 1)
                > Unpacking objects: 100% (10/10), done.
[Click Here](https://docs.github.com/en/free-pro-team@latest/github/creating-cloning-and-archiving-repositories/cloning-a-repository) for more info on cloning. 

You will need to install the requirements.txt using the following command the command line
        pip3 install -r requirements.txt

* You will need to set up your local environments and key value pairs for deployment and running the application in your local environment. 

***

## Credits

### Code:

* I used code from [Materialize css](https://materializecss.com/) for some of my front-end styling and Javascript

### Media:

* All images used were taken from [google images](https://www.google.com/imghp?hl=en)

### Acknowledgements:

* Rohit Sharma (mentor support) - Provided me with help on how to structure the site and what should be the main focuses of the project

* Matt Rudge - Template for Gitpod.io

* Full Stack Developers WhatsApp group (members of the codeinstitute slack community) - for taking the time to test the website aswell as providing help when needed with issues

* I had used the [Code institute sample read me template](https://github.com/Code-Institute-Solutions/SampleREADME) to strcuture my own readme.

* [W3schools](https://www.w3schools.com/) was used for various code information and trouble shooting problems

* Code insitute tutor support - Provided me with a lot of help support when needed whenever I contacted them

* [Youtube](https://www.youtube.com/) - Provided me with a lot of help when trouble shooting issues

* [Code instiute Task manager mini project](https://github.com/Code-Institute-Solutions/TaskManagerAuth/tree/main/08-SearchingWithinTheDatabase) Provided me with a lot of help intialising the development process of the site aswell as setting up MONGO DB with the site, it also helped me with understanding more on python and how it works

* Rebecca Kelsall (fellow codeinstiute student) - for proof reading my README.md, and providing me with her [MS3 reposoitory](https://github.com/crypticCaroline/puppyplaymates) to give me an understanding on how to structure my README

### Content:

I asked friends and family to create a profile and add definitions to the site to see if it works effectively

Code & Content (not already attributed): Adil Khair

### Inspiration:

* Inspiration was taken from the [Code instiute Task manager mini project](https://github.com/Code-Institute-Solutions/TaskManagerAuth/tree/main/08-SearchingWithinTheDatabase) to help gain an idea of how to structure my site and more idea on developing the backend side of my site

* The idea of the site came from the game [Call of Duty](https://www.callofduty.com/uk/en/home), as a player of the game, I thought this would be a great idea for me to create an online dictionary based on the many terms used in the game where new players may not understand words that are being said by other players


