# Milestone project 3: Building a jargon glossary/dictionary for a particular domain named COD Dictionary

![Main Mockup](README-files/mainmockup.png)

[Link to Live Website](https://adz-dictionary.herokuapp.com/)

[GitHub Repo](https://github.com/adilkhr/my-ms3-project)

***

## The purpose of the project

* To create an applicaition for users to look for defintiions in regards to the game Call Of Duty warzone and understand what terms mean in the game, and also to allow users to create an account for them to create their own definitons for new words and to be able to then update the site aswell as being able to delete their definitions if they arent happy with it. For Data handling, i will be using MongoDB and flask to achieve the Data handling aspect of the application, aswell as using HTML and custom CSS for the website's front-end.

***

## User Experience (UX)

## Strategy

### User Stories

#### First time visitor goals:

As a new user:

* I am looking to understand what certain words/terms mean for the game
* I want the site to be very easy to navigate aswell as being able to use it on other devices aswell
* I would like to be able to create account for the applicaiton to add new definitions

#### Visting User goals:

* As a user, i want to be able to sign up to add new defintions for words for others to see and understand what it means
* As a user, when signing up i would like to have a profile portal that is fully functional and working
* As a user, i want to be able to update defintions of words aswell having the option to delete

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

* An option to edit a word (once they have created an account) that they have added into the dictionary if they feel like they can improve the meaning of it
* An option to delete a word (once they have created an account) that they added into the dictionary
* A access link to the official call of duty website

#### As a developer / business I expect:

* To provide an easy feature for users to register an account
* To provide an easy login page for users to log in once they have succesfully created their account
* To allow registered users to create new words with the definition and add them to the dictionary
* To also allow registered users to only have the choice wether or not they would like to delete or edit their words in the dictionary

## Structure

The website will consits of 3 pages for users that have not logged in,

* A home page which will contain the defintion of words aswell as having search bar, it will also contain some messages for users to understand why the website was designed
* A log in page for users to log in if they have created an account
* A Register page for users who dont have an account can register

The website will consits of 4 pages for users that have an account and are logged in,

* Again, a home page which will contain the defintion of words aswell as having search bar, it will also contain some messages for users to understand why the website was designed
* A profile page which will display the users name to know that they are currently logged in
* An add word paged which will allow the logged in user to add a word into the dictionary
* A logout option for users to log out once they are finished using the site

Also if a user is logged in and have added words into the dictionary they will be able to delete or edit the word at the home page, when clicking the edit button, they will be directed to a new page to edit the word and update the definiton along with the word. Only the user of the created word has acess to this feature

***

## Features

### Navigation Bar:

The navigation bar will be simple black and white,easy to use with the name of COD Dictionary which will have a home, log in and register pages for new users and users who are not logged in. When users log in, it will have a home, profile addwords and a logout link. On smaller devices I have used a dropdown button to display the menu to make it fully responsive.

### Footer:

The footer will contain social media links for users to browse and connect with the site makers. The footer will have an about us section explaining more about the site. The footer will also contain a link to the offical call of duty page.

### Home:

Home page will include an image sliders that will present text to make it visually appealing for all users. It will also contain the word definitions that registerd users create with only them being able to edit and delete any words that they have created. It will also contain a search bar for users to search for words with in the dictionary. There will also be a message for users that will direct them to the register page if they would like to add a new word into the dictionary.

### Log in page:

A log in page for users who have already registered in the past to access their account by inputing their username and password into log in form. It will also contain a carousel slide of images along with a quote underneath it.

### Register page:

A register page for new users to fill in the register form by inputting a username of their choice aswell as a password. It will also contain a carousel slide of images along with a quote underneath it.

### Profile page:

A profile page for users once they log in will be prompted this page with their username showing aswell as a welcome image and welcome text. It will also have a link for the user to be directed to the add words page.

### Add words page:

A page for users to add a new word with a definiton to the dicitionary for other users to see when they access the home page of the site. It will also contain a carousel slide of images along with a quote underneath it.

### Log out:

An option for users who are logged in to log out once they are finished using the site.

### 

***

## Future Features 

A future feature that I would like to add to my website would be more customisable features for users who have an account on their profile page. This would be great for users as they will enjoy using the site even more and will possibly use the site even longer.

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

* For Typography I used google fonts to then apply the oswald font all round the site, and i also used the font-family of Bona Nova for the quotes i have added on some of my pages
* The colour scheme used throughout the page were mainly white, black, and grey/blue grey. I kept the colour theme to a minimum as i felt there was no need to overcomplicate the site as it may distract users from the content and would not look visually appealing. Using materialize css throughout my project i used the color pallete to pick the colors used in my site, using the following: black, blue-grey darken 4, blue-grey darken 2 and blue-grey darken 1

***

## Technonologies Used

### Languages & Frameworks

* HTML5 - Mark-up language used to create the pages for site using semantic structure
* CCS3 - Cascading style sheet used to style the site, aswell as adding media queries to make it responsive for pretty much all devices
* Javascript - Programming language used to create functions working for the site
* Python - Programming language used to control backend development of the site
* Flask - Framework + Extensions
* [Materialize](https://materializecss.com/) - CSS Framework used fro structure, buttons and some styling around the site, aswell as media functions for images
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

### Flask

The application was built using the Flask Famework which is reliant on the jinja templating language. The application was written in python.

Flask-PyMongo - For the applicaition to interact with the MongoDB database

Werkzeug - Used for providing security's, password_hash, check_password_hash

***

## Testing

### Supported Screens:

After using Materialize to build my pages and the use of CSS media queries styles, using the google inspect tool i was able to see that my site is supported for all screens with a width of 280px. I also did some testing by sending my website link to my friends and familys devices and they had seen no issues.

### Supported browsers:

The website link has been tested on Google chrome, Internet Explorer and Microsoft edge, Brave and Firefox and seem to be working fine.

### OS compatability:

Tested on iOS, Android 10, and Windows 10. - I asked a friend with an Android to test that it was working. Tested for responsiveness using Chrome DevTools.

### Peformance Testing:

### Testing User Stories:

### Code Validation:

* All my pages of the website was run through the [HTML Validator](https://validator.w3.org/#validate_by_input), because of flask being a templating language, the code when inputed was not showing the html code being valid, however i copied the html code om within DEV Tools, both by viewing page source and from within the inspect as HTML and pasted it into the validators to check the validity which all pages showed validity

* The [CSS Validator](https://jigsaw.w3.org/css-validator/#validate_by_input) was used to check the validity of my CSS code which turned out to be all fine with no faults

* [jshint](https://jshint.com/) was used to check the validity of my javascript code which turned out to be all fine with no faults

* [Pep8 Online](http://pep8online.com/) was used to check for Pep8 compliances for my python file and test the validity of the code, which the code turned out to be all good

### Fixed bugs:

***

## Deployment

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

* Code insitute tutor support - Provided me with a lot of help support when needed whenever i contacted them

* [Youtube](https://www.youtube.com/) - Provided me with a lot of help when trouble shooting issues

* [Code instiute Task manager mini project](https://github.com/Code-Institute-Solutions/TaskManagerAuth/tree/main/08-SearchingWithinTheDatabase) Provided me with a lot of help intialising the development process of the site aswell as setting up MONGO DB with the site, it also helped me with understanding more on python and how it works

### Content:

I asked friends and family to create a profile and add definitions to the site to see if it works effectively

Code & Content (not already attributed): Adil Khair

### Inspiration:

* Inspiration was taken from the [Code instiute Task manager mini project](https://github.com/Code-Institute-Solutions/TaskManagerAuth/tree/main/08-SearchingWithinTheDatabase) to help gain an idea of how to structure my site and more idea on developing the backend side of my site

* The idea of the site came from the game [Call of Duty](https://www.callofduty.com/uk/en/home), as a player of the game, i thought this would be a great idea for me to create an online dictionary based on the many terms used in the game where new players may not understand words that are being said by other players


