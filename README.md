# Klondike(Kata20)

Experiment with different heuristics for playing the solitaire game Klondike.
The solitaire game Klondike is probably the most widely played in the world (particularly if you’re a Window’s user, where it has been available since Windows 3.1). It’s a simple game.

## Game rules
Cards are dealt face down onto the seven piles in the tableau. The first pile receives one card, the next two, up to the seventh pile, which not surprisingly has seven cards initially. The top card on each pile is turned face-up, and the undealt cards are placed on the Stock pile, all face down. Here’s a picture of the game (52kb) if you haven’t seen it before.
The idea is to build up four piles of cards in their suits on the foundation area (one pile for the clubs, one for the diamonds, and so on). The piles must start with the ace and end with the king.

## The available moves (in no particular order) are:

 * If the Stock becomes empty, turn the entire discard pile over and make it the new Stock.
 
 * Turn over the top card of the Stock and place it face-up on the Discard pile.
 
* Move a card from the tableau or discard pile to one of the foundation piles. If the foundation pile is empty, only an Ace can be placed there, otherwise only the next highest card in the appropriate suit can be placed (so if a foundation pile is currently showing a four of hearts, only the five of hearts may be placed there).

 * Move the top card of the discard pile to one of the tableau piles. This card must be one less in rank and opposite in color to the card at the top of the destination tableau.
 
* Move one or more cards from one tableau pile to another. If multiple cards are moved, they must be a sequence ascending in rank and alternating in color. The card moved (or the top of the sequence moved) must be one less in rank and opposite in color to the card at the top of the destination tableau. If the move leaves a face-down card to the top of the original pile, turn it over.

* If a move leaves a tableau pile empty, an exposed King at the top of a tableau or discard pile, or a sequence starting with a King on a tableau pile, may be moved to it.


