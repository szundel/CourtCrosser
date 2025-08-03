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
