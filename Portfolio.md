# Identifying and defining

### **Problem Need**

| Need | Problem Statement | Skill development |
| :--- | ---: | :--: |
| To promote mindfulness, relaxation and emotional wellbeing though a peaceful exploration based open world game, fostering creativity and stress relief. | Stress is a prominent issue around the world, and can impact mental health, physical health and an individual's daily life. A low pressure adventure game available to all ages can help players relax whilst having fun, reducing feelings of stress and rush. | To develop the skills in Unity required to create the game, I would use this series of online tutorials as a scaffold, and further customise the graphics using free libraries or custom models. [3D open world game tutorial ](https://youtu.be/rkk0rs62_qw?si=GISH8RSPHktLDAVk) [, 3D model in Unity tutorial](https://www.youtube.com/watch?v=4Am9E36-7HM)|
| To improve hand-eye coordination, reaction speed and motor skills in young children through an interactive game that is both rewarding and supports quick-decision making. | Young children often struggle to develop strong hand-eye coordination and quick reaction times, while traditional exercises feel too repetitive and fail to hold their attention. With a fun, low investment rhythm game, children are able to actively engage in their motor skills, keeping them entertained through music and interactive gameplay. | To develop the skills in Unity required to create the game, I would use this series of online tutorials as a scaffold, and further customise the graphics with piskel. [Rhythm game tutorial ](https://youtu.be/cZzf1FQQFA0?si=dl_ITgFcWEwOiffK) |
| To refine motor skills and typing proficiency with a lyric typing game that is entertaining and low-investment. | It is estimated that around 80% of the world cannot efefectively touch type, which could be inconvenient in an increasingly digital world. With a lyric typing game, players are able to hone their skills with their favourite songs, maintaining motivation and allowing typing practice to feel more like a game rather than a chore. | To develop the skills in Unity required to create the game, I would use this series of online tutorials as a scaffold, and further customise the graphics with piskel. [Typing game tutorial ](https://youtu.be/j98a_X9G1fM?si=JipPHYkUpvXuaEr2) |
| To develop and enhance the visual memory and concentration of young children.| Young children often have a hard time concentrating and paying attention to detail. A memory game can help by providing interactive challenges that gradually build their visual memory and attention span in a creative way. | To develop the skills in Unity required to create the game, I would use this series of online tutorials as a scaffold and further customise the graphics. [Memory game tutorial ](https://youtu.be/HajiNmv4UNY?si=eIt6dvlivzPd5tDu) |

### **CHOSEN GAME: RHYTHM GAME "TEMPOTAIL"** 

---

### **Requirements outline:**

**Inputs**:  
The game will use arrow keys as the primary user input for hitting notes during gameplay, while mouse clicks will be utilised for navigate the main interface, including the splash screen, settings, tutorial and other menu options. 

**Processing**:  
In gameplay, the system will compare the timing of each arrow key pressed to the expected timing of the note. Based on the accuracy, it will count and categorise the result as "Perfect", "Good", "Bad" or "Miss". 
The system will also count the player's combo, representing the number of notes consecutively hit before a "bad" or "Miss". "Bad" or "Miss" notes will reset the combo to zero.

When the game settings (note speed, music) are changed, the output will be adjusted accordingly.

**Outputs**:  
During gameplay, the system will provide real time feedback, presenting the accuracy of each note at the bottom middle of the screen, and combo in the middle right. Upon completion of a song, a summary page will display the total number of each rating category and the user's overall accuracy as a percentage. 

The game settings will appear as bars and change colour when selected. 

Examples:

<img src="results.png" width="200" height="150">
<img src="bars.png" width="150" height="100">

**Storage + Transmission:**    
The game will operate entirely on the user's device and will not require any network communication or multiplayer support. All calculations will be processed locally, and gameplay data will be temporary and reset when the game is restarted. 

Assuming I have time, this may be altered to save the player's highscore and settings.

### **Functional Requirements**:
**User interaction:**

Players will interact in the main gameplay through the arrow keys, which correspond to the four notes displayed on the screen.
The game begins on a splash screen where they can choose to either start or exit the game. Navigation through scenes such as the settings, tutorial and results page will be done entirely using mouse clicks. Within the settings, players can adjust chart speed and volume, each option represented by four selectable bars of varying intensities. 

**Core gameplay**:  
During gameplay, the player will press the designated arrow key in rhythm with the background music as notes fall towards the target zone at the bottom of the screen. The goal is to press the correct key when the note perfectly aligns with the target zone. The system will compare the accuracy of the player's timing and assign an accuracy rating of "Perfect", "Good", "Bad" or "Miss". The more perfect notes hit, the higher their overall accuracy is when displayed in the results page, which then exits back to the main menu.

A completed round with no "Bad" or "Miss" notes will result in a full combo.

The chart will have a three second intro before beginning.

**Scoring or feedback**:  
When a song is completed, the results page will pop up, showing the player's overall accuracy as a percentage and the number of notes rated as "Perfect", "Good", "Bad", or "Miss", allowing them to reflect on their performance and track improvement over time. During gameplay, the system will also provide real time feedback on each note's accuracy and player combo to maintain their engagement.

### **Non-Functional Requirements**:
**Performance requirements**:   
The system should run smoothly on the player's device with almost immediate response (1-2 seconds). Falling notes, audio and combo/note ratings (should appear under 0.5 seconds after note is pressed) must not lag and should occur in real time to ensure exactness.
The graphics should be high quality and appear exactly as drawn.

**Usability requirements**:  
The game should be simple for all players to understand and navigate, with clear, distinct buttons and easy to read text.
There will also be a tutorial page that can be opened in the corner of the splash screen with annotated images on core mechanics, controls and scoring system for first time users.

**Scalability requirements**:  
If I choose to add more content, there should be lag calibration, a pause button activated with double shift during gameplay (exit/ retry), new songs, difficulty levels for each chart, or note skins that serve as player rewards.
The system must be able to handle the increased content while the performance remains consistent and unaffected.


### **Consideration of social and ethical issues**: 
**Equity:**   
Equity is when everyone is given fair access to opportunities and resources, while acknowledging that different people - whether due to their circumstances, background or abilities, may need different levels of support to achieve a similar outcome.

**Accessibility**:  
Accessibility is the practice of ensuring that products, services and environments are easily used and understood by everyone in order to remove social barriers that might prevent fair participation.

Although my game currently focuses on a single chart, it may not be suitable for players of all skill levels and abilities. To improve accessibility, adjustable settings (mentioned prior) will allow players to customise their experience. The fonts and arrows used will also be simple and easy to read, with high contrast against the background to assist players with visual impairments.
If possible, multiple difficulty levels, translation to different languages and adjustable note sizes could be added for inclusivity later on.

**Privacy and data protection**:  
This version of the game will not permanently collect data, and scores/settings will only exist while the game is running. When the game closes or is restarted, the data is lost.
If a later version saves a player's settings and their high score, it will be done locally with consent and handled securely.

**Fairness and representation**:  
Content within the game, including visuals, text and symbol,s will avoid harmful steryotypes and biases. The characters in the games are cats, which means the designs are neutral and unlikely to misrepresent any groups of players. 
The audio used in gameplay will also be carefully selected to be without any lyrics and instead focus on the game's cute and enjoyable atmosphere while ensuring it remains suitable for all audiences.

**Mental and emotional wellbeing**:  
 Tempotails is designed to provide an appealing and engaging experience, and therefore improbable to affect an individual's mental health, unless it is temporary frustration caused by the difficulty of the chart. 

**Cultural sensitivites**:  
The symbols used in the game will be generic and universal, for example, arrows on the keyboard and the settings logo in the splashscreen's top corner. Text in the tutorial will avoid using slang or words that would confuse international players, using simple and straightfoward language instead. Additionally, the colours should also be pleasant and visually comfortable without cultural connotations that could be misinterpreted.



