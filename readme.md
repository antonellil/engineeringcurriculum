# Welcome to the software engineering curriculum!

To start create an account on https://www.github.com. Next, you can download this curriculum to your computer by:

1. Opening Terminal
2. Navigating to the folder you want to use for the curriculum by using the `cd` command
3. Typing `git clone https://github.com/antonellil/engineeringcurriculum.git` and hitting enter to download

Next, install the following:

- Sublime Text 3 (a nice text editor) https://www.sublimetext.com/3
- Google Chrome (a modern web browser) https://www.google.com/chrome/

## 1) Your computer

### Terminal and local fileystem navigation

- Terminal is just another way to interact with the computer and view files and run programs
  - `cd` is used for moving through folders. you can type `cd FolderName` to go into a folder named "FolderName" and you can use `cd ..` to move up a level
  - `ls` is used for viewing the files in the current folder
  - `mkdir` is used for creating folders
  - `touch` is used for making new empty files
  - `rm` is used for removing a file or directory

You will be using these commands throughout the curriculum and can reference them here as you go.

### Git

- git is a way to save your local files in the cloud
- it allows you to look at the history changes to those files and share with others
- there are commands you can use in Terminal to add files that you change to git

### Sublime Text 3

- This is basically a glorified text editor that makes writing code faster
- It has plugins you can install that help with development
  - Color-coding of syntax that makes reading and writing code easier
  - It shows warnings and errors for syntax and some coding logic

Throughout the curriculum you will be using Terminal and Sublime Text 3 to write your code.

## 3) Front-end/back-end, client/server, what are those?!

- Client is what homo sapiens interact with when they use websites and apps
  - The client is typically either a web browser, iOS app, Android app, Windows app, or Mac app.
- Server is what the client app talks to in order to send data and retrieve data
  - Server is just a computer somewhere that the client talks to
  - Server often uses a database to store things long-term

## 4) Client

- There are many ways to code the client, but the current way its often done is primarily in JavaScript because thats what the web browser uses
- The role of the client is to display things to the user and take user input
  - In the web browser, HTML and CSS are used for layout and display
  - On iOS/Android/Windows/Mac, there are has similar layout and styling concepts to HTML and CSS
  - JavaScript is used for user input

For the purpose of this curriculum and given its popularity, we will be focusing only on writing code in JavaScript.

Now we'll jump right into creating some fun websites.

View `https://www.github.com/antonellil/engineeringcurriculum/client.md` to get started.

## 5) Server

- There are many ways to code the server, for the purposes of this tutorial we'll be using JavaScript so that the language is the same on the front-end and backend. NodeJS is a server-side language that uses JavaScript.
- The role of the server is to act as a web server that talks to clients, or to perform processing and tasks and not talk to clients

Now we'll jump right into creating some fun servers.

View `https://www.github.com/antonellil/engineeringcurriculum/server.md` to get started.

## 6) Database

- PostgreSQL overview and tutorials
- Role of the database (storage, retrieval)
- Building practical database tables and usage

## 7) Caching

- Redis overview and tutorials
- Role of caching (often-accessed values, limiting database reads)
- Building practical things with caching

## 8) End-to-end

- Build several applications end-to-end through all layers of the stack
