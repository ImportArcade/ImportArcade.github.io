# Speed Card Game

![Project Image](image_url)

## Context

My team and I were tasked with replicating the well known card game Speed. The requirements were as follows:
- Two players must connect to the application on a LAN connection to play the game
- The game must update immediately after a valid play by one of the players
- On a win, the players must submit their names to the application, and that data must be sent to a database

## Content

The project allows players to drag and drop the cards in their hand onto the drop piles as if it were a real game.
As the game progresses, the number of cards the players have dwindles until there is one winner that has gotten rid of all their cards.

## Technologies

- Web Sockets (Socket.io)
- Drag and Drop (DnD kit)
- React.js
- Node.js
- MongoDB

## Contribution

Since this was a team effort, my contribution to this project was in implementing the Web Sockets. I used socket.io to receive and emit
socket actions to and from each player. I had to make sure that on the drag and drop actions, the sockets would receive the correct card that was placed and send it to the other player and updating the state of the game for both players.