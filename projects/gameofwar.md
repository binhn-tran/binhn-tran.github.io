---
layout: project
type: project
image: img/gameofwar_logo.png
title: "Game Of War"
date: 2022-02-01
labels:
  - Javascript
  - Abstract Data Structures
  - JUnit Testing
summary: "I created a game in ICS 211 named Game Of War and this game can be played with 2 players at most."
---

## Rules of the game
The goal of War is to be the first player to win all 52 cards. The deck is divided evenly, with each player receiving 26 cards, dealt one at a time, face down. Anyone may deal first. Each player places their stack of cards face down, in front of them.

Each player turns up a card at the same time and the player with the higher card takes both cards and puts them, face down, on the bottom of his stack.

If the cards are the same rank, it is War. Each player turns up one card face down and one card face up. The player with the higher cards takes both piles (six cards). If the turned-up cards are again the same rank, each player places another card face down and turns another card face up. The player with the higher card takes all 10 cards, and so on.

## Implementation of Code 
In order to create this game of war, you need to create 4 classes: Rank, Suit, Card, and Deck. Rank is an enumeration of the Ranks of cards, TWO through ACE. Suit is an enumeration of the Suits of cards, CLUBS, DIAMONDS, HEARTS, and SPADES. Card represents a single card. Deck represents a deck of cards.

You also need to create another class named GameOfWar that implements the IGameOfWar interface:

public interface IGameOfWar {
  void initializeGame(Deck d);
  boolean playARound();
  Stack<Card> playerOnesCards();
  Stack<Card> playerTwosCards();
  Stack<Card> combineStacks(Stack<Card> top, Stack<Card> bottom);
}

## Explanation of the methods in IGameOfWar interface
The void initializeGame(Deck d) method should deal the cards to player one and player two. Player one and two should have the same number of cards.

The boolean playARound() method should play one round of War. Then update the players’ stacks to reflect the results of the round. This method should return true if any player wins the game.

The Stack<Card> playerOnesCards() method should return player one’s stack of cards.

The Stack<Card> playerTwosCards() method should return player two’s stack of cards.

The Stack<Card> combineStacks(Stack<Card> top, Stack<Card> bottom) method should combine top and bottom creating the return stack. The cards should be in the order top then bottom.

## JUnit Testing
A JUnit Test file will also be used to test the GameOfWar class for correctness.

## Code Repository
[Link to project repository] (https://github.com/binhn-tran/binhn-tran.github.io/tree/main/projects)

To learn more about how this game of war works, here's the link: https://courses.ics.hawaii.edu/ics211s21/morea/090.stacks/experience-H07-war.html
