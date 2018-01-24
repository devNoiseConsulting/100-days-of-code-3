# 100 Days Of Code - Log

### Round 3, Day 1: Jan 2, 2018

**Today's Progress:** Declaring Round 2 complete and documenting it.

**Thoughts:** Was bad hit a road block and stopped working on my freeCodeCamp projects. Though I did continue doing daily programming challenges that were posted on the PhillyDev Slack. Just didn't really log them until now. Filed them under a Day XX which I use to show work, but don't count. In any case I wrote a JavaScript snippet to scape the links and descriptions from my gists. This also helped when I added my code to complete the Advent of Code challenges. Each of these challenges were counted as a day since I usually spent a couple hours completing them.

**Link to work:**

-   [gistScraper.js Gist](https://gist.github.com/devNoiseConsulting/a33f53423011e296ab804303682b6677/04cd3935a8b14d9be226690ce7d627b77b7d033e)
-   [100 Days of Code, Part Duex - Commit 1](https://github.com/devNoiseConsulting/100-days-of-code-2/commit/02155bf9092e0166ff29706bf01d84484e37bd34)
-   [100 Days of Code, Part Duex - Commit 2](https://github.com/devNoiseConsulting/100-days-of-code-2/commit/b8d5f277f01b520c07d5ed08d2a26544b3f19154)

### Round 3, Day 2: Jan 3, 2018

**Today's Progress:** Setting up my repo for round 3 and fixing my gist scrapper.

**Thoughts:** Instead of forking the freeCodeCamp #100DaysOfCode repo, I created a new one. This is an easy way for my log.md commits to count towards my contributions.

Missed that some of the links to my Advent of Code Gist were not linked to the correct Gist. Went back and worked on the gist scrapper. Realized I need to filter the descriptions so that the correct description can be combined with the gist url. Then I refactored the code by using more ES6 features.

**Link to work:**

-   [gistScraper.js Gist](https://gist.github.com/devNoiseConsulting/a33f53423011e296ab804303682b6677)
-   [100 Days of Code, Part Duex - Commit](https://github.com/devNoiseConsulting/100-days-of-code-2/commit/4bebcbef52db5b86bb8e049fa48bfac75adb2146)
-   [100 Days of Code, Partie Trois](https://github.com/devNoiseConsulting/100-days-of-code-3)


### Round 3, Day 3: Jan 4, 2018

**Today's Progress:** Login working on Voting App.

**Thoughts:** Need to remember and embrace the arrow function in a fetch's promise chain. Was losing reference to the the correct 'this' and couldn't update the component's state. Spent the rest of my time trying to figure out how react-router-dom' Redirect component is using the to object I gave it. Could not grok were the to.state was being handed off to the component that mapped to the to.pathname. Finally figure out that it ends up at props.location.state. Still doesn't help me with persisting this data. Can't tell if I need to break down and start using Redux in this app yet.

**Link to work:**
-   [fCC's Voting App Commit](https://github.com/devNoiseConsulting/fcc-voting-app/commit/667a1a7c96a5fe302a8cf2f814dbbd4c635e5d11)

### Round 3, Day 4: Jan 5, 2018

**Today's Progress:** Started Udacity's Front-End Web Developer preview.

**Thoughts:** Took a look at this since I've applied for [Grow with Google US Scholarship](https://www.udacity.com/grow-with-google). Not sure I'm the intended audience as I've written enough HTML that this is mostly a review.

**Link to work:**
-   [Udacity's New Year, New Skills](https://www.udacity.com/new-year)

### Round 3, Day 5: Jan 6, 2018

**Today's Progress:** Finished Udacity's Front-End Web Developer preview and refactoring on the voting app.

**Thoughts:** Completed the Front-End Web Developer preview. The sections today mostly focused on know how to use a text editor. Was a little bit useful, but mostly review.

Did a little bit of work on the Voting App. Moved most of the routing into the App component and move most of the old App component into a new component named Home. The moved the header back to the App component. Just a bit of busy work while I contemplate how state should move between routed components. Do I bite the bullet and drive into Redux for app state management?

**Link to work:**
-   [Udacity's New Year, New Skills](https://www.udacity.com/new-year)
-   [fCC's Voting App Commit](https://github.com/devNoiseConsulting/fcc-voting-app/commit/771d04dbc8af0f3a39e3b4087bbbbc9d9a582da6)

### Round 3, Day 6: Jan 7, 2018

**Today's Progress:** Worked on a map to visualize the Pokemon Go raid zones in my area.

**Thoughts:** Avoiding the Redux question for now by making a map. Used [Parcel](https://parceljs.org/) to handle building the project. Seems pretty good, but having issues with getting the browser to refresh. This may have to do with the fact that Parcel was invoked with index.html as an argument. Will have to look into this some more.

Hard coded a lot of circles. Should come back and have the code iterate over an array of objects with the needed data.

**Link to work:**
-   [Pokemon Go Raid Zones Commit](https://github.com/devNoiseConsulting/fcc-voting-app/commit/771d04dbc8af0f3a39e3b4087bbbbc9d9a582da6)


### Round 3, Day 7: Jan 8, 2018

**Today's Progress:** Refactoring the Pokemon Go raid zones map.

**Thoughts:** Move the Mapbox Access Token in a "config" file. Then started to move all the raid zone data into array of zone objects. Created a function that could take the raid zones and draw the circles on the map. Later moved the raid zones into the config object.

Color stuff will always suck up my time. Used the [Material Design color palette](https://material.io/guidelines/style/color.html#color-color-palette) to give each raid zone a unique color. Played around until I had a color set I liked.

**Link to work:**
-   [Pokemon Go Raid Zones Commit](https://github.com/devNoiseConsulting/PokemonGoRaidZones/commit/012d21eec9a1b4424319ee3f186bb0655f3a7b8d)


### Round 3, Day 8: Jan 9, 2018

**Today's Progress:** More work on the Pokemon Go raid zones map.

**Thoughts:** Still trying to improve my understanding of [Parcel](https://parceljs.org/). I've yet to figure out how to get it to do hot reloading, still have to refresh the browser. For the production build, have to use `--public-url ./` so the html points at all the right files.

Added the Bootstrap framework to give the page a polished look. Changed the units on the map from pixels to viewport height. Also added a function to reset the map back to default state. Moved starting data into the config object.

**Link to work:**
-   [Pokemon Go Raid Zones Commit](https://github.com/devNoiseConsulting/PokemonGoRaidZones/commit/76c9a272bd5f78a0feaa79ebbb57bfae0b1d9daf)

### Round 3, Day 9: Jan 10, 2018

**Today's Progress:** More tweaks to the Pokemon Go raid zones map and Udacity's Grow with Google Challenge Scholarship.

**Thoughts:** Received some suggestions for tweaking the data. This lead to working on having multiple config files. Using symbolic links to change out the config files. Also needed to change the .gitignore to not include the real config files.

Also found out that I got accepted into the Grow with Google Challenge Scholarship. Got started by joining the forum and slack.

**Link to work:**
-   [Pokemon Go Raid Zones Commit](https://github.com/devNoiseConsulting/PokemonGoRaidZones/commit/ee6771ea365bc8fec2c25dd2036da12ea36e49f7)

### Round 3, Day 10: Jan 11, 2018

**Today's Progress:** More work Udacity's course work.

**Thoughts:** Did some review work on the the Service Worker course that I worked on last year. Not having issues with the concepts, but getting the browser in to the state that will pass. Ran into some problems with [CacheStorage](https://developer.mozilla.org/en-US/docs/Web/API/CacheStorage). Seems like a slight difference in browser implementation between Chrome and Firefox. In Chrome, a promise if always return when you call cache.match(). The promise will resolve to undefined in Chrome, which broke the MDN example code. Oddly, the example for [cache.match()](https://developer.mozilla.org/en-US/docs/Web/API/CacheStorage/match) fit in with Chrome's behavior. Replacing the cache when the service worker activates cause major headaches. Got the code running, but major issues with getting the browser state to be exactly what the quiz code wants. Will tackle it again tomorrow.

**Link to work:**
-   [Wittr repo](https://github.com/jakearchibald/wittr) - Don't really have any work to show as I keep blowing away my code for the next task.

### Round 3, Day 11: Jan 12, 2018

**Today's Progress:** Finished the Introducing the Service Worker course.

**Thoughts:** Did some more sections that I had previously completed to refresh my memory on service workers. Screwed up the code for 3.21 which caused all of the caches for the service worker to be deleted. Took me a while to figure out what the bug was. After that I proceeded to pay closer attention to the code being discussed in the video. This definitely help to know what function/methods to call to complete the quiz.

**Link to work:**
-   [Wittr repo](https://github.com/jakearchibald/wittr) - Don't really have any work to show as I keep blowing away my code for the next task.
-   [Service Worker activate error Gist](https://gist.github.com/devNoiseConsulting/f856c42f3da77364a7b080cbf0c22660)

### Round 3, Day 12: Jan 13, 2018

**Today's Progress:** Started IndexedDB and Caching course.

**Thoughts:**
IndexDB API has functions/methods with value:key instead of the usual key:value parameters.
Couldn't see the IndexDB that I created in the Application tab of the dev tools. Page refresh didn't do anything. Had to "Refresh IndexDB" manually to see my data.

**Link to work:**
-   [Wittr repo](https://github.com/jakearchibald/wittr) - Don't really have any work to show as I keep blowing away my code for the next task.

### Round 3, Day X: Jan 14, 2018

**Today's Progress:** Working on IndexedDB and Caching course.

**Thoughts:** I don't think I really got my hour in, so I'm not counting it. Can't seem to get past part 7 in the IndexedDB and Caching course. Understand what needs to be done, but doesn't seem to work.

**Link to work:**
-   [Wittr repo](https://github.com/jakearchibald/wittr) - Don't really have any work to show as I keep blowing away my code for the next task.

### Round 3, Day 13: Jan 15, 2018

**Today's Progress:** Working IndexedDB and Caching course.

**Thoughts:** Finally got past part 7 in the IndexedDB and Caching course. Quite possibly, I had working code, but didn't bump the service worker to create a new cache.

**Link to work:**
-   [Wittr repo](https://github.com/jakearchibald/wittr) - Don't really have any work to show as I keep blowing away my code for the next task.

### Round 3, Day 14: Jan 16, 2018

**Today's Progress:** Finished IndexedDB and Caching course.

**Thoughts:**

**Link to work:**
-   [Wittr repo](https://github.com/jakearchibald/wittr) - Don't really have any work to show as I keep blowing away my code for the next task.

### Round 3, Day 15: Jan 17, 2018

**Today's Progress:** Finished Lesson 6: Syntax  and started Lesson 7: Functions for #GoogleUdacityScholars

**Thoughts:** This is mostly a review for me as I mastered most this completing the Front End Development Certification at freeCodeCamp. Getting people up to speed on the new syntax of ES6/ES2015. I'm clearly convinced that lessons 6-9 should have been before lesson 2. While I think that progressive web apps are important to learn, they really threw all the candidates into the deep end by making that first.

**Link to work:**
-   [Grow with Google Challenge Scholarship: Mobile Web](https://classroom.udacity.com/courses/ud899-gwg)

### Round 3, Day 16: Jan 18, 2018

**Today's Progress:** Finished Lesson 7: Functions for #GoogleUdacityScholars

**Thoughts:** Arrow functions, default parameters and classes. Again mostly a review for me as I mastered most this completing the Front End Development Certification at freeCodeCamp. Will admit that I didn't get all the answers right. Mostly due to me not reading the code closely enough to catch the errors.

**Link to work:**
-   [Grow with Google Challenge Scholarship: Mobile Web](https://classroom.udacity.com/courses/ud899-gwg)

### Round 3, Day 17: Jan 19, 2018

**Today's Progress:** Started Lesson 8: Built-ins for #GoogleUdacityScholars and some scripts for Pokemon Go Points of Interest.

**Thoughts:** Spent some time working on my Udacity course looking at the JavaScript Symbols builtin. I generally understand it, but not sure where I would use it. Decided to shift gears and work on getting some data for Pokemon Go points of interest. Grabbed a punch of portal data from Ingress. Wrote a script to filter the points into the raid zones used for the Montco/ChesCo discord server. Also worked on a script that would help identify hot spots or area with a high density of points.

**Link to work:**
-   [Grow with Google Challenge Scholarship: Mobile Web](https://classroom.udacity.com/courses/ud899-gwg)
-   [PokemonGoGIS](https://github.com/devNoiseConsulting/PokemonGoGIS)

### Round 3, Day 18: Jan 20, 2018

**Today's Progress:** Finished Lesson 8: Built-ins for #GoogleUdacityScholars.

**Thoughts:** 

**Link to work:**
-   [Grow with Google Challenge Scholarship: Mobile Web](https://classroom.udacity.com/courses/ud899-gwg)

### Round 3, Day 19: Jan 21, 2018

**Today's Progress:** Finished Lesson 9: Professional Developer-fu for #GoogleUdacityScholars.

**Thoughts:**

**Link to work:**
-   [Grow with Google Challenge Scholarship: Mobile Web](https://classroom.udacity.com/courses/ud899-gwg)

### Round 3, Day 20: Jan 22, 2018

**Today's Progress:** More work on my Pokemon Go Raid zones

**Thoughts:** Added gym markers, but some reason LeafletJS and ParceljJS aren't playing nice. To get markers working, I couldn't use the default marker because the URL for the marker image breaks. Created an Icon object that pointed to image file in the dist folder. Also needed to edit the Javascript file in the dist folder for the production build.

**Link to work:**
-   [PokemonGoRaidZones Commits](https://github.com/devNoiseConsulting/PokemonGoRaidZones/commit/d74042bd45a07e25e28956ce43c91726c18a835a)
-   [PokemonGoGIS Commits](https://github.com/devNoiseConsulting/PokemonGoGIS/commit/94f6ea6dd5afbe263ce7d65627803f97eb50f88e)

### Round 3, Day 21: Jan 23, 2018

**Today's Progress:** Started Udacity's JavaScript Promises Course.

**Thoughts:** Completed Lesson 1: Creating Promises.

**Link to work:**
-   [JavaScript Promises Course](https://classroom.udacity.com/courses/ud898)

<!--

### Rouond 3, Day 0: Jan 1, 2018 (Example 1)
##### (delete me or comment me out)

**Today's Progress** Fixed CSS, worked on canvas functionality for the app.

**Thoughts:** I really struggled with CSS, but, overall, I feel like I am slowly getting better at it. Canvas is still new for me, but I managed to figure out some basic functionality.

**Link to work:** [Calculator App](http://www.example.com)

-->
