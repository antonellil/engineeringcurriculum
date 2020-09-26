Welcome to the software engineering curriculum!

To start create a git account on https://www.github.com and download this curriculum to your computer. This can be done by:

1. Opening Terminal
2. Navigating to the folder you want to put this in by using the `cd` command
3. Typing `git checkout https://github.com/antonellil/engineeringcurriculum.git` and hitting enter to download

Next, install the following:

- Sublime Text 3 https://www.sublimetext.com/3

- Google Chrome https://www.google.com/chrome/

# 1) Computer overview

## Terminal and local fileystem navigation

- Terminal is just another way to interact with the computer and view files and run programs
  - cd, ls for navigating and viewing files
  - mkdir for creating folders, touch for making new empty files
  - rm to remove a file or directory
  - mv to move a file or directory

## Git

- git is a way to save your local files in the cloud
- it allows you to look at the history changes to those files and share with others

# 2) Sublime editor overview

- Glorified text editor
- Has plugins that help with development
  - Color-coding of syntax
  - Shows warnings and errors for syntax and some coding logic

# 3) Separation of concerns with front-end/back-end client/server

- Client is what users interact with (web browser, iOS, Android, desktop apps)
- Server is what the client talks to in order to send and retrieve things from the client
  - Server is just a computer somewhere that the client talks to
  - Server often uses a database to store things long-term

# 4) Client

- Tons of ways to code the client, but the current way its often done is primarily in JavaScript because thats what the web browser uses
- Role of the client is to display things to the user and take user input
  - In the web browser, HTML and CSS are used for layout and display
  - On iOS and Android, there are has similar layout and styling concepts to HTML and CSS
  - JavaScript is used for user input
- Building practical client-side things
  - Calendar
  - Selfie photo album

# 5) Server

- Node overview and tutorials
- Role of the server (web server, background processing server)
- Building practical server-side things
  - Scraping
  - Database storage

# 6) Database

- PostgreSQL overview and tutorials
- Role of the database (storage, retrieval)
- Building practical database tables and usage

# 7) Caching

- Redis overview and tutorials
- Role of caching (often-accessed values, limiting database reads)
- Building practical things with caching

# 8) End-to-end

- Build several applications end-to-end through all layers of the stack
