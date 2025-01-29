Requirements

For development, you will only need Node.js and the universal Node package, Yarn, installed in your environment.

Node

Installing Node on Windows

Just head over to the official Node.js website and download the installer. Also make sure you have git in your PATH, npm might need it (you can find git here).

Installing Node on Ubuntu

You can install nodejs and npm easily using apt install, just run the following commands.

$ sudo apt install nodejs $ sudo apt install npm

Other Operating Systems

You can find more information about installation on the official Node.js website and the official NPM website.

If the installation is successful, you should be able to run the following command.

$ node --version v8.11.3 $ npm --version 6.1.0

If you need to update npm, you can do so using npm! Great, right?  After running the following command, just open the command line again and you should be good to go.

$ npm install npm -g 

Install

Just clone the repository

git clone https://github.com/mostlypanda/Text-Translator-using-Nodejs.git 

Now head to the code directory

cd Text-Translator-using-Nodejs 

Install all dependencies

npm install 

Application configuration

Now you need to create a file named .env containing the database link to connect to Mongoose and just save it and you should be good to go.

Run the project

npm start 

Application structure

/app.js - This is the main of the app having code of all the API's and app formation and listening and DB connection /Language DB/ languages.js - This file contains all the languages ​​supported by the app and their manipulations.  /Models/ model.js - This contains the schema of cache object /Assets - Contains image assets for Readme 

 API format

 The REST API endpoint is '/api/translate/' And the format of data to be send via the API in the body of API { "to" : "chinese simplified", "from" : "English", "text" : "That person is calling you" } where 'to' is the target language 'from' is language of given text 'text' is the data to be translated.
 
