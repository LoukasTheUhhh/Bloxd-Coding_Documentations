# Bloxd-Coding Documentations
A complete,better and more informative repository for Bloxd's coding api for the server "Bloxd-coding"
It will teach about APIs,statements,definers,callbacks etc.
## APIs
Here's a list of APIs(does not include all,will get updated frequent)
```js
api.sendMessage(myId, "example") //sends a message to the player executing the code.
//@arg(argument) myId -> the player executing the code
//@arg message("example") ->the message being sent
//@arg (optional) {color: " "} -> color of the message
//@arg (optional) {bold: true/false} -> whether the message is bold or not.


api.broadcastMessage("example") //sends a message to everyone in the lobby
//@arg message("example") -> the message being sent
//@arg (optional) {color: " "} -> color of the message
//@arg (optional) {bold: true/false} -> whether the message is bold or not.


api.log/console.log("example") //logs a message(Both api.log and console.log do the same thing)
//@arg message -> the message being logged


api.getHealth(myId) //gets the health of a certain player/entity
//@arg myId -> the person executing the code


api.setHealth(myId, number) //sets a players health to an amount
//@arg myId -> the player executing the code
//@arg number ->(replace with an actual number) the amount of health it was set to
//@arg whoDidDamage(optional) -> I really dont understand this one too lol
//@arg increaseMaxHealthIfNeeded = true/false -> whether the player gets a new maximum health or not


api.forceRespawn(myId, respawnPos[]) //force respawns a player to a certain position
//@arg myId -> the person executing the code
//@arg respawnPos[] -> [x, y, z] -> the coordinates of where the player respawns


api.getEntityName(myId) //Get the name of a entity ingame
//@arg myId -> the person executing the code


api.isPlayerCrouching(myId) //check if the player is crouching or not
//@arg myId -> the person executing the code


api.getPlayerIds() //gets all un-permanent player IDs for every player in the lobby (resets upon leave).
//this API,along with some others,has no arguments needed.


api.getPlayerDbIds() //gets all permanent player IDs for every player in the lobby.
//this API,along with some others,has no arguments needed.
```
IMPORTANT NOTES:     
-myId is always the person executing the code. But,you could also use a playerId instead in "" using api.getPlayerIds() or api.getPlayerDbIds().          
-any argument that has (optional) near it is not needed at all,and sometimes not listed.          
-when using these în world code,any Person that starts the functions will be playerId.        
