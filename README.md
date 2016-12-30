# I've joined the #100DaysOfCode Challenge.

## Contents
* [Rules](rules.md)
* [Log - click here to see my progress](log.md)
* [FAQ](FAQ.md)
* [Resources](resources.md)

# Project I: Refreshist Progressive Web App for me and 7 others

Refreshist is my website and my mobile app - A progressive web app that shares news, photos, videos and more about me. 
The top 7 people in my life have access to this app for comments - All who download it for mobile and aren't of the top 7 can only view. 
Built with Node, Polymer 2.x, Xcode, Homebrew, Bower, Firebase

**Working in Native Default Terminal OSX**
$brew install node //READ all WARNINGS and fix as needed or gitter me for help @st.fresh
$npm install -g polymer-cli
$npm install -g bower
$npm install -g firebase-tools
$firebase version //make sure you get `3.2.1` or higher if `no command found` refer to [Firebase in CLI errors (below)]
$firebase login //careful here, it will auth using Safari.. so your gmail account that's auth'd with Safari will be used.. needs to be same gmail that you setup at https://console.firebase.google.com/

**Working inside your repo or local top-level directory**
$mkdir app-name //all your stuff goes in this folder called `app-name` 
//I highly suggest you connect this folder to git and utilize branching for this project
//Git setup & repo creation: https://www.atlassian.com/git/tutorials/what-is-version-control
//Git branching practice: http://learngitbranching.js.org/  
$cd app-name //make sure last part of CLI prompt is `/app-name$` before proceeding!!
$firebase init //lots of options here and things to read.. standby

**Node upgrades**
$brew upgrade node //READ all WARNINGS and fix as needed or gitter me for help @st.fresh

**Homebrew upgrades**
$brew upgrade //READ all WARNINGS and fix as needed or gitter me for help @st.fresh

**Firebase in CLI errors**
$npm get prefix //Should return something like `/home/your-username/npm-global` 
//but mine returned `/Users/jonathanjames/.npm-packages` on Mac OSX
$nano ~/.bash_profile //some say `~/.bashrc` ? idk! nano edit both?

**Add the line below [line 43] to bash_profile on a new line of its own**
43 export PATH="/home/your-username/npm-global/bin:$PATH" # Add npm bin PATH
//for me `export PATH="/Users/jonathanjames/.npm-packages/bin:$PATH"`
$source ~/.bash_profile //reapply profile to shell for CLI 
$firebase version //make sure you get `3.2.1` or higher if still `no command found` gitter me @st.fresh with your bash_profile

**Firebase logout situation**
$Firebase logout //if you auth'd with a gmail that isn't connected to your https://console.firebase.google.com/
$Firebase login //execute this again with browser ready - meaning browser already signed into proper gmail account 
//`$Firebase login` should return `Success! Logged in as your-email@gmail.com`
