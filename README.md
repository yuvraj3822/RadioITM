# RadioITM
*This application basically performs the 2 function streaming the audio and displaying the current and recent list of tracks.

*In this application MVVM, Coroutines and Room Persistence Data has been used in Kotlin.
*Here in the splash screen api is being called and stored in database
*Where in the dashboard it represent the data saved in Db
*To have the recent data it also has the pull to refresh

*Audio streaming is done via media player.
*Foreground service is being used to play the audio.
*Media player declared with singleton to access its start pause stop from from other classes 


Problem I faced during in the media player is 
* After releiving the player resources and stopping it still retain the instance.

Shortcut I used is 
* I didnt used the seprate Repository class for the api call or local data. Just called directly in the viewmodel

Things that could be used in this are
* Databinding with binding adapters and Navigation graph

