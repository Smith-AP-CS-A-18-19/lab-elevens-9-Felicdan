# Elevens 9
*Daniel Feliciano*
Follow the instructions provided for Activity 9 in the student lab guide. Complete the necessary methods and ensure that your game is running properly. You may need to run it from the command line to have it recognize the card graphics. Answer the questions below before you push the finalized repo.

## Questions
1. The size of the board is one of the differences between *Elevens* and *Thirteens*. Why is size not an abstract method?

    * Answer- because when you construct the board for what ever game you are playing it askes what size you want

2. Why are there no abstract methods dealing with the selection of the cards to be removed or replaced in the array `cards`?

    * Answer- because each game will require different things for what needs to be removed

3. Another way to create “IS-A” relationships is by implementing interfaces. Suppose that instead of creating an `abstract Board` class, we created the following `Board` interface, and had `ElevensBoard` implement it. Would this new scheme allow the Elevens GUI to call `isLegal` and `anotherPlayIsPossible` polymorphically? Would this alternate design work as well as the `abstract Board` class design? Why or why not?
	```java
	public interface Board {
	    boolean isLegal(List<Integer> selectedCards);
	    boolean anotherPlayIsPossible();
	}
	```

    * Answer- It would effectively be the same thing because for both you have to actually write the code in the "ElevensBoard" class
