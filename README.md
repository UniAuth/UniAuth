# UniAuth

alright pack, here it is.

## TLDR
I had a plan to create an authentication system that'd allow us to have a central data storage and could be used in other projects that we do, and guess what, the MVP is done, and if you're interested in building this onward, time to hop in.

## The Problem
When working on different projects in our club, Google OAuth was our way to. Users and developers both like this sytem because:
1. It ensures that user are actually authorized to use the email the logged in with.
2. Prevents bruteforce.
3. Users do not like registering at sites.
4. Users do not need to enter their details at every site.
5. Users are **not concerned about security issues**. There have been cases when systems had minor bugs and exposed user data and sometimes even unhashed passwords.


The limitation of using Google or any other provider's auth is that 
1. We can not store details about users. For example: students have registration number, users have various social accounts like github, dribble, youtube, twitter, stack overflow which the application might request.
2. Since there is no method to achieve the above, it becomes the task of the application developer to get these details from the user. This also means that the application developer is also tasked to ensure that these details are valid, which means manually integrating these services for their APIs.
3. Customization: there are limited **scopres** that the application developer can use, which means that there is no method to get very specific data about user from the server.

## The solution -> UniAuth
UniAuth has been created to solve the above mentioned problems, and also support more features that make life less painful. UniAuth aims to provide **all features, and more**. For example, client applications registed on UniAuth also provide a dashboard which the developers can use to get metrics.
