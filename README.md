## **MUD Project**

### **Overview**

Multi-User Dungeons (MUDs) are multiplayer text-driven experiences designed for multiple people to crawl through dungeons together. What it really boils down to is an interactive chatroom experience. These types of games later evolved into MMORPGs once computing power gave rise to more powerful, realistic graphics.

For me, this is an opportunity at tyring to re-create the 80's-90's "MMO" scene as well as learn how to program network communications using nothing but the **C** language.

### **Setting**

After playing around with Metal Gear Solid 5, I thought it'd be kinda neat to have a tactical espionage-type MUD to play around in. Featuring a setting similar to the MGS Universe, dungeons and raids of traditional MUD settings would become mission objectives and warzones. Players could write their own mission scenarios and submit them for review to be integrated into the MUD as well.

---
### **Game Structure**

#### Database
* Custom-made, essentially a large text file to hold character data structures. (Will be sloppy)

#### Server
* Is the middleman between the database and clients.
* Must be able to send/receive data to multiple connections.

#### Client
* Receives/sends data to the server.
* Server writes to database after certain operations have happened in game.
>* Collecting an item.
>* Quitting the game/closing connection
>* Completing a battle with a creature/player
>* Performing an in-game transaction (shops, trade, etc.)
