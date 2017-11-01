# *Frinder* [![Build status](https://travis-ci.org/frinder/frinder-app.svg?branch=master)](https://travis-ci.org/frinder/frinder-app/builds)

**Frinder** is an android app that matches you with people nearby who are also looking to meet new people (not focussed on dating).

Have you found yourself in the following situations when you were bored and could use some conversation? 
- Waiting for a flight alone 
- Taking the train by yourself 
- At a bar alone
- Having a meal by yourself at your office cafe  

We are sure everyone has some time been in such a situation where they were alone and wouldn't mind meeting a new person. However, the initial conversation or ice-breaker can be particularly awkward.

This app links to your Facebook profile and has a profile that contains basic information about you. On opening the app, you can see nearby people in the area and sent them a notification incase you'd like to meet them. Similar to Tinder, the app notifies you only when the other person reciprocates interest in meeting you. Some additions to this would be a chat functionality and the ability to create interest-based groups (e.g. an IoT focussed ad-hoc group at a computer science conference).

## User Stories

Profile
* [X] User can sign into Frinder using Facebook login
* [X] Query user profile data from facebook
* [X] User can click on a person to view their detailed profile
* [X] User can edit/fill their profile (desc, choose interests)

Discover Users
* [X] User can view list of active people nearby
* [X] Ask for the required permissions (location)
* [X] Update the server with the user's location updates
* [X] User can edit their search settings (radius, gender, age, interest, turn off discoverability)
* [X] Setup geofire for faster location queries
* [x] Auto refresh discover feed

Requests
* [X] In a notification view, user can view their friend request(s) and contact details of accepted friends
  * [X] Use Fragments + Tabs to differentiate between sent, received and accepted requests
* [X] Update the server with responses to the requests
* [X] Add an unread mechanism to highlight new request
* [X] Add in-app badging to notify user about new requests

Messaging
* [X] User can send/receive messages in the app
* [X] Add a messages view to view your recent messages
* [x] Observe changes to the message thread and thread list while on the view and update UI
* [x] Add in-app badging for unread messages

General
* [x] Setup firebase
* [x] Error handling (permissions, internet connectivity)
* [X] Setup automated builds to catch build failures
* [X] Create scripts to help with testing
  * [x] Add scripts to generate data for random users along with profile pictures
  * [x] Add scripts to clean up/update db entries on changes to the scheme
  * [x] Add scripts to clear data added while testing

User interface
* [x] Explore different list view options (card stack, single card)
* [x] Improve the UI of the app (icons, color scheme, launch screen)

Bonus
* [x] Show a list of suggested nearby places to help choose the location for the initial meet (hooked to Facebook Place search)
* [x] Allow the user to ephemerally share their location so as to allow new contacts to find them
* [x] Add app shortcuts to allow users to easily perform certain actions
* [ ] Fire push notifications to notify users when the app is not active

Ambitious:
* [ ] Find common attributes with the person
  * [ ] Mutual friends
  * [ ] Similar visited places
  * [ ] (very ambitious) Common interests
* [ ] Link to Instagram and LinkedIn accounts
* [ ] Show people around you on a map
* [ ] On meeting, support sharing contact details via NFC
* [ ] Extending chat to VoIP calls
* [ ] Allow group meetups

## Walkthroughs

Sprint 3

[![Sprint 3 Walkthrough](https://user-images.githubusercontent.com/1111292/32263236-1621d046-be96-11e7-955e-3f6c05825cc0.png)]](https://www.youtube.com/watch?v=kgYTNTG9ht0&feature=youtu.be)

Sprint 2

![Sprint 2 Walkthrough - User logging into app for the first time](https://i.imgur.com/8d9zsQr.gif) ![Sprint 2 Walkthrough - User logging into app again](https://i.imgur.com/eB4oOkB.gif) ![Sprint 2 Walkthrough - Showing settings screen](https://i.imgur.com/u3u2nst.gif)

Sprint 1

![Sprint 1 Walkthrough](https://imgur.com/gBtGWj1.gif)

## Wireframe

![Sprint 1 Wireframe](https://user-images.githubusercontent.com/1111292/31313212-b4bbb4d8-ab90-11e7-9346-af22cdf64056.JPG)

## Open-source libraries used

- [Glide](https://github.com/bumptech/glide) - Image loading and caching library for Android
- [ButterKnife](https://github.com/JakeWharton/butterknife) - Bind Android views and callbacks to fields and methods
