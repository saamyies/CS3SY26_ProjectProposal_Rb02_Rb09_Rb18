# CS3SY26_ProjectProposal by Aline Teresa Mendoza from CS Unit of PSHS


## Project Proposal Template:

### Project Title or Name of the Application	: Lock : Key
 -- (read as "Lock is to Key")
### Section			   	      : Rubidium
### Group Members			    :
ALMADIN, Samantha I, - Rb02
CRUZ, Jhea Eunice V. - Rb09
NER, Arya Isabelle G. - Rb18
### Date (Proposal Date)  : Nov 21, 2026

### Project Description:
In the quiet night of Niš, Serbia, a halting scream broke the stillness. The next moment was a human heart on the asphalt, a body with a hole by its left side of the torso, and blood leaking out of the two items. The body of an honored general, torn apart tragically with no trace of a killer. This was clearly the work of the Key, a famous, yet anonymous serial killer roaming the city of Niš.

The day after the tragic death of General Vailyn Asteroth Sinclair, another folder was slapped onto Detective Ignatius’ desk. “Anothey Key case,” the man passing the folder had said before he left. Detective Ignatius–the player–was in charge of finding the real identity of Key, and has struggled for weeks with the case. Now, after the recent passing of her cousin and the pressure of the law, she is more than motivated to avenge her beloved cousin, General Vailyn, and the many other victims of Key.

“By the honest scales of Lady Justitia, I hereby declare you pay.”

In this text-RPG, you play as Detective Ignatius, tasked to investigate the many serial cases of anonymous killer Key. Your job is to gather evidence, interrogate suspects and their connections, and correctly find the killer. You will be working with a pathologist who did the autopsy on your cousin’s body, Emil Alix Laurent. They will also accompany you in evidence-gathering. All detectives need a partner, after all.

Beginner text-RPGs often rely on static, unchanging dialogue unaffected by the player's choices, use passive storytelling lacking engaging mechanics, and lack proper clue tracking and organization, reducing player engagement and replayability. Our game's system aims to address these issues---providing an interactive, story-driven detective text RPG that features various mechanics, such as:
- A trust system for all characters (NPCs’ behavior and the difficulty of the case depends on this system)
- Court record (witnesses/suspects, evidence record, information on victims)
- Special actions during interrogations (pressing, presenting evidence)
- Options to travel to different locations, talk to characters (sometimes optionally, for extra story points), and examine the scene

Our game targets players who enjoy cracking murder-mysteries with careful observations and logic skills, as well as those who look for story-rich, choice-driven games where the simplest of choices could cost you everything.

While this game focuses more on analytical and critical skills for players who enjoy such things, the game will also have some secret paths and endings the player may achieve according to what dialogue options they pick; just a little treat for players who enjoy stories outside of solving to touch the waters of each character’s story. Be sure to pay attention to every detail in each piece of evidence analytically, objectively, and with the best of your knowledge. We’re counting on you, Detective. 

#### System Features & OOP Design: 
##### Core Management Classes
- Game; describes the central engine, manages player progress
- CourtRecord; an organized database tracking discovered people and clues
- TrustSystem; tracks how much trust a character has in the player, may affect how NPCs respond and reveal to the player

##### Entity Classes
- GameObj; serves as the parent class for interactive objects and characters in the game
- Evidence (inherits from GameObj); represents clues, and items found by the player
- Character (inherits from GameObj); represents NPCs that can be interacted with
- Suspect (inherits from Character); represents persons of interest who may be the killer
- Witness (inherits from Character); non-suspect characters who hold vital information and clues regarding the case

##### Narrative Classes
- Dialogue; lines and topics that are said by the NPCs when interacted with; some may be gated at specific trust levels
- Statement; individual lines said by NPCs during an interrogation; the MC may press characters for more info regarding these statments, or present evidence proving any contradictions in a statement
- Scene; serves as parent class for playable locations in the game
- InvestigationScene (inherits from Scene); locations the player may travel to for clues, or to interact with characters in the area
- InterrogationScene (inherits from Scene); triggers when interrogating and cross-examining a character; contains multiple statements the player may press or contradict
<img width="1069" height="757" alt="image" src="https://github.com/user-attachments/assets/4b3d9711-8856-4848-8ff7-063c9910006b" />


### Goals:
 
 The long-term outcome of our project is to use CS3 Python OOP programming concepts to give players an immersive, story-driven mystery where players must question every move---every message from a person, carefully build trust with witnesses and suspects, and uncover contradictions to solve the mystery.
- Objective 1: Build the core game management classes and system essential for player progress, and storage of any new findings
- Objective 2: Implement interactive exploration system that allows players to inspect items, examine clues, and hold optional conversations with NPCs
- Objective 3: Develop the interrogation and cross-examination mechanics enabling players to investigate a character's statements, press them for more details, and expose contradictions using found evidence
- Objective 4: Add branching dialogue and story-choices only unlockable through specific sequences of events and actions
- Objective 5: Write and add an immersive, thrilling story that captivates players and convinces them to uncover the truth

[Click here for Rubrics and Sample projects](https://docs.google.com/document/d/1xKd1CqK6DcNWS2_oJPBNtY5n3I3Hqiw8FY3W295Iqfk/edit?usp=sharing)
