# Welcome to the client part of the curriculum!

You will be making a selfies website that lets you take selfies, add them to photo albums, give the selfies captions, and remove them.

Get pumped!!!!!!!!!!!!!!!!!!!!!!!

## Anatomy of a website (or web app)

A website typically consists of three parts:

1. The HTML which describes how to lay the website out
2. The CSS which describes how to make the website look
3. The JavaScript which describes how to make the website come alive.

## Selfies

To start:

1. Open Terminal
2. Create a folder called `selfies` by using `mkdir selfies`
3. Navigte to the folder using `cd selfies`
4. Create a file `index.html` by using `touch index.html`
5. Create a file `index.css`
6. Create a file `index.js`
7. Open the `selfies` folder in Sublime Text

Every website has a standard format for HTML that all browsers can read. Read and copy the example template from here https://www.w3schools.com/html/html_basic.asp and paste it in your `index.html` file.

There are many HTML elements, but practically only the `div` element is needed and used as the main building block for websites. Delete the contents of the `body` tag in your `index.html` and add a new empty `div` element in your `body` like `<div>Selfies</div>`.

Open your `index.html` file in Google Chrome by going to `Chrome -> File -> Open File`.

Next, lets change the color of that `div`. Create a class (which is what CSS uses to describe how to make elements look) in `index.css` by typing:
```
.header {
  color: purple;
}
```

In your `index.html`, add that class to your selfies `div` by doing `<div class="header">Selfies</div>`.

If you refresh your Google Chrome you'll see that the color hasn't changed yet. That is because we haven't told the `index.html` file that it needs to use the `index.css` file. To do that, add a link to that file in the `head` tag of your `index.html` by following https://www.w3schools.com/tags/tag_link.asp. The `head` tag goes right above the `body` tag.
