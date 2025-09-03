# CourtCrosser
Mobile IOS, Android, and Web application built for organizing and recording pickleball meetups.

## Code Stack
Client and front end code is built using React Native for IOS, Web, and Android. The backend server code is a nodejs application hosted in google cloud and using a Supabase database.

Content is controlled in a separate repository and is hosted in a StrapiJS app that allows authors to manage and edit content such as images and text.

## UX
### Records Health Data
App records meetups like Strava displaying health data recorded from watches and devices such as apple watch and Garmin watch.

### Meetup
Has a call for meetup feature. Users post a date, time, and location to meetup with local pickleball players. Meetups are shown to other users in the geographical area.

Push notifications can be sent out to users.

Meetups can be filtered by location, players (only receive notifications from friends and trusted associates), by skill level (cross couter score), or by game type such as doubles matches.

### Safety
CourtCrosser places importance on physical safety to not disclose location data to any other users without permission to view it.

For safety meetups keeps names anonymous.

Reporting feature. Feature that allows users to report other users who they believe may be unsafe or violent.

Additional data is also tracked such as a streak score similar to duolingo, but the streak can be adjusted to the players schedule such as by weekday, weekend, etc.

Badges are also awarded, such as those found in Strava for taking certain actions such as defeating another players, playing your first game, recording matches, meeeting a streak goal, leveling up, etc.

### Shop
A shop will be displayed allowing people to purchase CrossCourter gear featuring the logo, their level, streak, etc.

## Premium Features
Premium features require a monthly subscription. Allows serious pickleballers to filter their meetups to people at their general pickleball level. Level is determined by CourtCrosser Score above.

### CourtCrosser Score
A central feature of the application is a gamification. Users can level up by defeating players with higher scores and level down by losing to players with lower scores.

### App Appearance
The icon for the app across all platforms exists here in this repo.

The app will be built with a nav menu across the bottom using the titles: "Menu", "Profile", "Schedule", "History" and "Record"

#### Menu
Menu button takes the user to a menu page where they can find more buttons to navigate through the rest of the app. The menu button will include links to other pages.

Additional pages will include:
* Health - this link takes the user to a page with health and fitness records such as heart rate, weight, active weekly minutes.
* Report - this is a reporting feature. If the person you meetup with presents any perceived dangers users should report them
* Meetup - This is a scheduling feature meant to schedule an upcoming event. Creat
* Notifications - Notifications includes both the type of notifications (e.g. email, in app messages) as well as the subcriptions (i.e. which communications do you want to receive). Some of the important notification settings will be centered around which meetups to subscribe to. 

##### Subscriptions
* Meetups
  * meetups within specified distance (e.g. 5 miles)
  * meetups organized by a set of users (e.g. previous players)
  * meetups that include players above or between a certain crosscourter score
  * meetups at a specific gym
  * official tournaments 
* Account notifications
  * account deletion
  * payments due

#### Profile
The Profile button contains most of the users personal information stored as settings. These items include their most frequently used court locations to play at, their common partners, their cross courter score value, email address, payment info, and their picture.

For some meetups a recent photo is required to allow other cross courters to see who they will be playing meeting up with. Users who do not use a recognizable photo will be reported and their recent matches will be invalidated.

There will also be a link on this page used to reset a users password, setup 2FA, or setup a passkey.

Payment methods will also be included and recorded on this page.

Player ID numbers along with a scannable QR code will be added to this page allowing players to use the record feature.

#### Schedule
The schedule page shows all upcoming events in orderwith the most recent at the top and the events farther in the future showing below them. Each item in the schedule will show the Title of the event, the location where it will be played, the time and date when it will occurr, an image of the venue, and any familiar crosscourt atheletes that are currently planning to attend.

Clicking on a scheduled item will show more information as well as allow the players to resolve issues such as making payments to the scheduled event planners.

#### Record
The record section provides an easy mobile friendly page to record the score.

To start a match a user must click "record", which begin an NFC connection with another cell phone. When the connection is opened the user will be shown a loading image such as a spinner, but will also be provided with a button that says "try another method". Clicking "try another method" will allow players to link up using a QR code (shown in their profile). Other methods will include a search feature for the players name and a id number lookup.

Matches can be recorded by a single individual allowing all players to "Agree", or they can be submitted and recorded privately. All scores must be agreed upon by all players for a score to become a stored and saved official match and allowing the match to affect a players score.
