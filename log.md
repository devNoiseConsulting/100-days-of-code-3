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
-   [PokemonGoRaidZones Commit](https://github.com/devNoiseConsulting/PokemonGoRaidZones/commit/d74042bd45a07e25e28956ce43c91726c18a835a)
-   [PokemonGoGIS Commit](https://github.com/devNoiseConsulting/PokemonGoGIS/commit/94f6ea6dd5afbe263ce7d65627803f97eb50f88e)

### Round 3, Day 21: Jan 23, 2018

**Today's Progress:** Started Udacity's JavaScript Promises Course.

**Thoughts:** Completed Lesson 1: Creating Promises.

**Link to work:**
-   [JavaScript Promises Course](https://classroom.udacity.com/courses/ud898)

### Round 3, Day 22: Jan 24, 2018

**Today's Progress:** Completed Udacity's JavaScript Promises Course and tweaking my Pokemon Go Raid zones map.

**Thoughts:** Completed Lesson 2: Chaining Promises. Realized my Pokemon Go Raid zones was not really mobile friendly so added viewport info to the HTML. Also found Bootstrap.native so I wouldn't have to include jQuery to make the Bootstrap components work.

**Link to work:**
-   [JavaScript Promises Course](https://classroom.udacity.com/courses/ud898)
-   [PokemonGoRaidZones Commit](https://github.com/devNoiseConsulting/PokemonGoRaidZones/commit/09154de8029a5a51074ff3dc72f5f696e6c4b7a6)

### Round 3, Day 23: Jan 26, 2018

**Today's Progress:** More coding on my Pokemon Go Raid zones map.

**Thoughts:** Writing code to write code. So maybe not the best plan, but I put all the gym data points into the code. On the plus side it is in a separate code file that I can import. Thus I just need to update the file for changes and no round trips to the server to get data. Initially, I used some regex in Atom to format the code and pasted it into my module file. Today I wrote a script that will generate the module file from a .csv source file.

**Link to work:**
-   [PokemonGoRaidZones Commit](https://github.com/devNoiseConsulting/PokemonGoRaidZones/commit/b9a290dae808ea436cb08082f6ba64e7a7561783)

### Round 3, Day 24: Jan 27, 2018

**Today's Progress:** Started working on a Discord bot.

**Thoughts:** Trying to figure out how to create a Discord bot. Mostly looking through a tutorial, but also setting up the app/bot with Discord and getting some code to run.

**Link to work:**
-   [MegaBot commit](https://github.com/devNoiseConsulting/MegaBot/commit/3d2d5a80cdaf5ad2b4bba4c014ca019e7b455cbc)

### Round 3, Day 25: Jan 28, 2018

**Today's Progress:** More work on Discord bot.

**Thoughts:** Getting more commands into the bot. Looking at some code from the bot used on the MontCo/ChesCo Raids Discord server. They used Eris as they framework to talk to the Discord server. I'm using discord.js, so I'm porting some commands over. The bot's permissions are not setup correctly to handle role assignment. Ignored that and focused on the "Unhandled Promise Rejection" warning. Converting the code to make more use of Promises so the error goes away. Then worked on making the code into a better module for some code reuse.

**Link to work:**
-   [MegaBot commit](https://github.com/devNoiseConsulting/MegaBot/commit/0c549263f99a71575db528a326fb869028ab73cf)

### Round 3, Day 26: Jan 29, 2018

**Today's Progress:** Discord bot is assigning roles and clearing messages.

**Thoughts:** Code looked good, but ran into `DiscordAPIError: Missing Permissions` or  `DiscordAPIError: Missing Access` errors when the bot tried to assign a new role. Was using permission calculators to give the bot the permissions, but still didn't work. Ended on Reddit to see if I could get some help. Turns out the solution was to reorder the roles on the server so that the bot was higher. The /r/Discord_Bots linked me to a different tutorial and started to use their shell for my bot. So I started working on the nest feature which will store users input to a sqlite file and then create a message based off of the data in sqlite.

**Link to work:**
-   [Plea for help](https://www.reddit.com/r/Discord_Bots/comments/7ttd58/get_missing_permissions_when_trying_to_add_a_role/)
-   [MegaBot commit - Team Assignment](https://github.com/devNoiseConsulting/MegaBot/commit/03bd8678fed55346a1419f734bf0a7ecc8deddd0)
-   [MegaBot commit - Nest List](https://github.com/devNoiseConsulting/MegaBot/commit/1a0ab1f89005a0c73e122ac14e13644cdb00a499)

### Round 3, Day 27: Jan 30, 2018

**Today's Progress:** MegaBot command fix and merge. Contributing to variadic.js

**Thoughts:** Seems like the test bot I wrote may become the new bot for the MontCo/ChesCo Raids Discord server. Changed the assignTeam function to remove old team rolls. Received a pull request from one of the bot coders.
Looking to collaborate on a side project for the Grow with Google Challenge Scholarship. Started to help out on the variadic.js project. Took the standard deviation task/issue. Cribbing some notes from Wikipedia on the process and wrote some ES5 code to get it done. Then the real work was to get the Jasmine test working. Started with a copy from another test and started tweaking the test. Had to change some of the test data so I would cause all of the errors to be thrown. Checked it in and made a pull request.

**Link to work:**
-   [MegaBot commit - Remove old teams](https://github.com/devNoiseConsulting/MegaBot/commit/f8e936e10f0451dc869fef591e72932ca45a6630)
-   [MegaBot merge](https://github.com/devNoiseConsulting/MegaBot/commit/52296c24496bcab9b3d0fee9519da2450e8f986c)
-   [variadic.js commit - Standard Deviations](https://github.com/devNoiseConsulting/variadic.js/commit/2b4465e0d8dcca3087cf93366311dac5897cbf93)
-   [variadic.js Pull Request](https://github.com/variadicjs/variadic.js/pull/39)

### Round 3, Day 28: Jan 31, 2018

**Today's Progress:**

**Thoughts:** Worked on variance math functions for variadic.js. Which includes writing tests and making pull requests.

**Link to work:**
-   [variadic.js commit - Standard Deviations](https://github.com/devNoiseConsulting/variadic.js/commit/2b4465e0d8dcca3087cf93366311dac5897cbf93)
-   [variadic.js Pull Request](https://github.com/variadicjs/variadic.js/pull/39)

### Round 3, Day 29: Feb 1, 2018

**Today's Progress:** Enhancing the nest command on MegaBot

**Thoughts:** Working through what features the nest command needs. Refactored the code a bit to extract code that would be common to the sub commands. That ended up being the clear messages and post new nest list. To avoid a load of promise chaining, I used the async/await feature. Mostly used on the delete messages as I didn't want to have the new nest list posted and getting deleted.

**Link to work:**
-   [MegaBot commit - Nest and more linting commit](https://github.com/devNoiseConsulting/MegaBot/commit/f8e936e10f0451dc869fef591e72932ca45a6630)

### Round 3, Day 30: Feb 2, 2018

**Today's Progress:** Started working on Wes Bos's CSS Grid class.

**Thoughts:** Was meaning to start this earlier, but had other coding projects take my time since this launched. From what I've seen this looks like a nice way to layout web pages. Wonder how this replaces or works with Flexbox.

**Link to work:**
-   [CSS Grid class](https://cssgrid.io/)

### Round 3, Day 31: Feb 3, 2018

**Today's Progress:** More work on Wes Bos's CSS Grid class.

**Thoughts:** Doing my bare minimum hour this weekend. CSS Grid seems to be pretty nice.

**Link to work:**
-   [CSS Grid class](https://cssgrid.io/)

### Round 3, Day 32: Feb 4, 2018

**Today's Progress:** More work on Wes Bos's CSS Grid class.

**Thoughts:** Got my hour in and that's about it. Seeing lots of good stuff with CSS Grid. Think this might make responsive design a lot easier. May not need to rely on CSS frameworks as much.

**Link to work:**
-   [CSS Grid class](https://cssgrid.io/)

### Round 3, Day 33: Feb 5, 2018

**Today's Progress:** Working on exercises for Wes Bos's CSS Grid class.

**Thoughts:** Getting to the last third of the course. I have been working along with the videos to make a similar page, Now the course is switching to having me pause the video and attempt a solution. Getting close, but still need help to complete them. I'm not baffled by the solution, but I'm forgetting pieces of CSS Grid.

**Link to work:**
-   [CSS Grid class](https://cssgrid.io/)

### Round 3, Day 34: Feb 6, 2018

**Today's Progress:** Working on a factorial function to variadic.js

**Thoughts:** Saw an issue come up requesting a factorial function and assigned it to myself. Found an answer on Stack Overflow that was close what we needed. Converted it into the module form that we needed. Turns out by 19!, the code is generating a number bigger than `Number.MAX_SAFE_INTEGER`. Added a comment to the issue to get some input from the other team members.

**Link to work:**
-   [variadic.js commit - Factorial](https://github.com/devNoiseConsulting/variadic.js/commit/7ee074f928b4858ecbb32633b98b9af7c00f8838)

### Round 3, Day 35: Feb 7, 2018

**Today's Progress:** Working on test spec for variadic.js and Philly.net meeting.

**Thoughts:** Got some feedback on the factorial issues and moved ahead with writing the test specs. Ideally, I should write the test first, but I tend to jump into getting working code. Tests are all passing, just have an issue with uncovered lines of code. Not sure what the issue is. Also attend a Philly.net meeting that did a basic overview of React, Angular, and Vue.js. Forked some projects and followed along making the code changes to see how things worked.

**Link to work:**
-   [variadic.js commit - Factorial](https://github.com/devNoiseConsulting/variadic.js/commit/1ef8d677bb9b333150e20960bf4d377fa7c4716e)
-   [React with Routing, NFL SPA](https://codesandbox.io/s/8y0k3vxyo8)
-   [React with Routing and Data, NFL SPA](https://codesandbox.io/s/n4r7q42xn4)
-   [Vue with Routing, NFL SPA](https://codesandbox.io/s/71ww71k6k0)
-   [Vue with Routing and Data, NFL SPA](https://codesandbox.io/s/8kvqx09nzj)
-   [Angular with Routing, NFL SPA](https://stackblitz.com/edit/angular-7qarzy)
-   [Angular with Routing and Data, NFL SPA](https://stackblitz.com/edit/angular-nsyl3y)

### Round 3, Day 36: Feb 8, 2018

**Today's Progress:** Fixed code so jasmine is happy and making S2 cells for Pokemon Go Raid zones map.

**Thoughts:** Getting back to my Factorial function and trying to figure what's wrong with line 12. No real indication of what it didn't like, just a line number. I want my 100%! So I took a closer look at the code and realized that the ternary operator wasn't needed at all and I could simplify the logic. Getting rid of the ternary operator got rid of my uncovered line of code. Committed and made a pull request.

**Link to work:**
-   [variadic.js commit - Factorial](https://github.com/devNoiseConsulting/variadic.js/commit/1ef8d677bb9b333150e20960bf4d377fa7c4716e)
-   [variadic.js Pull Request](https://github.com/variadicjs/variadic.js/pull/59)
-   [PokemonGoGIS commit](https://github.com/devNoiseConsulting/PokemonGoGIS/commit/d9331bad5b551b30eec47d36b0e41122edf7b531)
-   [PokemonGoRaidZones commit](https://github.com/devNoiseConsulting/PokemonGoRaidZones/commit/06f7bdfcea39537b6766d9a5508e807023088156)

### Round 3, Day 37: Feb 9, 2018

**Today's Progress:** Fixed a coding style problem in variadic.js and getting more S2 neighbor cells for Pokemon Go Raid zones map.

**Thoughts:**

**Link to work:**
-   [variadic.js commit - Factorial](https://github.com/devNoiseConsulting/variadic.js/commit/faf5e2df13791abb6924a35daa97002a4f295d18)
-   [PokemonGoGIS commit](https://github.com/devNoiseConsulting/PokemonGoGIS/commit/0177d97f972f25bc0ebab28b10c1509d215a4447)

### Round 3, Day 38: Feb 10, 2018

**Today's Progress:** More work on Wes Bos's CSS Grid class.

**Thoughts:** Doing my bare minimum hour this weekend. Looked a bit at how flexbox and css grid can and can't do similar things.

**Link to work:**
-   [CSS Grid class](https://cssgrid.io/)

### Round 3, Day 39: Feb 11, 2018

**Today's Progress:** Trying to get Raspbian setup.

**Thoughts:** More work on getting Raspbian setup on an SD card multiple partitions. Would like a second partition that is FAT32 for making it easy to load videos onto the SD card without having to use scp or ftp. Lots of failed attempts using NOOBS or trying to use fdisk to resize/shink the parition and create a new one. NOOBS didn't like that I removed OSs from the SD card to make a new parition. Shinking the partition resulted in a kernel panic.

**Link to work:**
-   [Pi Notes Gist](https://gist.github.com/devNoiseConsulting/4e97be9aedc0ca0c5509dd891014f285)

### Round 3, Day XX: Feb 12, 2018 - Feb 18, 2018
**Today's Progress:** No progress.

**Thoughts:** Working on a Raspberry Pi project that I'm going to be paid for. So a lot of my time shouldn't count toward my hour of code. With that disclosed, I'm not being paid a fair wage for the time I've sunk into this project.

Also I went on vacation for a couple days. I tried to code, but didn't really get the time in. More rides! Single rider line forever!

### Round 3, Day 40: Feb 16, 2018
**Today's Progress:** Starting UI improvements to myGeoBeerMap

**Thoughts:** First try at moving some buttons into a navber dropdown.

**Link to work:**
-   [myGeoBeerMap commit - Add dropdown to nav](https://github.com/devNoiseConsulting/myGeoBeerMap/commit/83a42673db5b3bd4f981b1165e5fcbb1f44d2858)

### Round 3, Day 41: Feb 19, 2018
**Today's Progress:** Daily Programmer is active again.

**Thoughts:** While I was on vacation, the person who ran the #daily_programmer started posted challenges again. Made use of some ES6 array features to complete the task. Wrote a second solution stream lined the code a faction.

**Link to work:**
-   [Number Diamond - PhillyDev Slack #daily_programmer](https://gist.github.com/devNoiseConsulting/aa9e4ee1d2c202df58daecffa637b9fd)

### Round 3, Day 42: Feb 20, 2018
**Today's Progress:** More Daily Programmer.

**Thoughts:** The concept of today's challenge was good, the execute was a bit of a pain. Since the input consisted of `\`, I had to work around the fact the JavaScript would escape half of my `\`s. This also broke the code and the input had an odd number of `\`s. Wrote three solutions for this. The second was really just a big chaining of the first solution. The third solution was based off of an answer that someone else gave. My solution made use of template literals but the `' '.repeat(i)` was totally from the other answer.

**Link to work:**
-   [Draw Doodle - PhillyDev Slack #daily_programmer - 20180220](https://gist.github.com/devNoiseConsulting/7c1c03e92e2063b7bde14e27504acb88)

### Round 3, Day 43: Feb 21, 2018
**Today's Progress:** A bit more of the same Daily Programmer

**Thoughts:** A challenge similar to yesterday's but the now we have `/` in the input. This means the amount of padding could decrease as well. Took my third solution from yesterday and adding in the logic to change the amount of padding. Also just gave up on the input and manually escaped all the `\`s in the input strings.

**Link to work:**
-   [Draw Doodle II - PhillyDev Slack #daily_programmer](https://gist.github.com/devNoiseConsulting/23b528e9da503f65eb4b3f931b056b60)

### Round 3, Day 44: Feb 22, 2018
**Today's Progress:** Daily Programmer Fail.

**Thoughts:** This one kicked my butt. I had code that was similar from a challenge last year, but I couldn't make it work. Something was wrong with the logic on determine what direction the code should move through the 2D array. I had to give up. Note link to my work is the working solution. Stay tuned

**Link to work:**
-   [Alphabet Spiral- PhillyDev Slack #daily_programmer](https://gist.github.com/devNoiseConsulting/b9fbe56413c577d72fcffd1acc576cb5)

### Round 3, Day 45: Feb 23, 2018
**Today's Progress:** Daily Programmer Success.

**Thoughts:** Continued to work on the previous day's challenge. Ended up switching over to multiple loops so the code moved through the 2D array correctly.

**Link to work:**
-   [Alphabet Spiral- PhillyDev Slack #daily_programmer](https://gist.github.com/devNoiseConsulting/b9fbe56413c577d72fcffd1acc576cb5)

### Round 3, Day 46: Feb 24, 2018
**Today's Progress:** Trying to migrate myGeoBeerMap to a Parcel.JS build

**Thoughts:** Parcel.JS is working fine for my PokemonGoRaidZones map. Thought I'd make the change from Gulp.JS since I getting some errors with recent updates to Gulp.JS. Also worked on the navbar dropdown.

**Link to work:**
-   [myGeoBeerMap commit - Parcel.js Build and navber changes](https://github.com/devNoiseConsulting/myGeoBeerMap/commit/f0d9fffd2488757080949f1898db9f101135ab08#diff-b9cfc7f2cdf78a7f4b91a753d10865a2)

### Round 3, Day 47: Feb 25, 2018
**Today's Progress:** Trying to get myGeoBeerMap to work.

**Thoughts:** Still running into problems with the Parcel.JS build for myGeoBeerMap. Code builds without errors, but no data is loaded onto the map. The Javascript used a fetch call to get the data from a .geojson file. The data file doesn't make into the dist folder. Tried making changes to package.json so that a script would copy it into the dist folder. Unfortunately, the Parcel.JS dev server redirects all call it doesn't know about to index.html. So even though it's in dist, the server won't give it to me.

**Link to work:**
-   [myGeoBeerMap commit - Attempt to include geoJSON data](https://github.com/devNoiseConsulting/myGeoBeerMap/commit/b8d68d7a523c002f3838623f66561cef624d0952)

### Round 3, Day 48: Feb 26, 2018
**Today's Progress:** Adding polygon zones to the PokemonGoRaidZones map and daily programmer challenge.

**Thoughts:** My discord group is switching the bot that scan for us. We now have the option to plot out the zones instead of a radius around a LatLng point. A lot of the work on this doesn't count as its not coding, but I still spent more than my hour to get the polygons into the map and making changes to the map display.

The daily programmer challenge was pretty quick. Needed to have a variable outside the scope of the reduce function. I would stuff the odd numbers in there and then add the reverse order to the accumulator array when have an even number. Made use of the spread operator to build an array that was concatted to the accumulator array.

**Link to work:**
-   [PokemonGoRaidZones
 commit - Adding polygon zones.](https://github.com/devNoiseConsulting/PokemonGoRaidZones/commit/77d8801bcccb53415d27af0a9e7780b17062bff7)
-   [Reverse Odd Runs - PhillyDev Slack #daily_programmer](https://gist.github.com/devNoiseConsulting/c5ac3aeaa1f14f03f61fa0ba24899497)

### Round 3, Day 49: Feb 27, 2018
**Today's Progress:** Trying to get myGeoBeerMap to build for production

**Thoughts:** While the code doesn't run, it does build for dev. Received an error when trying to build for production. Spend a lot of time trying to track this down and figure it out. End result from some searches was to downgrade Bootstrap to a beta version so everything is happy. Feel that Parcel.JS needs to update autoprefixer.

***Errors***:
`Node#moveTo was deprecated. Use Container#append.`
`Unknown error from PostCSS plugin. Your current PostCSS version is 6.0.19, but autoprefixer uses 5.2.18. Perhaps this is  /Users/flynnmj/src/myGeoBeerMap/node_modules/bootstrap/dist/css/bootstrap.css:undefined:undefined: Unknown browser ma`

`/Users/flynnmj/src/myGeoBeerMap/node_modules/bootstrap/dist/css/bootstrap.css:undefined:undefined: Unknown browser major`

Also tried to get change the fetch call to get the data file from the production server. The network panel shows that it get the data, but it doesn't seem to make it to my code. Some sort of CORS issue I'm sure. Unfortunately, I can't seem to figure out what options I need to change to make it work.

**Link to work:**
-   [myGeoBeerMap commit - Downgrade BootStrap and change fetch](https://github.com/devNoiseConsulting/myGeoBeerMap/commit/178688353db5d211f7614bc407a79a48f75bc37b)


### Round 3, Day XX: Feb 28, 2018
**Today's Progress:** Getting caught up on my log.

**Thoughts:** Had a bit of a lapse. Started coding but didn't log it. Got out of hand, but took the time to get the log back on track today.

**Link to work:**
-   [100-days-of-code-3 commit - Days 40-49](https://github.com/devNoiseConsulting/100-days-of-code-3/commit/50a67b892a8fb742fbbc5bd9088f28a8f64c7317)

### Round 3, Day 50: Mar 01, 2018
**Today's Progress:** Trying to debug Parcel.JS build

**Thoughts:** Create a new repo to see if I can duplicate the issue that I'm having. When I go to make a production build, I get an error (`Unknown browser major`). Bootstrap seem to be the instigator, but seems like cssnano is the culprit.

**Link to work:**
-   [parcel-bootstrap-test commit](https://github.com/devNoiseConsulting/parcel-bootstrap-test/commit/5c60a1d7ed4eb5711c93781cc5e6dd923ce6bde9)
-   [parcel bug #645](https://github.com/parcel-bundler/parcel/issues/645)
-   [cssnano bug #447](https://github.com/ben-eb/cssnano/issues/447)

### Round 3, Day 51: Mar 02, 2018
**Today's Progress:** More navbar changes for myGeoBeerMap.

**Thoughts:** Making more changes to the UI for better mobile experience. Unfortunately parcel.js breaks are making this hard to verify. May look into using webpack for this project.

**Link to work:**
-   [myGeoBeerMap commit](https://github.com/devNoiseConsulting/myGeoBeerMap/commit/a65bc7a12aa48fa841d009da43bc4b60dd7d7d87)

### Round 3, Day 52: Mar 03, 2018
**Today's Progress:** Started Udacity's Web Tooling & Automation course

**Thoughts:** Discouraged by issues with Parcel.JS. I'm looking into doing some course work to step back from my projects.

**Link to work:**
-   [Web Tooling & Automation](https://www.udacity.com/course/web-tooling-automation--ud892)

### Round 3, Day 53: Mar 04, 2018
**Today's Progress:** Continued Udacity's Web Tooling & Automation course

**Thoughts:** Just squeezing an hour in today. Unfortunately, this course seems a little dated. While Sublime is a decent editor, it seems like the dev community has moved on to VSCode or Atom. Gulp is a good build tool for JavaScript, but Webpack seems to have the mind share today.

**Link to work:**
-   [Web Tooling & Automation](https://www.udacity.com/course/web-tooling-automation--ud892)

### Round 3, Day 54: Mar 05, 2018
**Today's Progress:** Started Udacity's Intro to Progressive Web Apps

**Thoughts:** Based off of some posts to the Grow with Google challenge slack, I decided to start the Intro to Progressive Web Apps course.

**Link to work:**
-   [Intro to Progressive Web Apps](https://www.udacity.com/course/intro-to-progressive-web-apps--ud811)

### Round 3, Day 55: Mar 06, 2018
**Today's Progress:** Continued Udacity's Intro to Progressive Web Apps

**Thoughts:** Still on the basics, where we're trying to get the HTML and JavaScript into the App shell. This should allow us to handle caching parts of the app for future visits.

**Link to work:**
-   [Intro to Progressive Web Apps](https://www.udacity.com/course/intro-to-progressive-web-apps--ud811)

### Round 3, Day 56: Mar 07, 2018
**Today's Progress:** Nuking it from Orbit

**Thoughts:** Doing a bit of devops today. Trying to figure out how to keep RocketMap running on a droplet. We probably need a bigger droplet. So I felt like things were not in a clean state when we restarted scripts. This lead me to writing a bash script that would:
-   Kill all processes related to scanning.
-   Restart the mysql database.
-   Start both PoGoMap scripts.
-   Start the PokeAlarm script.
Added this script to cron so every morning we can start the day with a good clean state. Hopefully this will keep everything running during the day.

**Link to work:**
-   [XXX commit - XXX](https://github.com/devNoiseConsulting/)

### Round 3, Day 57: Mar 08, 2018
**Today's Progress:** Completed Lesson 1 for Udacity's Intro to Progressive Web Apps

**Thoughts:** Finishing out the lesson with some browser storage. A bit frustrating to not see an instructor notes that were mentioned in the video. Was going to use Jake Archibald's [idb lib](https://github.com/jakearchibald/idb), but tooling on the code is non existent. Not sure how I could use it when I import the lib into my code. So I peaked at the solution and used [localForage](https://github.com/localForage/localForage) as well. I loaded the lib from a CDN and attempted with get it working without further peaking.

**Link to work:**
-   [Intro to Progressive Web Apps](https://www.udacity.com/course/intro-to-progressive-web-apps--ud811)

### Round 3, Day 58: Mar 09, 2018
**Today's Progress:** Started Lesson 2 for Udacity's Intro to Progressive Web Apps

**Thoughts:** Moving into the service worker portion of Progressive Web Apps. Not very successful in getting code to work.

**Link to work:**
-   [Intro to Progressive Web Apps](https://www.udacity.com/course/intro-to-progressive-web-apps--ud811)

### Round 3, Day 59: Mar 10, 2018
**Today's Progress:** Falling down the JavaScript syntax hole.

**Thoughts:** While trying to figure out some of my Parcel.JS build issues, I looked for some examples. Should I import everything in the index.js or do I load them in via script tags in index.html? My code is doing the latter and I'm trying to figure out if the former is better. Found a [GitHub repo](https://github.com/potato4d/parcel-examples) that has some Parcel.JS examples. So looking at the VanillaJS example I see a line `$('#root')...` in the javascript. I expect that to be jQuery syntax, but don't see jQuery being included. I try similar syntax to select a DOM element from the console and it works. This leaves me confused as I really haven't seen in any of the modern JavaScript course work I've taken.

**Link to work:**
-   [parcel-examples](https://github.com/potato4d/parcel-examples)

### Round 3, Day 60: Mar 11, 2018
**Today's Progress:** Continuing Lesson 2 for Udacity's Intro to Progressive Web Apps

**Thoughts:** Really trying to make my code work and not just copy the solution into my code. Getting lost in the details. On the install event, my code will pre fetch a list of URLs to cache. Also believe that my code will clear the cache on the activate event. The fetch event is all fubar. What I have been basing my work off of is the examples on Mozilla's Developer Network. I feel like I follow it, keep getting `undefined` as the cached response. Then the page breaks. Really feels like I need a check list to follow to make sure the browser is in the state I want it so I can test that the code is working.

**Link to work:**
-   [Intro to Progressive Web Apps](https://www.udacity.com/course/intro-to-progressive-web-apps--ud811)

### Round 3, Day 61: Mar 12, 2018
**Today's Progress:** Nuking it from Orbit

**Thoughts:** Seems like we have to many threads/workers running on the server. Sometimes a simple restart doesn't do the trick. The server runs out of memory to run the processes and a couple will be killed by the OS. Problem being that sometimes that ends up being one of the MySQL/MariaDB processes. Then the database is in a funky state where the processes are no longer connected. Thus I wrote a script to kill all the processes, restart the database and then get the processes running again.

**Link to work:**
-   [nukeItFromOrbit.sh gist](https://gist.github.com/devNoiseConsulting/a9b066141b007387bcb0327875e43bd9)

### Round 3, Day 62: Mar 13, 2018
**Today's Progress:** Completed Lesson 2 for Udacity's Intro to Progressive Web Apps

**Thoughts:** I was bad and didn't keep notes on my thoughts.

**Link to work:**
-   [Intro to Progressive Web Apps](https://www.udacity.com/course/intro-to-progressive-web-apps--ud811)

### Round 3, Day 63: Mar 14, 2018
**Today's Progress:** Started Lesson 3 for Udacity's Intro to Progressive Web Apps

**Thoughts:** I was bad and didn't keep notes on my thoughts.

**Link to work:**
-   [Intro to Progressive Web Apps](https://www.udacity.com/course/intro-to-progressive-web-apps--ud811)

### Round 3, Day 64: Mar 15, 2018
**Today's Progress:** Finished Lesson 3 for Udacity's Intro to Progressive Web Apps and started Lesson 6 for Udacity's Web Tooling & Automation

**Thoughts:** I was bad and didn't keep notes on my thoughts. Though I recall that I found out that I still had a lesson to do in Web Tooling & Automation.

**Link to work:**
-   [Intro to Progressive Web Apps](https://www.udacity.com/course/intro-to-progressive-web-apps--ud811)
-   [Web Tooling & Automation](https://www.udacity.com/course/web-tooling-automation--ud892)

### Round 3, Day 65: Mar 16, 2018
**Today's Progress:** Finished Lesson 6 for Udacity's Web Tooling & Automation

**Thoughts:** I was bad and didn't keep notes on my thoughts.

**Link to work:**
-   [Web Tooling & Automation](https://www.udacity.com/course/web-tooling-automation--ud892)

### Round 3, Day 66: Mar 18, 2018
**Today's Progress:** Doing some password generation and sed scripting.

**Thoughts:** Found a script that would let bulk create some accounts and passwords. Unfortunately, raspbian has an older version, 2.0.7, of pwgen installed. So I can't used the `-y` option to omit certain characters. Spent a lot of time piping the output to sed and seeing if I could create a regex that did the same thing. To many special characters was making this hard to pull off. In the end I decide to chunk the password and insert the same special characters between the chunks. Not the most secure passwords, but would suit my needs.

**Link to work:**
-   [genaccts.sh](https://pastebin.com/nF2rviJM)
-   `pwgen -c -n -s 9 1 | sed -E 's/(.{3})(.{3})(.{3})/\1!\2?\3+/'`

### Round 3, Day 67: Mar 21, 2018
**Today's Progress:** Setting up myGeoBeerMapTest to test out Webpack 4.0 builds

**Thoughts:** With Parcel.JS lettting me down for a production build. Started to look into the newwer features of Webpack 4. Reading some articles and getting a test repo setup.

**Link to work:**
-   [myGeoBeerMapTest
 commit - Initial commit](https://github.com/devNoiseConsulting/myGeoBeerMapTest/commit/b2665e90a7ce52cc6259b1f3a41981e9c0c8ea25)

### Round 3, Day 68: Mar 22, 2018
**Today's Progress:** More testing out Webpack 4.0 builds on myGeoBeerMapTest

**Thoughts:** Getting webpack installed and trying to get the project running.

**Link to work:**
-   [myGeoBeerMapTest
 commit - Trying out Webpack 4](https://github.com/devNoiseConsulting/myGeoBeerMapTest/commit/d204a891a603640f4d8f3d722f9cabc386ac6fed)

### Round 3, Day 69: Mar 23, 2018
**Today's Progress:** Philly.NET's Code Camp 2018.1 Workshop

**Thoughts:** Spent the day at Philly.NET's Code Camp. Attended Chris Love's workshop on Progressice Web Apps.

**Link to work:**
-   [Philly.NET's Code Camp 2018.1](http://phillydotnet.org/camps/2018-1/)
-   [Progressive Web Apps From Beginner to Expert](http://phillydotnet.org/sessions/progressive-web-apps-from-beginner-to-expert/)

### Round 3, Day 70: Mar 24, 2018
**Today's Progress:** Philly.NET's Code Camp 2018.1

**Thoughts:** Not really a .NET developer, but I can find a good set of sessions that matched up with my interests.

**Link to work:**
-   [Philly.NET's Code Camp 2018.1](http://phillydotnet.org/camps/2018-1/)
-   [Vue + Vuetify + Vuex](https://phillycc.love2dev.com/session/vue-vuetify-vuex/)
-   [The Server is Dead! Going Serverless to Create a Highly Scalable Application You Can Manage](https://phillycc.love2dev.com/session/the-server-is-dead-going-serverless-to-create-a-highly-scalable-application-you-can-manage/)
-   [Optimizing ReactJS](https://phillycc.love2dev.com/session/optimizing-reactjs/)
-   [Creating a Progressive Web Application (PWA) From Scratch to Engaging App
Chris](https://phillycc.love2dev.com/session/creating-a-progressive-web-application-pwa-from-scratch-to-engaging-app/)
-   [Introduction to React Native with Redux](https://phillycc.love2dev.com/session/introduction-to-react-native-with-redux/)

### Round 3, Day 71: Mar 26, 2018
**Today's Progress:** Working on a manifest.json for the Inner Sphere Atlas

**Thoughts:** Using the PWABuilder site to get my manifest.json. Renaming some icons files to match up with all the new icons. Updated templates, then adding the new icons and the manifest.json.

**Link to work:**
-   [InnerSphereAtlas commit - Preparing for Manifest.json](https://github.com/devNoiseConsulting/InnerSphereAtlas/commit/4266f9bf3218a015122e26bccf8ad35b297a2768)
-   [InnerSphereAtlas commit - Manifest.json](https://github.com/devNoiseConsulting/InnerSphereAtlas/commit/ec7d7b5b7409700678a9e4d7971b55f0a147e1b1)

### Round 3, Day 72: Mar 27, 2018
**Today's Progress:** Working on the service worker for the Inner Sphere Atlas

**Thoughts:** Started working on getting a service worker. At this point, it won't do much as the site is still really a dynamic PHP site.

**Link to work:**
-   [InnerSphereAtlas commit - Service Worker](https://github.com/devNoiseConsulting/InnerSphereAtlas/commit/d90a9ecb9f175f74bb3885eeea23790ba17afb06)

### Round 3, Day 73: Mar 29, 2018
**Today's Progress:** Writing a script to test out the pokemagic module.

**Thoughts:** Looking into using this module for a Pokemon/Discord Bot. Trying to figure out if some IV values can be pre calculated so the bot is only doing lookups. From initial tests, it looks like there are to many values to return. This will make a bot very spammy. Waiting to hear feedback from other coders on the discord server.

**Link to work:**
-   [Pokemon-IV-Test commit - Catch Calcs](https://github.com/devNoiseConsulting/Pokemon-IV-Test/commit/aa47b08cacb072506ae333a040ac4d6484886318)

### Round 3, Day 74: Apr 1, 2018
**Today's Progress:** Adding a Service worker cache to PokemonGoRaidZones

**Thoughts:** Using parcel-plugin-sw-cache to have Parcel.JS create a service worker cache for the site.

**Link to work:**
-   [PokemonGoRaidZones commit - Adding a SW cache](https://github.com/devNoiseConsulting/PokemonGoRaidZones/commit/0579c0376c5b8f8ca1aa6dd5fb8e254828b35e7a)

### Round 3, Day 75: Apr 2, 2018
**Today's Progress:** No real progress on PokemonGoRaidZones due to build errors in Parcel.JS.

**Thoughts:** Started working on getting a manifest.json setup for PokemonGoRaidZones. I can waste a lot of time working on graphics. Decided to clean up the repo a bit by moving most of the code to a new src dir. One I did this and cleaned up links into the node_modules dir, I get `🚨  Cannot read property 'js' of null` as the build error. Not really getting a good idea were the error comes from. Went with a `git reset --hard 0579c03` to be me back to yesterday's state. Still have the error. I give up for today.

**Link to work:**
-   [PokemonGoRaidZones commit - Adding a SW cache](https://github.com/devNoiseConsulting/PokemonGoRaidZones/commit/0579c0376c5b8f8ca1aa6dd5fb8e254828b35e7a)

### Round 3, Day 76: Apr 3, 2018
**Today's Progress:** Creating some offline html for the service worker to cache, but then 501.

**Thoughts:** Realized my basic service worker from [PWABuilder](http://www.pwabuilder.com/) wants to cache `offline.html`. Which I hadn't made yet. So I made a copy of the `index.html` template and started work on `offline.html`. Installed the [CSS Used](https://chrome.google.com/webstore/detail/css-used/cdopjfddjlonogibjahpnmjpoangjfff)
 extension for Chrome to get the a copy of the CSS in use by the page. Once deployed, the website just gives me a blank web page. Having a hard time tracking down the error logs for the PHP code so I can see what went wrong.

**Link to work:**
-   [InnerSphereAtlas commit - Offline HTML](https://github.com/devNoiseConsulting/InnerSphereAtlas/commit/669eea6ce4107997198a746c8855264458417609)

### Round 3, Day 77: Apr 4, 2018
**Today's Progress:** Fixed Content Security Policy to allow Service Worker to work.

**Thoughts:** Think the problems I had yesterday were due to me breaking the Content Security Policy header. To prevent down time, I set up a test domain that I could deploy the new code to. Chrome is not liking inline javascript. So this was breaking the service worker as the page couldn't load it. Move the code into a seperate javascript file, and later had to move the Google analytics code in as well. With the service worker installed, the page looks like crap. Back to the Content Security Policy and add all external dependencies to the `connect-src` section as well.

**Link to work:**
-   [InnerSphereAtlas commit - Content Security Protocol](https://github.com/devNoiseConsulting/InnerSphereAtlas/commit/77d0b5631a90b15a92ad2636ce7d6cd590aa9909)

### Round 3, Day 78: Apr 6, 2018
**Today's Progress:** Refactoring some coding challenges.

**Thoughts:** Saw a link to a coding challenge on the Grow With Google slack server and decided to do it. So far these have been easy to do and I didn't consider mentioning them. Been semi active in a thread with other participants. My code is a mix of modern and standard JavaScript, but comments are pushing me to use as much ES2016+ as I can. One comment I saw today, made me refactor my code to handle the edge case that would cause it to fail. Another comment showed an abstraction I has thought about, but hadn't implemented yet. After taking the advice from the comments, I furthered refactored the code. Almost all of the arrow functions are now expressed as one liners. Once the challenge is over I'll be sure to post my code to a gist.

**Link to work:**
-   [21 Day Coding Challenge](https://coding-challenge.lighthouselabs.ca/start)

### Round 3, Day 79: Apr 7, 2018
**Today's Progress:** Started working with Google Lighthouse and Workbox

**Thoughts:** Working on my Google Lighthouse audit. The trying to replace the service worker with the one generated my Google Workbox. Ran into some deployment issues.

**Link to work:**
-   [InnerSphereAtlas commit - Workbox integration](https://github.com/devNoiseConsulting/InnerSphereAtlas/commit/2324d11b728c3ad2b21f383a3f8eb8a93a600f1a)

### Round 3, Day 80: Apr 8, 2018
**Today's Progress:** Reviewing my Google Lighthouse Audit and revising my deployment script.

**Thoughts:** Working on correcting some of the items in the Lighthouse audit. The Content Security Policy was the cause of a couple errors. Had to add a `manifest-src` option to the policy so Chrome could load the manifest.json. Updated a couple external dependencies (ie BootStrap/jQuery). Will have to look into getting the http request to be served as httpd.

Revised the install script so that it uses sed to inject the Google Analytics ID. The will help cut down on manual edits to files on the server.

**Link to work:**
-   [InnerSphereAtlas commit - Lighthouse tweaks](https://github.com/devNoiseConsulting/InnerSphereAtlas/commit/9af175407b2018ed0e42a9d2198d883fd07e902c)

### Round 3, Day 81: Apr 9, 2018
**Today's Progress:** Working on improving the accessibility part of the Google Lighthouse Audit.

**Thoughts:** Mostly adding some aria-labels to improve accessibility. Started with the social media links in the footer and then the icons that indication descriptions or factories present on the planet. Adding the manifest.json and theme-color to the site’s pages.

**Link to work:**
-   [InnerSphereAtlas commit - Lighthouse tweaks again](https://github.com/devNoiseConsulting/InnerSphereAtlas/commit/9f3a20545c26da38cf022c2b54e15418a14f58ee)

### Round 3, Day 82: Apr 10, 2018
**Today's Progress:** Fighting with the code challenge interpreter.

**Thoughts:** First off the challenge was not very tricky. Understood exactly what they wanted and had some a good idea how to implement it. The code editor in the browser is ok, but I prefer the setup I have in Atom. So I have been writing the code in Atom and testing it with Node.js. Came up with a solution that worked, and did some refactoring. When I go to paste the new function into the browser, I get the following error when I run it: `Your code has a syntax problem. Please check it and try again.` Spent so much time trying to debug what should be a working solution, I'm declaring it my hour of code. Turns out that the site is only saving my code at the time of first successful completion of the challenge. So the site doesn't have all of my refactored code. After many rounds of debugging, I found out that the `const ROCK` wasn't defined. The error Node.js would give me for that is: `ReferenceError: ROCK is not defined`. Which would have been a lot easy to debug and fix.

**Link to work:**
-   [21 Day Coding Challenge](https://coding-challenge.lighthouselabs.ca/start)

### Round 3, Day 83: Apr 12, 2018
**Today's Progress:** Free React.js Bootcamp, Day 1.

**Thoughts:** Started taking a free React.js Bootcamp by Tyler McGinnis. Found it from a link on the Grow with Google slack. I'm a couple days behind, so I'm not watching the live stream. Covered the basics, and did the challenge code pens,

**Link to work:**
-   [Free React.js Bootcamp](https://tylermcginnis.com/free-react-bootcamp/)
-   [Props - 1](https://codepen.io/_dev_noise/pen/jzoPdJ)
-   [Props - 2](https://codepen.io/_dev_noise/pen/qoGdvR)
-   [Props - 3](https://codepen.io/_dev_noise/pen/MVdwMW)
-   [Props - 4](https://codepen.io/_dev_noise/pen/WzBvVm)

### Round 3, Day 84: Apr 13, 2018
**Today's Progress:** Free React.js Bootcamp, Day 2.

**Thoughts:** Continued the Free React.js Bootcamp. Making the web page more interactive. Also covering the problems around `this` and making sure to `.bind(this)` so we have the right context.

**Link to work:**
-   [Free React.js Bootcamp](https://tylermcginnis.com/free-react-bootcamp/)
-   [Day 2 Challenge Gist](https://gist.github.com/fe2f3c9b8c0bc9a7d6e89c22824ec27a)

### Round 3, Day 85: Apr 16, 2018
**Today's Progress:** Started Free React.js Bootcamp, Day 3.

**Thoughts:** Started day 3, but didn't have enough time to finish it. Focused on the React.js lifecycle with componentDidMount being the main one used.

**Link to work:**
-   [Free React.js Bootcamp](https://tylermcginnis.com/free-react-bootcamp/)

### Round 3, Day 86: Apr 16, 2018
**Today's Progress:** Finished Free React.js Bootcamp, Day 3.

**Thoughts:** Finished day 3. componentDidUpdate was the other main lifecycle method day 3 focused on. Can see componentDidMount and componentDidUpdate doing basically the same work. Should abstract/refactor that work into another function that will be called by both.
Made a local copy of the solution to make sure I had the same things displayed. Used the dev tools to inspect to figure out to code the styling. Had to look at the code a bit to figure out why I didn't have the same repos displayed. I only fetched the repo list once and then filtered the list based on the selected language. The solution code was fetching a new list of repos when a language was selected.

**Link to work:**
-   [Free React.js Bootcamp](https://tylermcginnis.com/free-react-bootcamp/)
-   [Day 3 Challenge Gist](https://gist.github.com/ddc930ca5db7d428cf0ddc4edb5708c0)

### Round 3, Day 87: Apr 16, 2018
**Today's Progress:** Free React.js Bootcamp, Day 4.

**Thoughts:** Finished the Free React.js Bootcamp. Going over the React Router v4. Covered setting up the routes and how to make sub routes in a component.

**Link to work:**
-   [Free React.js Bootcamp](https://tylermcginnis.com/free-react-bootcamp/)

<!--

### Rouond 3, Day 0: Jan 1, 2018 (Example 1)
##### (delete me or comment me out)

**Today's Progress** Fixed CSS, worked on canvas functionality for the app.

**Thoughts:** I really struggled with CSS, but, overall, I feel like I am slowly getting better at it. Canvas is still new for me, but I managed to figure out some basic functionality.

**Link to work:** [Calculator App](http://www.example.com)

-->
