#   Project Documentation
##  Requirements Definition
### Functional Requirements
This program is an interactive video game experience where users will move around an open 3D worldspace and interact with objects to collect and view excerpts of the book/lore. It is primarily made to entice and engage people interested in the LOTR book and the epic-fantasy genre as a whole. It can be used to promote the LOTR series to new readers, but is moreso dedicated to people who already know of the series.


-   Movement/Basic User Input
-   Object Interaction + UI

### Use Cases
**Main Menu**

- User will navigate through different menus before engaging in 3D worldspace interactions.
    
    Actors: User
    
    1. The User will open the app and view the main menu.
    2. The user can click to enter the game
    3. The user can open a a settings menu to change volume, resolution, etc.
    4. The user can quit the game.

    Post Conditions: The user is now either playing the game, editing their settings or has closed the program.
        
**Player Movement**

Player will use WASD or Arrow Keys to navigate a game object through a worldspace.

Actors: User

1. The User will press the WASD or arrow keys to move their object (front, left, back, right respectively) relative to the camera position.
2. The camera will be rotated using the mouse to allow users to view different parts of the map, and the cameras rotation will be clamped in specific directions to ensure the program is not disorienting. The playerbody will only follow the rotation on 1 axis.

Postconditions: The user has rotated the camera/playerbody to view other parts of the map and/or has navigated their character around the map.

**Object/Book Interaction**

Player will interact with items in the map by facing the camera towards the objects and interacting with a  key or clicking.

1. The user will approach an interactible object and hover their camera over or around it.
2. The user will interact by clicking or pressing E over the object to open the UI.
3. The book UI will open and display a message/text entry about the books events, characters and other importance pieces of lore.
4. The user can close the book and/or add it to a journal/list of entries to save it.

Postconditions: The user has viewed the journal entry and has learned more about the information and lore of the site, and can review previous pieces of collected information.
**World Boundaries**

Player will be bound to the designed area by a worldborder.

1. The user will enter an area of which there are no entries/areas intended for users to explore.
2. The user will not be allowed to enter these areas through invisible barriers and/or unnavigable terrain.

Postconditions: The user does not enter out-of-bounds areas and is confined to the designed, expected areas.

### Test Cases
1. When the user opens the game and is met with the main menu, they can choose different options to play, edit settings and quit. - (**self-testing.**)
2. When the user moves around the map, the objectives and path, as well as the interactable objects, are marked clearly, and the user explores a clear, linear area. - (**peer-testing.**)


### Non-Functional Requirements
-   Performance - Game uses Unity features to ensure performance and optimisation (baking lighting, choosing not to instantiate and destroy objects, and instead reusing them). Additionally, design cleanliness and readability is sustained using Unity (prefabs, scriptableobjects, etc).

-   Usability - Program is usable for different parties by giving clear instructions on gameplay, dynamic settings, etc.     

-   Reliability

-   Security - Data is saved securely.


---
##  Social, Ethical and Legal Issues

### Social
***Target Audience Considerations*** -
*Who will be using this experience? Are there any accessibility needs?*

- This program will be used for all users with access to a device **(PC)**. It might need interaction tutorials, but should be relatively understandable for most people. keybinds, menu options and UI will be **clearly labelled** to prevent confusion. Book-wise, the book could be difficult to understand without a prior understanding of some of the lore. Thus, it is important that the experience **displays the story clearly**, with **context** provided.



***Potential Benefits*** -
*How does the project positively impact users (e.g., encouraging reading, fostering discussion within the book’s fan community)?*

- This program can positively benefit users by encouraging reading amongst users and promoting interest in the epic-fantasy genre.

***Potential Risks*** - *Could the design exclude or misrepresent certain groups? Are there any themes from the book that might be sensitive to users?*


- A simplified or misinformed representation of the book may cause disagreement between the community. Additionally, the existence of different races, countries and aspects could be sensitive content to some users, and will need to be addressed in the program.

### Ethical

***User Data & Privacy***
*Will the prototype collect user data? If so, how will it be handled responsibly?*

- The prototype likely won't collect significant user data, but may save interactions/logs and data in the program. This should be optimised for users and easy to do.

***Representation & Inclusion***
*Does the project fairly represent characters, themes, or ideas from the book?*

- As the book has characters and themes like race, conflict, and other sensitive topics, it is important it is fairly represented. Characters should be represented faithfully to the source material, and events/places should be explained concisely. This will ensure all users have an understanding of the lore, but can still learn more on their own.

***Content Sensitivity***
*Does the book contain controversial topics (e.g., violence, discrimination), and how will the prototype handle these responsibly?*

- The book contains sensitive topics of racial conflict/discrimination, war and violence, obsessive behaviour/addiction, etc. To ensure all content of this manner is managed in a responsible and considerate way. This could include trigger warnings, context/explanations on the content and/or when it was written to give users and understanding of possible outdated ideas, etc.

### Legal

***Copyright & Intellectual Property:***

*Are any book images, quotes, or fan content being used? If so, are they legally allowed under fair use or with permission?* I will likely use sources from the book, like cover art, quotes, etc. I may use some other sources like a community wiki for extra lore information, which I will have to credit in the program.



*Will you create original assets, or do you need to credit external sources?*

- While some assets may be original, I will likely use some free assets from the Unity asset store. I will credit all external asset sources, and follow terms and regulations applied to them by the creators.

***Terms of Use***

*If you were to launch this product, what legal regulations might apply? Have you investigated terms of use of the product?*

https://www.copyright.org.au/

https://smartcopying.edu.au/

https://creativecommons.org/

PMIs:

|User Interface|Plus|Minus|Implication|
|:---:|:---:|:---:|:---:|
|Spotify|The Spotify UI is efficient for navigating between different pieces of music, lyrics, and more. It allows users to easily create playlists, change volume/output devices, etc.|Some features of the Spotify app (Like jams, Song Radio) are hidden behind tricky/unexplained inputs, like right clicking, difficult-to-distinguish symbols, and more.|It is important that I ensure efficient navigation between key functions of the program, but I must also allow guided/simple navigation to secondary features of the program.|
|Riddle School|Riddle school's UI is a classic point and click, which is simplistic to navigate. It's puzzle based nature allows for an engaging and interactive user experience.|While a point-and-click is simple, the complexity of Riddle Schools puzzle elements can be off-putting and/or inaccessible to some users.|It is important to engage users in the experience with interactions that promote focus on the game, while still being relatively accessible for all users of different states.|




### Riddle School UI
![An image of Riddle School 1.](https://i.ytimg.com/vi/kzOGc5xkGIU/maxresdefault.jpg "Riddle School 1")