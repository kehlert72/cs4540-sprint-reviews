# Townie Cup (Flutter)
This is the townie cup project that utilizes flutter. The application is for the Townie Cup tournament. This is an app for Dr. Green and it includes several projects. These projects include API, Android, iOS, public website, and admin website.



The public website can be accessed here, https://towniecup.com/

## Flutter
#### Summary

The UI is split into multiple files and the different pages are separated via different classes. The code for Dart translates between both iOS and Android.

#### UI

**Login:** The page the user logins into the menu

**Leaderboard:** Consists of list tiles that make use of the padding widget.

**Dashboard:** Consists of a collection of buttons that navigate you to the different pages in the application.

**Contact Us:** Gives the user contact info and a place they can see the next date of the event

**Menu:** Gives you the ability to navigate through the different pages



#### Scorecard

Each score card displays all of the holes and the information on each hole. Then, when each list tile is clicked they pop up a dialog that allows the user to edit the number of strokes. Once, the user enters the data and the data has been pushed to the server the list that contains the data is also updated.



#### Navigation

The navigation consists of the login page that allows you to move between any other page, however, you have to move back to the login page before you can navigate to any other page. The different pages are contained in a array, where you must use push to add a new page and pop to remove a page from the array. Additionally, each page is contained within a class, which returns the widget that holds the contents of the page.



#### Tests

The tests consists of modules which tests something specific to the program. There are tests for the UI to ensure everything that is there exists. All of these tests are contained under the folder tests and in the file widget_test.



#### Resources:

* [Flutter Docs](https://flutter.dev/docs)
* [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
* [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)



## Android

This project consists of Fragments in order to modularize code. The goal is to create a more sophisticated UI that is still maintainable. The Fragments belong to an Activity that can be restarted when that Activity is restarted. Once, the Activity is destroyed, the Fragment is also destroyed.

The Android UI and the iOS UI are still completely separate projects. Due to the refactoring of the iOS app the iOS app is ahead of the Android app. This creates a different user experience on the same app for the different operating systems. Flutter streamlines the UI, so that the UI can be changed once in Flutter. Changes in one project will apply to both projects, however, the code will have to be changed separately as they use different programming languages.

## iOS
The IOS app uses a profile to install all dependencies. The app itself is written in Swift, and uses a lot of different controllers which appear to modify the UI.

## API

For the leaderboard the API sends the data for the tournaments, holes, and teams all at once. Though the teams data also includes the scores and members table as well. This adds to the complexity of the query and is unnecessary, which should be refactored. For the score card it sends tournament, holes, and teams.

The API sends all the data that may be needed at once and you have to pick and choose what you want. This is confusing at first but can be maniplated in good ways. 
Tournament has information on the tournament
Holes has all the data on each hole.
Teams has all the teams that are in this year's tournament, The score of said team, and the members of said team.

With the way the API is set up you can fetch all the hole data that you need, while also having access to the team scores. This is very handy for building the scorecards. 

## Public Website

## Admin Website