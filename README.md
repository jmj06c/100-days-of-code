# I've joined the #100DaysOfCode Challenge.

## Contents
* [Rules](rules.md)
* [Log - click here to see my progress](log.md)
* [FAQ](FAQ.md)
* [Resources](resources.md)

## If you've decided to join:
1. Read [Join the #100DaysOfCode](https://medium.freecodecamp.com/join-the-100daysofcode-556ddb4579e4)
2. Fork this repo and commit to the [Log](log.md) daily. [Example](https://github.com/Kallaway/100-days-kallaway-log).
3. **Code minimum an hour every day for the next 100 days.**
4. Change the date in [Rules](rules.md) to the day you've started the challenge.
5. Delete the examples in the log, or comment them out, and start filling it with your own content.
6. **Tweet your progress every day using the #100DaysOfCode hashtag.**
7. Follow [100DaysOfCode](https://twitter.com/_100DaysOfCode) Twitter Bot that retweets all the tweets that contain the #100DaysOfCode hashtag. It's a great way to keep yourself motivated and to participate in the community. Thanks [@amanhimself](https://twitter.com/amanhimself) for creating it!
8. Important: Encourage others who are doing the same challenge on Twitter or elsewhere - by giving them props when they are posting updates on their progress, supporting them when things get difficult. Thus we will grow a community that is helpful and effective, which will lead to a higher success rate for each person involved. It's also more likely that you will stick to your own commitment, given that you will get acquainted with a couple people (or more) right away.
9. If you find a great, helpful resource that others would benefit from, either submit a Pull Request to add it to the repo, or just tweet at me (see info below)

Refreshist is my website and my mobile app - A progressive web app that shares news, photos, videos and more about me. 
The top 7 people in my life have access to this app for comments - All who download it for mobile and aren't of the top 7 can only view. 
Built with Polymer 2.x, Xcode, Homebrew, Bower, Firebase,

**Working in Native Default Terminal OSX**
$brew install node //READ all WARNINGS and fix as needed or gitter me for help @st.fresh
$npm install -g polymer-cli
$npm install -g bower
$npm install -g firebase-tools
$firebase version //make sure you get `3.2.1` or higher if `no command found` refer to [Line 27]
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

**Add the line below [line 33] to bash_profile on a new line of its own**
export PATH="/home/your-username/npm-global/bin:$PATH" # Add npm bin PATH
//for me `export PATH="/Users/jonathanjames/.npm-packages/bin:$PATH"`
$source ~/.bash_profile //reapply profile to shell for CLI 
$firebase version //make sure you get `3.2.1` or higher if no refer to [Line 20] if no gitter me @st.fresh with your bash_profile

**Firebase logout situation**
$Firebase logout //if you auth'd with a gmail that isn't connected to your https://console.firebase.google.com/
$Firebase login //execute this again with browser ready - meaning browser already signed into proper gmail account 
//`$Firebase login` should return `Success! Logged in as your-email@gmail.com`
