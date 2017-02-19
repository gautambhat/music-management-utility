# music-management-utility
Shell-based Music Management Utility for Linux

Gives user the flexibility to manage the entire MP3 files on the system and the freedom of listening to MP3 song of his choice. It provides multi-user functionality, so each user when login in to his account, has its own separate list for its MP3 files.

MMU is broadly classified into 4 modules: 

1. It keeps track of the existing and deleted MP3 files in the system.
2. List all the MP3 files at any instant of time.
3. Listening to MP3 file randomly.
4. Searching and listening to song by Artist, Album or keyword choice (A great advantage to keep track with detailed meta info...)

##Detailed specification:

1. There is a scanning utility which helps the user to search all the MP3 files in the systema/c to given directory permission to the user. Then it creates a temporary file from the scanned result and compares it with the existing list of MP3 file in the system, if finds new songs, then it add to the original existing list, and if it finds that some existing files are missed or deleted by the user, and then it removes the meta info from the existing list. And if there is no existing MP3 list present in the system, then it creates a new list for the user.
2. Compile the result from first module and displays the final list of MP3 files that belong to user.
3. We can play the songs from the user‟s MP3 list in random manner.
4. This module gives user a great flexibility, where user can search a MP3 files by its artist, album name or keyword search. And user has the choice to play the selected MP3 file and to view it in GUI explorer in the directory where they are placed.

##Software Required to run this utility:

- **VLC Player for linux system**: To play the MP3
- **MediaInfo**: A C program that extract the 128 bytes header information from MP3 File.
..*Information regarding Artist, Album/Performer, Track and Title details.

_Download MediaInfo from internet, it is an open source C code_

- **Platform Required**: Any Linux based platform for 32 bit and 64bit

####How to run:	
While working in user home directory, run the script file by specifying its path.

Depending on the user which is logged in to the system, the utility will check if a paylist is already created or not. If not, it will scan the system for music files and create a playlist.

The user can then follow the on screen instructions to proceed, manage or play his/her music.
