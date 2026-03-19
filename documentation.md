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

### Non-Functional Requirements
-   Performance - Game uses Unity features to ensure performance and optimisation (baking lighting, choosing not to instantiate and destroy objects, and instead reusing them). Additionally, design cleanliness and readability is sustained using Unity (prefabs, scriptableobjects, etc).

-   Usability - Program is usable for different parties by giving clear instructions on gameplay, dynamic settings, etc.     

-   Reliability

-   Security - Data is saved securely.