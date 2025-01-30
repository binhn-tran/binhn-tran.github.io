---
layout: project
type: project
image: img/olelo.jpg
title: "'Ōlelo and English Sayings Database"
date: 2015
published: true
labels:
  - Javascript
  - AVL Tree
  - AVL Node
  - Testing
summary: "I created this homework assignment in ICS 311 with my classmate Ellie Ishii, where it stores 'Ōlelo and English sayings."
---

The database stores 'Ōlelo and English sayings, the English translations and explanations. To implement this, my classmate and I used a AVL tree and an AVL node.

## AVL tree class

The AVLTree class efficiently stores and manages Hawaiian sayings. It makes sure that the tree remains balanced during insertions,  searching for members, finding first and last sayings, and finding the predecessors, as well as the successors.

## AVL node class

The AVLNode class provides efficient storage and retrieval of Hawaiian sayings. 

## Saying class

The Saying class represents the Hawaiian words, their English translation, as well as an explanation.

## Main class

The main class creates a SayingsDatabase object to hold all the sayings managed by the AVL tree. Insert sayings using the insert method along with their translations and explanations. Tests functions by printing the first and last sayings in alphabetical order. Checks if a saying exists in the database. Retrieves and prints the predecessor and successor of a saying. Finds sayings that contain a word in the Hawaiian language. Searches for sayings that contain English words as well.

## Sayings Database class

The sayings database class creates an AVL Tree implementation for the Sayings Database. It stores Hawaiian sayings, their English translations, and explanations, supporting operations like insert, search, and finding predecessors/successors alphabetically.


## Here's the code for the sayings database class:
```cpp
package sayingsDatabase;

/**
 * The Saying class represents the Hawaiian words, their English translation,
 * as well as an explanation.
 * 
 * @author Binh Tran and Ellie Ishii
 *
 */
public class Saying {
  private String hawaiianWords; // single string of Hawaiian words in the saying
  private String englishTranslation; // English translation of the saying
  private String sayingExplanation; // explanation of the saying

  // constructor to initialize the Saying object with Hawaiian words, English translation, 
  // and an explanation
  public Saying(String hawaiianWords, String englishTranslation, String sayingExplanation) {
    this.hawaiianWords = hawaiianWords; // assign the Hawaiian words
    this.englishTranslation = englishTranslation; // assign the English translation
    this.sayingExplanation = sayingExplanation; // assign the explanation
  }

  // Overloaded constructor without explanation
  // default explanation is an empty string
  public Saying(String hawaiianWords, String englishTranslation) {
    this(hawaiianWords, englishTranslation, ""); // call the constructor with an empty explanation
  }

  // get the Hawaiian words 
  public String getHawaiianWords() {
    return hawaiianWords;
  }

  // get the English translation
  public String getEnglishTranslation() {
    return englishTranslation;
  }

  // get the explanation
  public String getExplanation() {
    return sayingExplanation;
  }

  // override the toString() method to format the string representation of the Saying object
  @Override
  public String toString() {
    return "Hawaiian: " + hawaiianWords + "\nTranslation: " + englishTranslation + "\nExplanation: "
        + sayingExplanation;
  }

}
```

Link to my repository to view the code for this project[GitHub Repository](https://github.com/binhn-tran/binhn-tran.github.io/tree/main/projects).
