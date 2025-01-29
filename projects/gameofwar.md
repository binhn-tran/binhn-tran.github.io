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

#Rules of the game
The goal of War is to be the first player to win all 52 cards. The deck is divided evenly, with each player receiving 26 cards, dealt one at a time, face down. Anyone may deal first. Each player places their stack of cards face down, in front of them.

Each player turns up a card at the same time and the player with the higher card takes both cards and puts them, face down, on the bottom of his stack.

If the cards are the same rank, it is War. Each player turns up one card face down and one card face up. The player with the higher cards takes both piles (six cards). If the turned-up cards are again the same rank, each player places another card face down and turns another card face up. The player with the higher card takes all 10 cards, and so on.

#Implementation
In order to create this game of war, you need to create 4 classes: Rank, Suit, Card, and Deck. Rank is an enumeration of the Ranks of cards, TWO through ACE. Suit is an enumeration of the Suits of cards, CLUBS, DIAMONDS, HEARTS, and SPADES. Card represents a single card. Deck represents a deck of cards.
