# Final-cpp Project (Weather App)

Loads Weather info from selected Cities

## Authored by:
 Mohammad Abu Khdier  && Mohammad Abd al-Aziz

## Link
[Project](https://postjceac-my.sharepoint.com/:f:/g/personal/mohammadabk_post_jce_ac_il/Eh27Ie6OAv5BkaGmCaDP6lYBzQZag-6iv1ObWFVO3ls70A)

 ## Features
 - Search Cities by name
 - set cities as Favourites
 - remove cities from list

 ### Setup
- Follow the link in the gitHub to the drive
- Downlaod the zip file from the drive
- unzip it and run the .sln file to open up visual studio
- or download the Release folder with everything already setup

### Usage
- set the connected app as the startup
- inside visual studio run the project by pressing F5
- or run the .exe from the Release folder

![](./digram.drawio.svg)

### Files
- apiAccess.cpp:  uses the api to get info about a city
- CommonObects.h: has the object defenations being passed between threads
- ConnnectedApp.cpp: starts and runs both threads connects the gui with the backround process
- DownloadThread.cpp: uses the apiAccess class and parses the recived info using json and inputs into a WeatherBody Object
- DrawThread.cpp: starts the gui interface and defines all the features in it
- fileHandler: makes the directory for Faviorted cities and manages the created file
- WeatherBody: recives json object and translates it to approprite fields
