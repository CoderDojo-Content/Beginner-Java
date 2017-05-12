1. Every Java program needs to start with some special code. For now, let's call them "magic words". I'll explain them in later Sushi Cards. Type this in:

	```java
class Main {
	  public static void main(String[] args) {
		  System.out.println("Hello World!");
	  }
}
  ```  
  
2. Now run the code (click on the **run** button!) and see what happens in the section on the right!
3. That's your first Java program! A lot of that code is those magic words, but the bit inside the second set of curly braces (`{ }`) is what's making it do something. This bit is called the **main method**. The code there now tells Java to print whatever's in the the double quotes (`" "`) to the screen. It's how your game will talk to its player! 
	
	```java
	System.out.println("Hello World!");
	```
4. Notice a couple of things about that line of code: the way the editor highlights different parts (the message text and the command to Java) in different colours. Remove a quote (don't forget to put it back!) and notice how the colours change! Also, notice how the line ends with a semicolon (`;`). That tells Java the line is over. Without it, Java will get really confused!
5. Of course, while "Hello World!" is the classic way to start your first computer program, it's not going to be much use in this game! Change it to "Guess heads (h) or tails (t)!" and run it again to test it. Now you're ready to get the player guessing!

	```java
	System.out.println("Guess heads (h) or tails (t)!");
	```
