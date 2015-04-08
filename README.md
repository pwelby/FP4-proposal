# FP4-proposal

# Project Title: Dr. Match-it
### Problem Statement
Racket lends itself particularly well to creating rules for a card-matching game. Using the `cards` and `rsound` libraries, we can programmatically create matched pairs (or larger sets) of cards which have unique characteristics that are reconciled within each pair or set.

### Problem Analysis
<!--
Explain what approaches from class you will bring to bear on the problem. Be explicit and succinct.
-->
This project will rely heavily on the object-oriented facilities of Racket which we were introduced to in the lecture. The `cards` library uses local state to maintain the state of the game through the card table, and we will extend the card objects to keep track of the sound(s) they must play in response to particular gameplay events.

### Data set or other source materials
<!--
If you will be working with existing data, where will you get those data from? (Dowload it from a website? access it in a database? create it in a simulation you will build....)

How will you convert that data into a form usable for your project?  

Do your homework here: if you are pulling data from somewhere, actually go download it and look at it. Explain in some detail what your plan is for accomplishing the necessary processing.

If you are using some other starting materails, explain what they are. Basically: anything you plan to use that isn't code.
-->
We will design any assets which we cannot (or decide not to) define in code externally. Currently, we plan to design custom faces for our cards in Photoshop, which can be brought in as bitmaps. Additionally, some primitive sounds may be generated in Audacity if they cannot be adequately modeled by a generator procedure. These will be imported using the file I/O capabilities of the `rsound` library, and filtered to achieve the desired sound using the filter procedures we write.

### Deliverable and Demonstration
Our live demonstration will feature the playable matching game, with players winning upon successfully matching all corresponding cards. We plan to shuffle the cards after a set number of incorrect guesses in lieu of a firm lose condition. The player's score will be calculated using failed attempts, as well as how long it took to find all of the matches.

### Evaluation of Results
How will you know if you are successful?
The purpose of a game is to entertain. As such, our success will depend largely on our ability to offer an entertaining experience through our core gameplay and audiovisual feedback features.

## Work Plan and Schedule
<!--
Explain how you will go from proposal to finished product. Write your general plan here.
There are three deliverable milestones to explicitly define, below. The nature of deliverables depend on your project, but may include things like processed data ready for import, core algorithms implemented, interface design prototyped, etc.

You will be expected to turn in code, documentation, and data (as appropriate) at each of these stages, so take care in writing concrete steps for your schedule.

In this general plan, and in the deliverables below.
-->
### General Plan:

* Create scramble feature.
* Determine how to create matches.
* Begin point system using matches.
* Determine how to keep time.
* Create a final point system based on time, matches and mismatches.
* Design primitive sound generators and filters
* Synthesize final sounds through combination and filtering of primitives

### First Milestone (04-13)
* Have the scramble feature working for a set number of cards.
* Determine how to create matches.
* Begin to determine the point values for each element of the final score, and how it will be calculated.
* Initial set of primitive sound generators completed
* One or more filters completed
* Some, if not all, card faces designed

### Second Milestone (04-21)
* Integration of scramble feature with the rest of the game.
* Completed scoring system.
* Sound integration figured out with some sounds added to card objects and usable in-game

## Group Responsibilities
<!--
Here each group member gets a section where they, as an individual, detail what they are responsible for in this project. Each group member writes their own Responsibility section. Include the milestones and final deliverable.
-->

### Alex Li
Will be responsible for initializing the board state, as well as implementing the match checking system. The match checking system will called upon anytime there are two face up cards on the board. If the two cards are matching they will be removed, otherwise they will be flipped back down. Since this would be an ideal place to put any scoring procedures, I will also be working with other members on how to implement the scoring system.

### Pat Quaratiello
Will be working on creating the scramble feature after there are several (possibly 5 - we'll need to test what is reasonable) failed attempts at matching cards. I will also be working on the point system with the help of the other members to determine how we can incorporate both missed matches and time into your total score, as well as successful matches.

### Peter Welby
Will work primarily on building the sound effect system in `rsound`. This includes writing generators for primitive sounds, combining and filtering these primitives to create more interesting sounds for use in the game, and integrating these sounds with the core gameplay functionality. Additionally, I will design the custom card faces to be used in the game.

## Proposal Presentation Link
[Google Slides Presentation][presentation]

<!-- Links -->
[piazza]: https://piazza.com/class/i55is8xqqwhmr?cid=453
[markdown]: https://help.github.com/articles/markdown-basics/
[presentation]: https://docs.google.com/presentation/d/1RS-RpMVcs_PuakTo_GzXePOPTVv_1goc3mxZHn5pIWY/edit?usp=sharing
