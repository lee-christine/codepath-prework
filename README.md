# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Christine Lee**

Time spent: **6** hours spent in total

Link to project: (https://glitch.com/edit/#!/childish-fate-thunbergia?path=README.md%3A1%3A0)

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
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:
![](https://cdn.glitch.global/11db5f88-2a03-4f74-a8b5-260ae4fad8c5/ezgif.com-gif-maker.gif?v=1650689895726)
![](https://cdn.glitch.global/11db5f88-2a03-4f74-a8b5-260ae4fad8c5/ezgif.com-gif-maker.mov?v=1650690146002)
![](gif3-link-here)
![](gif4-link-here)

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
[YOUR ANSWER HERE]

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

Near the end of the project, I had to code a guess function that runs every time the player clicks a button. The function is used to make sure that the game responds properly after each move, either ending the game or playing the next clue sequence when appropriate. I used the flow chart as a guide to write the conditional logic inside the guess function, walking through the logic of the diagram and translating it into code. However, when I tested the game, it was not functioning properly – the game was ending even when I played the correct sequence. I realized that I was running the loseGame function every time the guess function was called because none of the functions inside the if statements contained a return statement and the code doesn’t exit out of the function, so I had to implement nested if statements. After rearranging my code, I walked through my logic and steps to make sure it would work properly.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

**How do I make sure my website is accessible to users?** How do I think about the users that will be using my product and how do I make sure that they will be able to use it smoothly? (ex. changing the colors to address color blindness)
**How do I organize my code?** As more features are added and the code gets more complicated, what are some best practices for organizing the code and providing good documentation?
**How do I test for bugs?** The game works well now, but what if there are unknown bugs? How do I run tests to cover every potential case?
**How do I optimize web applications to work as efficiently as possible?** How do I make sure that stuff is working efficiently and not taking too much memory and time especially as I keep adding more features?

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

If I had a few more hours to work on this project, I would complete the couple of optional features I did not get to, including the countdown timer to limit the amount of time the player has to make a guess. I would do more research into the setInterval and clearInterval functions and figure out how to apply them to creating a timer that starts and stops at the proper moments.
Additionally, there are some more features that I would want to implement. I would add a progress bar so players can see how far they’ve progressed in the game and how close they are to finishing it. I could implement this by changing the length of the bar after each turn to be a constant multiplied by a variable that keeps track of how many clues have been guessed correctly so far. I would also adjust the tones that the buttons play when clicked so that I can create more melodic patterns. I’d add a mistake counter that is visible throughout the game for players to check and know how many more mistakes they’re allowed to make before they lose the game. I have already created a counter for the mistakes when I implemented the feature of allowing players to make 2 mistakes without penalty, so I would just need to display this variable.




## Interview Recording URL Link

[My 5-minute Interview Recording](https://www.loom.com/share/6134b475d82f4ccb971b592b720f3a67)


## License

    Copyright [Christine Lee]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
