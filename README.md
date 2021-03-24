# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Tyler Zamski

Time spent: 7 hours spent in total

Link to project: (insert your link here, should start with https://glitch.com...)

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [x] Buttons use a pitch (frequency) other than the ones in the tutorial
* [x] More than 4 functional game buttons
* [x] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [x] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [x] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough

Here's a walkthrough of implemented user stories:
http://g.recordit.co/pEXEvD5WB7.gif


## Reflection Questions
**1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here.**

  For picking colors:

  https://css-tricks.com/snippets/css/named-colors-and-hex-equivalents/ 
  https://www.w3schools.com/colors/colors_picker.asp

  For Finding Piano note frequencies:
  
  https://pages.mtu.edu/~suits/notefreqs.html
  
  For some more examples on creating a countdown timer:
  
  https://www.w3schools.com/howto/howto_js_countdown.asp

**2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words)** 

Though my experience with HTML, CSS, and JS was rather limited coming into this project, I had a relatively easy time completing the required features. I followed the instructions carefully, and within about 3 hours had created a fully working version of the template memory game. However, there was one additional feature that gave me quite a bit of trouble when completing the optional components: the clock timer. 

The given links to external references provided the necessary examples to create this feature, however there was an abundance of techniques and it was a process to determine which would be the most optimal in this scenario. In trying to adapt these techniques into my project, I encountered some pretty noticeable errors, such as a counter that would double its speed every time a button was clicked, a counter that wouldn’t reset, and a case where if the counter hit 0 the game would end up in an infinite loop of “you lose” alerts. 

To overcome these challenges, I started breaking my code down into smaller pieces to try and isolate the issues. The examples on w3schools.com provided a “try it yourself” button to test their methods with an interface similar to Glitch, and so I used their test environment to edit segments of my code. By working on only a single section of my code at a time, I was able to quickly identify and resolve errors in my code. My primary issue was a misunderstanding of the scope of my variable that contained the counter interval. Once I had fixed the scope issue and modified the related code segments, I was able to produce working start and stop functions for the timer. 

After creating the working pair of functions, I reimplemented them into my glitch project. Then, it was just a matter of determining where to call these functions inside the rest of my code. This final step really came down to some educated guesses, but now that I understood that my counter was just a global variable, figuring out the logic was straightforward-- start the timer whenever a sequence of clues is played, and stop the timer whenever the player presses the stop button. 


**3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words)** 

I’m sure I could probably come up with a couple dozen questions concerning web development, however there are a few that are at the forefront of my mind right now. In regards to front end development, I would like to know how to add more style to a website’s design. While I am happy with the results of my project, I recognize that it is relatively static, while in comparison many modern websites have dozens of dynamic elements on any given page. Also, I wonder what additional steps must be taken regarding development for mobile browsers. 

In terms of back-end design, I am curious to learn about how data is stored in web development. More specifically, I would like to know more about database management systems within web development, as I believe this is a crucial element of almost any modern website. One cannot create a complex website without a way to store data. On a related note, I would also be interested in learning about how a website saves cookies to a user’s browser. I am sure I will think of many other questions about web development as I continue to learn and practice, but for the time being these are the ones that have piqued my interest.


**4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words)** 

While working on this project, I found it enjoyable to just click through the buttons and play different sound patterns. If I had more time available, I would have tried to add an additional feature that would allow the user to record a series of button presses and then play it back. After figuring out the setInterval() function, I’m confident this playback feature could be capable of not only playing back the user’s input pattern, but also matching the duration of time each button was held for. 

If I was able to add this feature and still had additional time, I would then try to modify the way each colored button worked so that they could be pressed via keyboard inputs. Then, try to allow multiple button inputs to be recorded at once. My aforementioned issues with the clock timer feature taught me that it’s possible to have multiple intervals active at a time, so I believe this could be useful in implementing my idea. Each button might utilize its own interval to record input concurrently, thus allowing the output to play multiple tones at once. If I could get this feature to work, I would add some better sounding audio files to each button, and would have essentially created a virtual synthesizer.




## License

    Copyright Tyler Zamski

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.