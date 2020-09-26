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

If you refresh your Google Chrome you'll see that the color hasn't changed yet. That is because we haven't told the `index.html` file that it needs to use the `index.css` file. To do that, add a link to that file in the `head` tag of your `index.html` by following https://www.w3schools.com/tags/tag_link.asp. The `head` tag goes right above the `body` tag and closes itself before the `body` starts.

Next, lets add our first interaction to the page using JavaScript. We need to link our `index.js` to our `index.html`. To do that, add a tag `<script src="index.js"></script>` right before you close the `</body`. This tells the `index.html` page to load your `index.js` javascript file.

Let's add a `button` element after your Selfies `div` like `<button>Take a selfie</button>`. Then let's make your JavaScript do something when the button is pressed. In your `index.js` file, you can tell it to find the `button` you just added in the html. First add an `id` attribute to your button and like `<button id="butts">Take a selfie</button>`. The `id` attribute is an attribute that is used to uniquely identify elements on the page.

In your `index.js` file you can create a variable that stores the button that we can use. Try adding the below to your `index.js` file:
```
const selfieButton = document.getElementById('butts');
```
This will create a `selfieButton` variable from the element with your `id='butts'`.

Now we can tell the `selfieButton` to do something when it is clicked. This is done by adding what JavaScript calls "listeners" which are functions that get called when certain "events" happen to elements in the html. There is an event called `click` that we can use to tell the button to do something when a click happens to it. You can add a listener to the button with
```
const selfieButton = document.getElementById('butts');

selfieButton.addEventListener('click', () => {
  alert('I was smashed');
});
```

This listener will call the function and pop up an alert when it is clicked. If you refresh your page in Google Chrome and press the button, you should see an alert message pop up. You can close the alert and click the button and see it again.

Now, lets access the camera from the browser. Add a `video` element to your html that we will use to display your camera. You can add it to `index.html` like `<video id="video">Video stream not available yet.</video>`

In order to access the camera, we will have to ask the browser if we can use it and the user will have to confirm that. Add a new function to the top of your `index.js` that we will use to request access. The function will be an `async` function (which means that it needs to wait for the user to provide its "okay" to use the camera before proceeding) and `await` for the user input to say "okay you can use the camera":
```
async function openCamera() {
  const stream = await navigator.mediaDevices.getUserMedia({ video: true, audio: false });

  const video = document.getElementById('video');

  video.srcObject = stream;
  video.play();
}
```

What this function is doing is asking the browser to access the user media (the camera, and also potentially the microphone) and then displaying that camera in the `video` element that we added before. We should also make the video a certain size by adding some styling to `index.css` for it:
```
#video {
  width: 400px;
  height: 400px;
}
```

Now we need to tell the button to call the `openCamera` function when its clicked. To do that, change your listener to remove the `alert` line and change it to `openCamera()` which will call the `openCamera` function that we added. The `()` parentheses after the function tell the JavaScript that we want to run the function, and pass in no arguments to it since the function doesn't take any arguments.