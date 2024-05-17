# Assigment 1

This Node.js module allows its users to browse, add, delete and search songs, 

## Getting Started

To use this module in your Node.js project, follow these steps:

Install Node.js if you have not already done so.
Download Lennard_music.js file and put it into your project directory.
Create a file named music.js.
Require the module in your music.js file:
```
const musicLibrary = require('./TayWaiSeng301.js');
```
### Music.js code

```
musicLibrary.addSong("Michael Jackson", "They Don't Care About Us", "Album1 HIStory: Past, Present and Future, Book I", "16/04/1996", "4:44 ", "Pop");
musicLibrary.addSong("Steve Jablonsky ", "Arrival To Earth", "Transformer Score", "25/06/2007", "5:27", "	Film score");
musicLibrary.addSong("Linkin Park", "What I've", "Minutes to Midnights", "01/04/2007", "5:00", "Hard Rock");
musicLibrary.addSong("Angela Zhang ", "yin xin de chi bang", " Zhang Shao Han", "11/07/2010", "3:27", "Chinese pop");


// Search songs by genre
const popSongs = musicLibrary.findSongsByGenre('Pop');
musicLibrary.logSongs(popSongs);


// View all songs in the library
musicLibrary.viewAllSongs();


// Delete songs by artist
musicLibrary.deleteSongsByArtist("Artist1");
musicLibrary.viewAllSongs();

// Delete a song by title
musicLibrary.deleteSongByTitle("Song2");
musicLibrary.viewAllSongs();

//play song
music.library.playsong('yin xin de chi bang');
```

### Fuction

addSong(artist, title, album, releaseDate, duration, genre): Allows you to add any song with the details.
deleteSongsByArtist(artist): Deletes songs by the artist.
deleteSongByTitle(title): Deletes a song by its title.
findSongsByGenre(genre): Searches for songs by their genre.
logSongs(songs): Logs songs by genre.
viewAllSongs(): Displays all the songs in the database.
playsong(): play the song if given the name in the database.


