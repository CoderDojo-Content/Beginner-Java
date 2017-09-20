1. So, you're asking the player for a guess. How do you tell Java to listen for that guess? You'll need to add a few bits to the code to make it happen. First, you're going to use something called **Scanner** which you'll need to **import**. Importing code is how you tell Java you're going to use something more than the very basics, and lets it load it so it's there when you ask for it. So, add this line at the very start of your code:

   ```java
    import java.util.Scanner;
   ```

2. Next, you need to create a **Scanner** inside your **main method** and give it a label you can use to refer to it later. I picked `user_input` as my label, since I'm going to use the scanner to get user input! Add the following line at the very start of your **main method**:

   ```java
    Scanner user_input = new Scanner(System.in);
   ```

   It tells Java to create a label for a **Scanner** called `user_input` and attach it to a **new Scanner** that looks at **System.in**, which is where things your users type into your program end up! This process of creating the **Scanner** and giving it a label is called **declaring** it. You'll be **declaring** lots of things as you create this game!

3. Now you need to user your **Scanner** to collect and store your player's input! After your print line, where you tell the player to guess, add the following code:

   ```java
    String user_guess = user_input.next();
   ```

   What this does is **declare** a new **String** called `user_guess`, which is a piece of text, and tells **user\_input** to collect the next text the player types and store it in that **String**.

4. Now time to check that you're getting the player's input! Add another line, just after the last one, that prints out what the user typed:

   ```java
    System.out.println("You guessed: "+user_guess);
   ```

   Notice how you can stick two **Strings** together with a `+`. Now, run your code and type in a guess. See what happens!



