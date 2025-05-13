# TDD_PokerHands_SDL

> This excercise is mostly copied from the [TDD Katas repository](https://github.com/garora/TDD-Katas).

## Requirement

Business wants to expand into the online gaming market by developing a poker game.  

The first requirement is to develop the functionality to determine a winning hand of poker cards out of two hands hands of cards.
- A poker hand consists of five cards, each card is unique
- A card has a value and a suit
  - Possible values are 2, 3, 4, 5, 6, 7, 8, 9, 10, jack, queen, king, ace
  (denoted 2, 3, 4, 5, 6, 7, 8, 9, T, J, Q, K, A)
  - Possible suits are clubs, diamonds, hearts, or spades
  (denoted C, D, H, and S)
  - The combination of value and suite are donted as for example 3C (3 of clubs) or QH (queen of hearts)
  - The scoring rules for poker hands are listed below
    
 
> This exercise isn't intended to be finished within the given time! Try to focus on the TDD cycle and break down the given problem space into smaller chunks. With the number of possible poker hands (= scoring rules) available, this excercise can be expanded or shrinked to your liking. Pick and focus on just one poker hand at first and then go from there.

### Poker hands and scoring rules

The poker hands below are ordered by the scoring value in ascending order.

#### High card
Hands which do not fit any higher category are
ranked by the value of their highest card. If the highest
cards have the same value, the hands are ranked by the next
highest, and so on.  

#### Pair
2 of the 5 cards in the hand have the same value.
Hands which both contain a pair are ranked by the value of
the cards forming the pair. If these values are the same,
the hands are ranked by the values of the cards not
forming the pair, in decreasing order.  

#### Two pairs
The hand contains 2 different pairs. Hands
which both contain 2 pairs are ranked by the value of
their highest pair. Hands with the same highest pair
are ranked by the value of their other pair. If these
values are the same the hands are ranked by the value
of the remaining card.

#### Three of a kind
Three of the cards in the hand have the
same value. Hands which both contain three of a kind are
ranked by the value of the 3 cards.

#### Straight 
Hand contains 5 cards with consecutive values.
Hands which both contain a straight are ranked by their
highest card.

#### Flush
Hand contains 5 cards of the same suit. Hands which
are both flushes are ranked using the rules for High Card.

#### Full house
3 cards of the same value, with the remaining 2
cards forming a pair. Ranked by the value of the 3 cards.

#### Four of a kind
4 cards with the same value. Ranked by the
value of the 4 cards.

#### Straight flush
5 cards of the same suit with consecutive
values. Ranked by the highest card in the hand.
