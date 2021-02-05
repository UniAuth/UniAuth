# UniAuth

## TLDR
I had a plan to create an authentication system that'd allow us to have a central data storage and could be used in other projects that we do, and guess what, the MVP is done, and if you're interested in building this onward, time to hop in.

## The Problem
When working on different projects in our club, Google OAuth was our way to. Users and developers both like this system because:
1. It ensures that users are actually authorized to use the email they logged in with.
2. Prevents brute force.
3. Users do not like registering at sites.
4. Users do not need to enter their details at every site.
5. Users are **not concerned about security issues**. There have been cases when systems had minor bugs and exposed user data and sometimes even unhashed passwords.


The limitation of using Google or any other provider's auth is that 
1. We can not store details about users. For example, students have a registration number, users have various social accounts like Github, dribble, youtube, Twitter, stack overflow which the application might request.
2. Since there is no method to achieve the above, it becomes the task of the application developer to get these details from the user. This also means that the application developer is also tasked to ensure that these details are valid, which means manually integrating these services for their APIs.
3. Customization: there are limited **scopes** that the application developer can use, which means that there is no method to get very specific data about the user from the server.

## The solution -> UniAuth
UniAuth has been created to solve the above-mentioned problems, and also support more features that make life less painful. UniAuth aims to provide **all features, and more**. For example, client applications registered on UniAuth also provide a dashboard that the developers can use to get metrics.

## Getting Involved
The project needs integration with major programming languages, so we're welcoming to all developers. 

All components of this project are available on [UniAuth Github Organization](https://github.com/UniAuth) with a free license.

The [roadmap for an overall development status](https://github.com/UniAuth/UniAuth/projects/1) is also publicly available.  If you want to recommend some changes / propose new plans / new features / discuss current features, please do so by [opening an issue](https://github.com/UniAuth/UniAuth/issues/new/choose). 
