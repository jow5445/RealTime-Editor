# Real-Time Editor

![Editor](https://cdn.hackclub.com/01a0d94b-3cde-7a08-9ea5-0a8d48b81fd2/Screenshot%20From%202026-09-25%2018-59-28.png)
A small browser-based editor where you can write HTML, CSS, and JavaScript and see the result immediately.

I built this as a simple way to experiment with front-end code without opening a full editor or setting up a project.

## What it does

* Edit HTML, CSS, and JavaScript separately
* See changes immediately in the preview
* Use `Tab` inside the editor
* Download each part as a separate file
* Resize the editor and preview by dragging the middle divider

## How it works

The page has two main parts:

* **Editor** - contains three text areas for HTML, CSS, and JavaScript
* **Preview** - an iframe that displays the result

Whenever you type something, the `update()` function takes the three editors and puts them together before writing the result into the iframe.

The download buttons create a file from the content of each editor using a browser `Blob`.

## Files
The project can be kept as a single HTML file:

```text
index.html
```

The page loads [Split.js](https://github.com/nathancahill/split/tree/master/packages/splitjs) from a CDN to make the editor and preview resizable.

## Downloading code

Each editor has a small download button.

The files are saved as:

```text
index.html
style.css
script.js
```

The download happens directly in the browser, so nothing is uploaded to a server.

## Technologies

* HTML
* CSS
* JavaScript
* Split.js
