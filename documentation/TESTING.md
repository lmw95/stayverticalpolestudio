# Testing 

During the development process, testing has been conducted as an ongoing process, with further testing conducted towards the end of the process:
* [Issues during development](https://github.com/lmw95/stayverticalpolestudio/blob/master/documentation/TESTING.md/#issues-during-development)
* [User stories](https://github.com/lmw95/stayverticalpolestudio/blob/master/documentation/TESTING.md/#user-stories)
* [Accessibility](https://github.com/lmw95/stayverticalpolestudio/blob/master/documentation/TESTING.md/#accessibility)
* [Performance](https://github.com/lmw95/stayverticalpolestudio/blob/master/documentation/TESTING.md/#performance)
* [HTML & CSS validation](https://github.com/lmw95/stayverticalpolestudio/blob/master/documentation/TESTING.md/#html--css-validation)

# Issues during development
* Issue: The navigation links were bunched up too close to each other
* Solution: I removed the styling for .nav-item divs and started over by styling the nav-item links only
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/7dedc1fbb8fe96b8214def040d666fd08f0912af)

* Issue: The zooming background div would overlap the navbar 
* Solution: I gave the navbar a z-index of 1 to place it over the zooming background div
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/005bf050dcad046f6b1f55471bb4c36e3aac7229)

* Issue: The slogan in the header would overlap the navbar
* Solution: I changed the z-index of the navbar to 2 which fixed the issue
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/672c6d2b4a117dfd0c8c119c9a88b375fdcd0aa0)

* Issue: The zooming background div was pushing down the About section
* Solution: I changed the positioning of the About section to relative 
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/9b25830d86586e6b856d5987dcfa06ff8de97854)

* Issue: The About section would not respond responsively when changing the screen width in Google Dev Tools Responsive Viewer
* Solution: I set the width of the whole About section to 100% which fixed the issue
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/852ba6ed9e5132ae91a5ab81d0d71dfbd0d37ce9)

* Issue: The overlapping of the zooming background div issue persisted 
* Solution: I changed the overflow of both header divs to hidden with the help of [Stack Overflow](https://stackoverflow.com/questions/32524423/zooming-an-image-on-hover-and-not-exceeding-parent-div-borders)
> * [Link to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/a747e7f1c89289a957a099b8e338e01e67d85cc4)

* Issue: There was white space showing on the side of the website when in mobile & tablet screen size in Responsive Viewer
* Solution: I changed the html overflow-x value to hidden for both mobile and tablet media queries, with the help of [Stack Overflow](https://stackoverflow.com/questions/47976439/unable-to-remove-white-space-from-right-in-responsive-design-html-css)
> * [Linl to commit & code](https://github.com/lmw95/stayverticalpolestudio/commit/852ba6ed9e5132ae91a5ab81d0d71dfbd0d37ce9)

# User stories

[Back to top](https://github.com/lmw95/stayverticalpolestudio/blob/master/documentation/TESTING.md/#testing)

# Accessibility

[Back to top](https://github.com/lmw95/stayverticalpolestudio/blob/master/documentation/TESTING.md/#testing)

# Performance

[Back to top](https://github.com/lmw95/stayverticalpolestudio/blob/master/documentation/TESTING.md/#testing)

# HTML & CSS validation

[Back to top](https://github.com/lmw95/stayverticalpolestudio/blob/master/documentation/TESTING.md/#testing)

