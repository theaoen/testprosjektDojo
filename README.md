# testprosjektDojo

How to create a React Native project with Expo: 

#Setting up Expo
There are a couple of requirements for Expo to work as planned. 

1.	First, make sure that you have the Expo app installed on your device. 
2.	Install NodeJS from this link: https://nodejs.org/en/ 
3.	Node also installs npm for you, but probably not the latest version. It’s therefore a good idea to update it asap by typing:

    npm install -g npm@latest
    
You should then install the command line tool for Expo. 
This will run locally to package, serve and publish your project. 
    
    npm install exp --global
   

#Creating your first project and opening it in Expo
1.	You’ll probably be asked to create an Expo account before proceeding. The following commands will create a project in the folder you are currently in, so navigate somewhere you’d want those project files to be saved. You’ll get the option to start out with a template or a clean project. 
    exp init my-new-project
    cd my-new-project
    exp start


2.	To start your project, navigate to it and start by typing the following. 
    cd dojoProject
    exp start


3.	The terminal window will now show instructions on how to open this project on a physical device. For Android devices you simply scan the QR code that is showing in the window. For iOS type 


    exp send -s < phone(+47) or email>


You’ll get notified with a link that allows you to open your project in the Expo app. 


#Adding an existing project to Git
1.	Start by creating a new repository in Github. You do not need to initialize it at this point. 
2.	Use terminal to navigate to the folder where your current project exists. 
3.	Initialize this local directory as a Git repository by typing

    git init


4.	Add the files in your local repository and stage them for commit by typing


    git add .


5.	Commit the staged files: 

    git commit -m ‘First Commit’


6.	Make sure that you copy the remote repository URL that you’ll find on top of your new GitHub repository. In terminal, add this URL to the code below. This sets the new remote.  

    git remote add origin <remote-repository-url>


7.	Verify the new remote by typing

    git remote -v


8.	Push the changes/files in your local repository to GitHub. You’ll be asked to type in your username and password for GitHub. If you have two-factor authentication activated on your account, the regular password will not be sufficient. You’ll then have to create a Personal access token at the GitHub website and use this to log in. 

    git push origin master




