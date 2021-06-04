# Testing 

> * This is the updated testing document to include the new components in the website

During the development process, testing has been conducted as an ongoing process, with further testing conducted towards the end of the process:
* [Testing process](https://github.com/lmw95/stayverticalpolestudio/blob/master/documentation/TESTING.md/#testing-process)
* [Issues during development](https://github.com/lmw95/stayverticalpolestudio/blob/master/documentation/TESTING.md/#issues--during-development)
* [Accessibility](https://github.com/lmw95/stayverticalpolestudio/blob/master/documentation/TESTING.md/#accessibility)
* [Performance](https://github.com/lmw95/stayverticalpolestudio/blob/master/documentation/TESTING.md/#performance)
* [HTML & CSS validation](https://github.com/lmw95/stayverticalpolestudio/blob/master/documentation/TESTING.md/#html--css-validation)

## Testing process 
This section outlines the testing of the interactive components of the website.
### Navigation menu
* Plan: I wanted a navigation menu that was fixed to the top of the user's screen. All the links should take the user to their intended destination, be it on the current page, a different part of the website or another site entirely.
* Implementation: I created the navigation menu using CSS Flexbox and a block of JavaScript code which I found on [Web/Design/Vista](https://www.webdesignvista.com/create-responsive-navbar-without-bootstrap/) which provided me with a responsive navigation menu that stretches the entire width of the user's screen, and the navigation items display neatly in a hamburger menu when viewed on a mobile screen. I styled the navigation in accordance with the colour palette of the website.
* Test: I tested the website on Google Chrome, Mozilla Firefox and Microsoft Edge. On Google Chrome, I used Responsive View to grow and shrink the device width to make sure the navigation menu changes display at the breakpoints.
* Result: The navigation bar displays correctly on all browsers and devices.
* Verdict: PASS

### Zooming header animation
* Plan: I wanted to have a hero image which moved towards the user to grab their attention when they first enter or refresh the page. 
* Implementation: I created a header background div within the header itself and set the background to the hero image, then used keyframes to create the zooming animation of the hero image div.
* Test: I tested the website on Google Chrome, Mozilla Firefox and Microsoft Edge and refreshed the page a few times on each. Using Google inspect and Responsive View, I refreshed the page a few times to test the zoom on smaller screens.
* Result: The background zoom works well on all browsers and screen sizes as intended - there was a slight delay on Google Chrome desktop view at first but worked well afterwards.
* Verdict: PASS

### Working links
* Plan: I wanted to have working links that took the user to external sites (such as social media), to another section of the page or opened another app (such as Outlook).
* Implementation: I left the link hrefs empty at first, then I created a 404 error page, and linked all the relevant pages and sections to each link with their correct targets.
* Test: I tested the website on Google Chrome, Mozilla Firefox and Microsoft Edge by clicking on all of the links one by one to check they took the user to the correct place.
* Result: I noticed an incorrect link in some of the buttons, but that was easily added in after testing and fixed the issue. All other links were working perfectly on all browsers.
* Verdict: PASS

### Hover effects
* Plan: I wanted animations on the buttons, social media links, navigation menu links and the instructors' profiles to increase interactivity with the user as they travelled through the website.
* Implementation: I utilised Hover.css: the 'float' effect for buttons and social media icons, and the 'grow' effect for the navigation menu links.
* Test: I tested the website on Google Chrome, Mozilla Firefox and Microsoft Edge, I hovered over all of the hoverable elements to make sure the effect was working.
* Result: All hoverable effects worked across all browsers and devices.
* Verdict: PASS

### Contact form
* Plan: I wanted to include a contact form which the user can fill in if they wish to reach out to the owners directly. They should insert their name, email address & phone number, a reason for contact and a message so the owners can respond to them. 
* Implementation: In order to implement this, I have created a form in my index.html with 3 input fields, 1 textarea field and a submit button, with corresponding labels. The form was styled in accordance with the colour palette of the site.
* Test: I tested the website on Google Chrome, Mozilla Firefox and Microsoft Edge, I tried to submit the form without entering the required information in the input fields to test the form validation.
* Result: An alert popped up telling the user to enter text in the field on all browsers and devices, which worked as expected.
* Verdict: PASS

### Flickity carousels
* Plan: I wanted to use [Flickity](https://flickity.metafizzy.co/) to create interactive carousels for the Classes and Reviews section so that it saves space on the webpage but also improves the user experience.
* Implementation: I utilised Flickity's CDN and code to create two carousels and edited them to how best suited the webpage in terms of colour, content and size.
* Test: I tested the carousels on all device sizes and browsers to ensure sizing was correct and that the scrolling effect was working.
* Result: The carousels worked correctly as planned on all devices and browsers.
* Verdict: PASS

---

## Issues during development
This section covers the major issues I encountered during the development and testing process and the solutions that fixed them.
### Navigation
* Issue: The navigation links were bunched up too close to each other
* Solution: I removed the styling for .nav-item divs and started over by styling the nav-item links only
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/7dedc1fbb8fe96b8214def040d666fd08f0912af)

* Issue: The slogan in the header would overlap the navbar
* Solution: I changed the z-index of the navbar to 2 which fixed the issue
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/672c6d2b4a117dfd0c8c119c9a88b375fdcd0aa0)

### Header (zooming background)
* Issue: The zooming background div would overlap the navbar 
* Solution: I gave the navbar a z-index of 1 to place it over the zooming background div
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/005bf050dcad046f6b1f55471bb4c36e3aac7229)

* Issue: The zooming background div was pushing down the About section
* Solution: I changed the positioning of the About section to relative 
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/9b25830d86586e6b856d5987dcfa06ff8de97854)

* Issue: The overlapping of the zooming background div issue persisted 
* Solution: I changed the overflow of both header divs to hidden with the help of [Stack Overflow](https://stackoverflow.com/questions/32524423/zooming-an-image-on-hover-and-not-exceeding-parent-div-borders)
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/a747e7f1c89289a957a099b8e338e01e67d85cc4)

### Responsive design
* Issue: The About section would not respond responsively when changing the screen width in Google Dev Tools Responsive Viewer
* Solution: I set the width of the whole About section to 100% which fixed the issue
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/852ba6ed9e5132ae91a5ab81d0d71dfbd0d37ce9)

* Issue: There was white space showing on the side of the website when in mobile & tablet screen size in Responsive Viewer
* Solution: I changed the html overflow-x value to hidden for both mobile and tablet media queries, with the help of [Stack Overflow](https://stackoverflow.com/questions/47976439/unable-to-remove-white-space-from-right-in-responsive-design-html-css)
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/852ba6ed9e5132ae91a5ab81d0d71dfbd0d37ce9)

* Issue: The sections were too large in height, providing extra empty space at the bottom of each section
* Solution: Removed height attributes entirely
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/3e0ac9a3e3b80063c02c6480dba7e3b466e38775)
> * [Linkl to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/335d7a02df7c476dc44344082393a8cbc6654831)

## Issues post-deployment
* Issue: Post-deployment website did not display background images due to incorrect file paths
* Solution: I simply switched the absolute paths to relative paths on all divs that had a background image with a URL
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/059f58c0a66b03af1ad77610412163cb9e5ff7f4)

* Issue: Post-deployment navigation menu links did not lead user to the correct page/section
* Solution: Fixed links to take user to correct places
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/1807913e171111fd8e0c1a9956df7005e7ccf353)

* Issue: The company logo (made with Favicon) was not appearing in the header post-deployment
* Solution: I changed the img to a div and set the background as the Favicon which fixed the issue
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/e999c887c9a0db2c4a98d3ae9004dc6ae6b9c8eb)

[Back to top](https://github.com/lmw95/stayverticalpolestudio/blob/master/documentation/TESTING.md/#testing)

## Google Lighthouse
### DESKTOP
Post-update, Google Lighthouse returned green across all reports (accessibility, performance, SEO and best practices)

![](documentation/screenshots-post-update/lighthouse-post-update.png)

