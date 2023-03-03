Assignment-4

Q. Write a menu-driven Java Program for the following: There are 52 cards in a deck, each of which belongs to one of four suits and one of 13 ranks. Represent a deck of cards as an array of Objects (*you may use the Vector class)

Use integers to encode the ranks and suits.
Have suitable default & parameterized constructors.
all data members to have private access.
The class ‘Card’ to have the following methods: createDeck(), printCard(), printDeck (),sameCard(),compareCard(), sortCard(), findCard() which searches through an array or vector of Cards to see whether it contains a certain card, dealCards() function: to print 5 random cards from the existing deck.
A. This program implements a simple deck of cards, with the ability to print the deck, compare cards, sort cards, and deal cards.

The program defines a Card class, which represents a single playing card. Each card has a suit (e.g. hearts, spades, diamonds, clubs) and a rank (e.g. ace, 2, 3, ..., 10, jack, queen, king).

The Deck class manages a deck of cards. It contains two lists: cards, which represents the deck of cards that have not yet been dealt, and dealt, which represents the cards that have been dealt. The createDeck() method initializes the deck by creating one card of each suit and rank, and shuffling the deck. The DealCards() method deals 5 cards at random from the cards list and adds them to the dealt list.

The main() method of the Deck class provides a simple command-line interface to interact with the deck of cards. The user can choose to print the deck, print the dealt cards, compare two cards, find a card in the deck, sort the dealt cards, or deal 5 more cards.

Deck class: This is the main class that contains the main method and implements the user interface. It contains the following methods: createCard: A method that creates a new Card object based on the user input. createDeck: A method that creates a new deck of cards and shuffles it. printDeck: A method that prints all the cards in the deck. printCard: A method that prints all the cards that have been dealt. sameCard: A method that checks whether there are any duplicate cards in the dealt cards. compareCards: A method that compares two cards and prints which one is greater or if they are equal. sortCard: A method that sorts the dealt cards based on their suit and rank. findCard: A method that searches for a card in the deck and returns its index. DealCards: A method that deals five random cards from the deck. Card class: This is a nested class inside the Deck class that represents a playing card. It contains the following methods: getSuit: A method that returns the suit of the card. getRank: A method that returns the rank of the card. isSame: A method that compares two cards and returns true if they have the same suit and rank. compare: A method that compares two cards based on their rank and returns a positive integer if the first card is greater, a negative integer if the second card is greater, and zero if they are equal. toString: A method that returns a string representation of the card, such as "King of Hearts". Scanner class: A standard Java class that reads input from the console.

ArrayList class: A standard Java class that provides a resizable array implementation.

Collections class: A standard Java class that provides utility methods for working with collections, such as sorting and shuffling.

Comparator interface: A standard Java interface that provides a way to compare objects based on a specified order. Overall, the program provides a basic implementation of a deck of cards, but it could be improved in a number of ways. For example, it could allow the user to specify how many cards to deal, or it could check if there are enough cards in the deck before dealing more. It could also implement more advanced features, such as shuffling the deck after a certain number of cards have been dealt.
