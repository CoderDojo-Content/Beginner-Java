1. So now you have a random coin, and it lands on either heads \(1\) or tails \(0\) every time the program runs. In order to have it tell the player which way the coin lands, you need to translate those numbers into words. You can do this using **conditional** or `if` statements. Something like “_If_ the coin value is 1 _then_ print 'heads', otherwise print 'tails'”.
2. In Java an `if` statement has a set of brackets after it in which you put your **condition**. Java reads the **condition** and decides if it's **true** or **false**. If it's **true**, it runs the code in the curly braces \(`{ }`\). If it's **false** it skips over that code and runs whatever comes after it.
3. So, to start with, get your code to print out that the coin landed on heads when you get a 1, or tails for a 0 by adding this bit of code after you've got that random `int`:

   ```java
        if (toss == 1) {
            System.out.println("The coin landed on heads.");
        }

        if (toss == 0) {
            System.out.println("The coin landed on tails.");
        }
   ```

   Notice that you use two equals signs `==` to check if the values on either side of them are the same.

4. Now you need to take the user's guess and turn it into a number, so you can compare it to `toss`. You use an **if statement** to check _if_ the user's guess was a _h_ and set a new **variable**, an `int` called `guess_number`, to _1_ if it is. Then do the same for _t_ and _0_. Add this to the end of the code in your **main method**.

   ```java
    int guess_number;
    if (user_guess.equals("h")) {
        guess_number = 1;
    }

    if (user_guess.equals("t")) {
        guess_number = 0;
    }
   ```

   Notice that to compare **Strings** you have to use `name.equals(thing_to_compare_to)`. The thing in brackets can be the label for another **String** or it can just be a **String** of text, like in the example above. Also, notice that `guess_number` is created without giving it a value. While you've been creating and giving values to **variables** at the same time so far, you can do it separately and it's helpful to do so when the value depends on another value. Finally, notice that you only need to use `int` when _creating_ the **variable**.

5. Ok, now it's time to tell the player if they guessed correctly! Check their guess against the toss and tell them if they won or lost! Notice that **not equal** is `!=` in Java.

   ```java
    if (toss == guess_number) { 
        System.out.println("You guessed right!");         
   }

   if (toss != guess_number) {
          System.out.println("You guessed wrong! Game over!");
   }
   ```

   Now play your game! On the next card, you'll see how to keep playing as long as you keep guessing correctly!



