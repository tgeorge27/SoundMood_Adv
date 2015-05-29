# Project: SoundMood 

![image](https://imgur.com/VrWE2CS.jpg)

##Scope
You have just been hired as a consultant for Sound Inc. A brand new streaming music service. 
You have been tasked to create a webapp that can play songs based on how the user is feeling. 
Your manager has given you a deadline of one week to complete this project and has provided you with a wireframe for the webapp.  

##Project Description
Your Manager has laid out the following requirements for the project: 

* This project must use the SoundCloud API
* The user must be able to input an array of moods and hear a song that reflects their mood
* The song title and artist must appear while the song is playing
* There must be a random button that will play a song based on a randomly chosen mood

Your Manager has offered a stipend a $500 for each of the bonus requirements listed below: 

* Change the color of the jumbotron to match the user's mood
* Add Bootstrap typeahead to the `#mood` input field


##References

* https://developers.soundcloud.com/docs/api/guide
* https://www.youtube.com/watch?v=B9vPoCOP7oY
 

##Instructions
You are given Starter Code for this project which you must clone into your own workspace.
You will notice that there are comments inside the script.js file that provide instructions for how components of this project can be made.  

####In order to make Soundmood functional! You will need to complete the four tasks below:

###1) Play a track

Play a track using the Soundcloud API (Reading the Soundcloud documentation will help you figure out how to play a track)

1. Read the Soundcloud documentation to figure out how to **stream** (or play) a track
```
HTTP API GUIDE -> Playing Sounds ->  Streaming sounds
```
2. Use `SC.stream` to play a track
  * Hint: you need to know something about the track
3. Fill out the `playOneTrack()` function
  * Hint: don’t forget to add `playOneTrack()` to `document.ready()`

###2) Add click handlers

Add a click handler for the `#go` button -- make the `#go` button DO something by adding a click handler!

* Hint: you can use Javascript or jQuery for this
* Hint: call the click handler `playOneTrack()` to play a song when you click the button

###3) Find a track based on the user's mood and play it

Find a track based on the user’s mood and play it -- make the click handler play a song based on the user's input!

1. **Fill out the `goClicked()` function! It should:**
  1. Get the user's input from the `#mood` field
  2. Call `searchTracks(mood)`.
    * Hint: there are helper methods in `script.js` that you can use!
2. **Fill out `searchTracks(mood)`**
  1. Read API documentation to find `SC.get`
  2. Fill out `searchTracks()` to find the track for the user's mood using `SC.get`
  4. Make sure to `console.log()` the response from the API so you can see what it returned!
  3. Get the track's `id`
  4. Call `playTrack(id)`
  5. BONUS: Update jumbotron `#songtitle` to display the song title
3. **Fill out `playTrack()`**
  1. Make sure to keep track of the song you are playing by storing it in `currentSong`
  2. Play the track for the given `id`
    * Hint: look at `playOneTrack()` for help

###4) Randomization: Make the random button work!

1. Fill out the `moodList` array with 10 moods/emotions
  * ex. 'happy', 'sad'
2. Add `#random` button click handler
3. Fill out `randomClicked()` + `randomMood()`


##Vocabulary

* API
* Click Handler
* Documentation
* Color gradient

##How to Submit
This project must be pushed back up to your repo on GitHub. 

##Homework
Instructor will assign homework based on progress in class.