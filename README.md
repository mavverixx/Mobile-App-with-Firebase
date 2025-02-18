# Leads Tracker

This is a simple yet functional Leads Tracker application that demonstrates the use of HTML, CSS, and JavaScript, integrated with Firebase Realtime Database. It allows users to save, display, and delete URLs dynamically, showcasing clean code practices with a focus on user interaction, DOM manipulation, and database integration.

![Screen Recording 2025-02-12 at 18-40-56_4](https://github.com/user-attachments/assets/86dea394-55b8-44cb-b359-491f2a5ee8a1)


## Table of Contents

- [Overview](#overview)
  - [The Challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My Process](#my-process)
  - [Built With](#built-with)
  - [What I Learned](#what-i-learned)
  - [Continued Development](#continued-development)
  - [Useful Resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The Challenge

Build a Leads Tracker application that:
- Saves user-entered URLs to a Firebase Realtime Database.
- Dynamically displays the saved URLs as clickable links in the DOM.
- Allows users to delete all saved URLs with a double-click action.

### Links

- **Source Code:** [GitHub Repository](https://github.com/mavverixx/Mobile-App-with-Firebase)
- **Live Site:** [Live Demo URL](https://mobile-app-with-firebase-wv6s.vercel.app/) *(update with your current live URL if available)*

## My Process

### Built With

The project is built using:
- **HTML5:** Provides the basic structure of the webpage.
- **CSS3:** Handles the visual presentation, layout, and styling.
- **JavaScript (ES6+):** Powers the interactive features and Firebase integration.
- **Firebase Realtime Database:** Stores and retrieves user data dynamically.

### What I Learned

Through this project, I gained insights into:
- Integrating Firebase Realtime Database with a web application.
- Dynamically updating DOM elements to reflect database changes.
- Handling user events like button clicks and double-clicks effectively.
- Writing modular and maintainable JavaScript code.

Example JavaScript snippet:
```js
onValue(referenceInDB, function(snapshot) {
    const snapshotDoesExist = snapshot.exists();
    if (snapshotDoesExist) {
        const snapshotValues = snapshot.val();
        const leads = Object.values(snapshotValues);
        render(leads);
    }
});
```
Continued Development

In the future, I plan to:

Add user authentication to secure the database.
Implement a feature to edit individual URLs.
Enhance the UI for a more modern and responsive design.
Useful Resources

Some of the resources that helped during development include:

Firebase Documentation for understanding Realtime Database integration.
MDN Web Docs for JavaScript and DOM manipulation references.
CSS-Tricks for practical tips on styling and layout.

Author
[LinkedIn](https://mobile-app-with-firebase-wv6s.vercel.app/)

Acknowledgments

Thank you to everyone who contributed ideas, feedback, and support during the development of this project.
