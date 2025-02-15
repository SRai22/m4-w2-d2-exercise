# m4-w2-d2-exercise: Cookie and Session Storage Demo

Web-602-Spring-2025

## Overview
This project contains two HTML pages demonstrating the use of **cookies** and **session storage** in JavaScript. These features help in storing user data either persistently (cookies) or temporarily during a session (session storage).

## Files Included
1. **cookie-demo.html** - Demonstrates how to set, retrieve, and check cookies in a browser.
2. **session-demo.html** - Demonstrates how to use session storage to track button clicks within a browser session.

## Features
### **cookie-demo.html**
- Stores a username in a **cookie** that persists for 30 days.
- Checks if the cookie exists when the page loads.
- If a user visits again, it retrieves the username from the cookie and displays a welcome message.
- If no cookie exists, prompts the user to enter a name and stores it in a cookie.

### **session-demo.html**
- Uses **sessionStorage** to count the number of times a button is clicked.
- The counter resets when the browser tab is closed.
- Displays a message with the number of times the button has been clicked during the session.

## How to Run
1. Open `cookie-demo.html` in a browser.
   - If it's your first visit, you'll be prompted to enter your name.
   - Reload the page to see the stored username in a welcome message.
   - Close and reopen the browser to see if the cookie persists.

2. Open `session-demo.html` in a browser.
   - Click the button and see the count increase.
   - Close the tab and reopen it to observe that the counter resets.

## Code Explanation
### **cookie-demo.html**
- `setCookie(cname, cvalue, exdays)`: Stores a cookie with a name, value, and expiration date.
- `getCookie(cname)`: Retrieves a cookie value by name.
- `checkCookie()`: Checks if the username cookie exists and either welcomes the user or prompts for a new username.

### **session-demo.html**
- `clickSessionCounter()`: Checks if `sessionStorage.clickcount` exists and increases the count.
- `sessionStorage`: Stores the counter value temporarily, resetting when the tab is closed.

## Browser Compatibility
- **Cookies** work across sessions but require user permission in some browsers.
- **Session Storage** works only within the current session and resets when the tab is closed.

