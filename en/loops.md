1. One of the things that makes computers really powerful is that you can get them to run the same code over and over again. Forever, if you really want to. This is done with **loops**, which are pieces of code that run until a certain **condition** isn't true \(if it's never true, the loop will never run!\).
2. You're going to use a `while` loop here, which will do the same task over and over, _while_ some condition is true. In this case, _while_ the player's last guess was right. You're going to need to store a `true` or `false` value that tells you whether that's the case. These are called **boolean** values, and are stored in a **variable** type of the same name. So, up at top of your **main method**, where you're creating all your variables, add one more like this:
   ```java
    boolean user_right = true;
   ```

   The value has to start as **true** or the **loop** you're creating will never run!
3. Now, just after all of the variables at the start of your **main method** are created, add your `while`** loop** like this:

   ```java
    while (user_right) {  

    }
   ```

4. Select all of the code below the loop and drag it _into_ the loop. Try running it. It should keep going forever, whether the player wins or loses \(since you never set `user_right` to false!\) and you'll need to use the stop button to end the program.
5. Breaking out of the loop and ending the program is easy. You just need to add a line to the **if statement** that handles the player guessing incorrectly, like this:
   ```java
   if (toss != guess_number) {
          System.out.println("You guessed wrong! Game over!");
          user_right = false;
   }
   ```
6. That's it! You've got a complete game! Now run it, test it and try to break it! There are a bunch of things you can do as a player that this game can't handle properly! You'll see how to take care of some of them in the Intermediate **Java** Sushi Cards!



