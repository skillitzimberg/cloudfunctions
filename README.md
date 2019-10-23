I am learning how to use and generally deal with Firebase Cloud Functions. Here I am documenting the steps I took, am taking, to get a simple project to work.  

I found, am finding this to be very confusing due to the many possible paths a person can take depending on what they are trying to accomplish.

What I am trying to accomplish: 
* I want to write functions and test them locally before I deploy them.
* I want these functions to use the project's Firebase database. The data is live. (It looks like there is a way to do this locally as well, but one thing at a time . . .)
* I want to deploy these functions.
* I want to write more functions and test them locally in conjunction with the deployed functions.  

Setting up the basic app  
I started [here](https://firebase.google.com/docs/functions/get-started) not realizing that although this does get you a basic cloud functions app set up, it assumes you're ready to deploy and pretty much stops there. I went through this process at least twice, this app being the second version. On this round I did NOT deploy the functions. I got the project set up, then skipped to testing locally.  


Adding Firebase to the app  
Following instructions here: [Get Started With Firebase](https://firebase.google.com/docs/web/setup):  
* I went to my [Firebase Console](https://console.firebase.google.com/).  
* I [created](https://firebase.google.com/docs/web/setup#create-project) a Firebase project called "cloudfunctions".  
* I [registered](https://firebase.google.com/docs/web/setup#register-app) my app.  
    - I would say that this is the one of the first things that could use clarification. To what are they referring when they say "your app"? I took it to mean the directory in which I will be building or already have built and application. For this project that directory is "/Users/ForeignFood/Development/cloudfunctions/".
* I added the [Firebase SDK and initialized Firebase](https://firebase.google.com/docs/web/setup#add-sdks-initialize).  
* I added my [Firebase config object](https://firebase.google.com/docs/web/setup#config-object). I got the object using the instructions [here](https://support.google.com/firebase/answer/7015592). 
* I did NOT install [Firebase hosting](https://firebase.google.com/docs/web/setup#install-cli_deploy).  

