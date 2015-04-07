# FP4-proposal
Project Proposal is due 2015-04-08 at 8am

Produce a plan for your final project, and prepare an in-class presentation.

Ask questions, as always, [on piazza!][piazza]

## Written Proposal Instructions

Teams will submit ONE written proposal, with sections that each member has done individually detailing their proposed contributions. The submission will be on github, as a pull request of this very file. Below is a template proposal report.

You should be proposing something that you have high confidence that you can achieve, and the proposal should project that confidence.
The proposal should be no longer than necessary, but long enough to include critical detail. Three pages is appropriate. Diagrams are welcome.

Remember, you can do some neat [formatting things with Markdown.][markdown]

## In-Class Presentation Instructions
Teams will each deliver an in-class presentation. **Presentations will be Wednesday, April 8** (and Friday, April 10 as necessary). The presentation material is due on April 8 by 9 am for everybody. [See piazza for full schedule.][piazza]

Your team will have two minutes to present. Create presentation with two or three slides. Make the slides in google drive, and share the public-viewable link at the bottom of this report. The day of presentations, I'll have the list of links on the display computer, so each team can simply click their link and begin.

(Template follows. You may delete this line and all above it. Please edit the following template to create your report.)

# Project Title: Dr. Matchket
### Problem Statement
Racket lends itself particularly well to creating rules for a card-matching game. Using the cards and rsound libraries, we can programmatically create matched pairs (or larger sets) of cards which have unique characteristics that are reconciled within each pair or set.

### Problem Analysis
Explain what approaches from class you will bring to bear on the problem. Be explicit and succinct.

Each matched pair or set of cards will have a particular set of sound effects associated with it. (e.g., one for turning a particular type of card face-up, and another for matching all the cards of that type successfully.) This should do well to provide an audible cue to accompany the visual cue of the card face itself, helping players to match pairs or sets successfully.

### Data set or other source materials
<!--
If you will be working with existing data, where will you get those data from? (Dowload it from a website? access it in a database? create it in a simulation you will build....)

How will you convert that data into a form usable for your project?  

Do your homework here: if you are pulling data from somewhere, actually go download it and look at it. Explain in some detail what your plan is for accomplishing the necessary processing.

If you are using some other starting materails, explain what they are. Basically: anything you plan to use that isn't code.
-->
Sound effects will be generated programmatically via the rsound library.
Visual effects through the cards will be created using the games/cards library.

### Deliverable and Demonstration
Our live demonstration will feature the playable matching game, with players winning upon successfully matching all corresponding cards. We plan to shuffle the cards after a set number of incorrect guesses in lieu of a firm lose condition. Your score will be calculated using your failed attempts, as well as how long it took you to reach all of the matches.

### Evaluation of Results
How will you know if you are successful?
The purpose of a game is to entertain. As such, our success will depend largely on our ability to offer an entertaining experience through our core gameplay and audiovisual feedback features.

## Work Plan and Schedule
Explain how you will go from proposal to finished product. Write your general plan here.
There are three deliverable milestones to explicitly define, below. The nature of deliverables depend on your project, but may include things like processed data ready for import, core algorithms implemented, interface design prototyped, etc.

You will be expected to turn in code, documentation, and data (as appropriate) at each of these stages, so take care in writing concrete steps for your schedule.

In this general plan, and in the deliverables below.

### General Plan:
** 
1. Create scramble feature.
2. Determine how to create matches.
3. Begin point system using matches.
4. Deterime how to keep time.
5. Create a final point system based on time, matches and mispatches.

**

### First Milestone (04-13)
1. Have the scramble feature working for a set number of cards.
2. Begin to determine the point values for each element of the final score, and how it will be calculated.

### Second Milestone (04-21)
1. Integration of scramble feature with the rest of the game.
2. Completed scoring system.


## Group Responsibilities
Here each group member gets a section where they, as an individual, detail what they are responsible for in this project. Each group member writes their own Responsibility section. Include the milestones and final deliverable.

### Alex Li
will write the....

### Pat Quaratiello

Will be working on creating the scramble feature after there are several (possibly 5 - we'll need to test what is reasonable) failed attempts at matching cards. I will also be working on the point system with the help of the other members to determine how we can incorporate both missed matches and time into your total score, as well as successful matches.

### Peter Welby
will build...

## Proposal Presentation Link
[Google Slides Presentation][presentation]

<!-- Links -->
[piazza]: https://piazza.com/class/i55is8xqqwhmr?cid=453
[markdown]: https://help.github.com/articles/markdown-basics/
[presentation]: https://docs.google.com/presentation/d/1RS-RpMVcs_PuakTo_GzXePOPTVv_1goc3mxZHn5pIWY/edit?usp=sharing
