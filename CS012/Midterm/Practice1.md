###### Written by Josh Beto

**Problem 1:**

Define a class called `Parser` that represents a parsed sentence.
  * You should store a `vector<string> words` that represents each parsed word in a given sentence
    * i.e. 
    ```cpp
    Parser p("This is a sentence");
    // p should store a vector<string> words as follows:
    // ["This", "is", "a", "sentence"]
    ```
  * You need to implement *functions* that do the following:
    * Prints out each word in the sentence on each line
    ```cpp
    Parser p("This is a sentence");
    p.print();
    /*
    This
    is
    a
    sentence
    */
    ```
    * Returns a word at a given index. Does not change any private variables.
    ```cpp
    Parser p("This is a sentence");
    string s = p.getWord(1);
    cout << s << endl; // prints out 'is'
    ```
    * Changes a word at a given index. Does not return anything.
    ```cpp
    Parser p("This is a sentence");
    p.changeWord(3, "string");
    p.print();
    /*
    This
    is
    a
    string
    */
    ```
    * Filters out parsed words based on a given word
    ```cpp
    Parser p("This is not a sentence");
    p.filter("not");
    p.print();
    /*
    This
    is
    a
    sentence
    */
    ```

  * **Note:** Don't worry about any out of bounds error checking

**Problem 2:**

Define a class 




**Challenge Problem:**

The new upcoming Pokemon game has simplified a great number of battling mechanics. There are now only 3 types in the game: fire, water, grass.
Pokemon now only have one move, attack, which is the same type as the Pokemon and deals the Pokemon's stored `int damage`. As usual, type 
weaknesses and strengths are still supported in the game i.e. fire deals *double* damage to grass but water does *half* damage to grass.
They also removed the ability to switch out Pokemon during battle. Your pokemon team can only store a *max of 6* Pokemon.

Define a class called `PokemonTeam` that represents a Pokemon team in the new games.
  * Stores a max of 6 Pokemon
    * Each Pokemon has the following attributes:
      * name
      * type
      * damage
  * 
  