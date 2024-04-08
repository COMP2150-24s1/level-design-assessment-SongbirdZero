[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/YyUO0xtt)
# COMP2150  - Level Design Document
### Name: Alanah O'Halloran
### Student number: 47841052

This document discusses and reflects on the design of your platformer level for the Level Design assessment. It should be 1500 words. Make sure you delete this and all other instructional text throughout the document before checking your word count prior to submission. Hint: You can check word count by copying this text into a Word or Google doc.

Your document must include images. To insert an image into your documentation, place it in the "DocImages" folder in this repo, then place the below text where you want the image to appear:

```
![Place any alt text here](DocImages/<IMAGE NAME AND FILE EXTENSION>)
```

Example:

![This is the alt text for an image!](DocImages/exampleimage.png)

## 1. Player Experience (~700 words)
Outline and justify how your level design facilitates the core player experience goals outlined in the assignment spec. Each section should be supported by specific examples and screenshots of your game encounters that highlight design choices made to facilitate that particular experience.

### 1.1. Discovery
What does the player learn? How does your encounter and broader level design facilitate learning in a way that follows good design practice?

The design of this level is focused around the idea of a puzzle game. The majority of this level is based on the use of the Pushable Box item, and how that interacts with the other parts of the game. The player is learning about how to use this item in correlation with the other items all throughout the level, after it's initial introduction in section 1.

![Movable Box Introduction](DocImages/)

 While all of the main mechanics are introduced early on, the player is learning about the mechanics until the end of the level. Every section is built with puzzles involving using the box to get to or unlock the next area. Each area builds on the functions introduced in the previous sections, but don't contradict each other: There is one situation where the rules are changed slightly, however, in the sequence which introduces the doors closing when the box is moved off their corrosponding pressure pad.
 
 ![Closing Door Demonstration](DocImages/)
 ![When the player pushes the box from the first pad to the second, the door in front opens, but the one behind closes.](DocImages/)
 
  This is inconsistent with section 2, where the trigger door stays open if the box is removed, the reason this has not been changed is that it would allow a potential failstate. 
  
  ![Section 2: Door is still open, even though the box is no longer on the pressure pad.](DocImages/)
  
  This should not impact the gameplay, however, and merely seem like an update on the rules, as the closing door is conveyed in a clear sequence, and all doors after this are consistent with the new rule.


### 1.2. Drama
What is the intensity curve? How does your design facilitate increasing yet modulating intensity, with moments of tension and relief? 

The second section involves a more complex platforming sequence than the other sections of the level, and contains the most hazards in the game. The third level is not as dangerous, because this section focuses more on the puzzle of using the boxes. The drama is fairly low in the first section, and gradually ramps up as it leads into the second section, as more enemies and hazards are encountered.

![Section 2: spikes](DocImages/)

 After section 2, there is a moment of relief, and after that the drama is more focused in the puzzle elements of the game rather than the platforming. The intensity in section 3 ramps up with three puzzles, Each one being more complex than the last, starting with more of a demonstration and ending with a fairly complex puzzle. After this, the drama dies down, as the player approaches the end of the level.

### 1.3. Challenge
What are the main challenges? How have you designed and balanced these challenges to control the difficulty curve and keep the player in the flow channel?

The main challenges of this level are intellectual, with some physical challenges involved too. The second section is most challenging in a physical sense, where the player has to navigate a dangerous environment with spitters and spikes while moving the box through to the pressure pad at the end. The player can choose to either approach the spitters aggressively, by attacking them on the way, which would make it harder to stay on the platform, or they can choose to take the damage or attempt to dodge, where it would be easier to stay on the platform, but could require them to sacrifice health in the process.

![Section 2: spitters](DocImages/)

 The third area is primarily focused on the puzzle of unlocking each door. This starts simple, with a demonstration of how the boxes impact the trigger doors, and ramps up to a fairly complex puzzle at the end of this section. The puzzle at the end requires the player to chain multiple actions together, and to think outside the box: The final solution requires them to extrapolate from the system to move the box up onto a platform, using a trigger door as an elevator, before being able to move the final box into place to unlock the door out.

![Section 3: third puzzle](DocImages/)

### 1.4. Exploration
How does your level design facilitate autonomy and invite the player to explore? How do your aesthetic and layout choices create distinct and memorable spaces and/or places?

The nature of the level is fairly linear, with each section leading into the next. however, later sections can be seen before they are able to be entered, and all sections end in the central area. This should encourage the players curiousity, and inspire intrigue in the areas they can't reach yet. This can especially be seen after section one, when the player reaches the main area: The end of section two is seen immediately, and both the entry and exit of section three can be seen, behind trigger doors which the player can't open yet.

![Hole above player at the end of section 1 is the exit to section 2.](DocImages/)
![Door going into section 3.](DocImages/)

 This is important to the player's understanding of the level as well, as can be seen with the end of section 2: There is a switch the player uses to open the door to enter section three, but the player is unable to see the change, since the door is off screen. Since the player has seen doors previously, this tells them to go back and investigate these places, as it would be expected that the switch opened one of these doors.

 ![Section 3 door is now open.](DocImages/)

## 2. Core Gameplay (~400 words)
A section on Core Gameplay, where storyboards are used to outline how you introduce the player to each of the required gameplay elements in the first section of the game. Storyboards should follow the format provided in lectures.

Storyboards can be combined when multiple mechanics are introduced within a single encounter. Each section should include a sentence or two to briefly justify why you chose to introduce the mechanic/s to the player in that sequence.

You should restructure the headings below to match the order they appear in your level.

### 2.1. - 2.2. Acid/Health Pickups
 I wanted to introduce the movable box as a platform in the acid fairly early in the level, so that's why the acid is the first encounter. Since the acid is the first hazard the player encounters, it made sense to give them the health pickup in the same sequence.



### 2.3. - 2.5. Checkpoints/Spikes/Passthrough Platforms
Since this area includes the first acid pit after the beginning of the level, the checkpoint is introduced here. Spikes are used to increase the difficulty, since the player should have a basic understanding of the controls by now, and the passthrough platform is used for the player to access the top area easily.


### 2.6. - 2.7. Chompers/Weapon Pickup (Staff)
The staff is given to the player at the same time as they encounter the first chomper, which is introduced here as an isolated confrontation, as well as encouraging the player to experiment with the staff.


### 2.8. - 2.9. Weapon Pickup (Gun)/ Spitters
The gun is introduced close to the end of the first section, along with the spitter. As with the staff and the chomper, the spitter encourages the player to experiment with the gun, as well as providing an isolated first encounter with the enemy.

### 2.10. Keys/ Single Use Switch/ Trigger Door
The first key is given at the end of the first segment. This section is immediately after the spitter encounter, and shows the player how to toggle the switch, as well as introducing the trigger door, which is used throughout the level constantly. 

### 2.11. Moving Platforms
This section of the level is fairly vertical, so the moving platform here is used to provide a safe way down without the player feeling like they have to take a leap of faith, as well as providing a simple introduction to the mechanics of the platform.




## 3. Spatiotemporal Design
A section on Spatiotemporal Design, which includes your molecule diagram and annotated level maps (one for each main section of your level). These diagrams may be made digitally or by hand, but must not be created from screenshots of your game. The annotated level maps should show the structure you intend to build, included game elements, and the path the player is expected to take through the level. Examples of these diagrams are included in the level design lectures.

No additional words are necessary for this section (any words should only be within your images/diagrams).
 
### 3.1. Molecule Diagram

![Molecule Diagram]()

### 3.2. Level Map – Section 1

![Section 1]()

### 3.3.	Level Map – Section 2

![Section 2]()

### 3.4.	Level Map – Section 3

![Section 3]()

## 4. Iterative Design (~400 words)
Reflect on how iterative design helped to improve your level. Additional prototypes and design artefacts should be included to demonstrate that you followed an iterative design process (e.g. pictures of paper prototypes, early grey-boxed maps, additional storyboards of later gameplay sequences, etc.). You can also use this section to justify design changes made in Unity after you drew your level design maps shown in section 3. 

You should conclude by highlighting a specific example of an encounter, or another aspect of your level design, that could be improved through further iterative design.

This is where my level design could be somewhat lacking, as I did not primarily work with an iterative design format. I did start out by planning out the original structure, up until about section 2.

![My rather pathetic attempt at iterative design.]()

After this point, I mostly improvised, or worked with a plan I had in mind, but not on paper. Essentially, I did prototype as I went inside the level itself, and adjusted as I went to reuse the successful prototypes. I did this simply because using the tilemap system, as was already set up within the project, was far easier and more efficient than using greybox prototyping, and also because as stated before, I could then implement the prototypes which behaved the way I intended into the final level design without having to rebuild them from scratch.

I also had a couple of playtesters test the game. I changed a few mechanics in the level according to their feedback. For instance, An earlier version of the game had the box in section 2, which had been used to unlock the door to the second key, have to be pushed down the hole leading out of section two onto another pressure pad, which unlocked the door into the third section instead of the switch behind the section two door, which instead unlocked a bridge door which blocked the hole. The first playtester said this was rather confusing, as it wasn't as obvious that the bridge had moved, and once the box was on the first pressure pad, his assumption was that it shouldn't be moved after that. After this, this area was changed to be less convoluted and easier to follow.

## Generative AI Use Acknowledgement

Use the below table to indicate any Generative AI or writing assistance tools used in creating your document. Please be honest and thorough in your reporting, as this will allow us to give you the marks you have earnt. Place any drafts or other evidence inside this repository. This form and related evidence do not count to your word count.
An example has been included. Please replace this with any actual tools, and add more as necessary.


### Tool Used: ChatGPT
**Nature of Use** Finding relevant design theory.

**Evidence Attached?** Screenshot of ChatGPT conversation included in the folder "GenAI" in this repo.

**Additional Notes:** I used ChatGPT to try and find some more relevant design theory that I could apply to my game. After googling them, however, I found most of them were inaccurate, and some didn't exist. One theory mentioned, however, was useful, and I've incorporated it into my work.

### Tool Used: Example
**Nature of Use** Example Text

**Evidence Attached?** Example Text

**Additional Notes:** Example Text


