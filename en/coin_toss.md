1. Next, you need to actually toss a coin! This is a lot like the last card: you'll need to do some importing and declaring.

   What you're going to use as a "coin" is a random number generator—a piece of code that's in Java already which picks numbers with an equal chance of choosing any number between 0 and some higher number that you tell it. Of course, since a coin only has two sides, you'll be picking between 0 and 1. Start out with the `import` line, just after your previous `import` line:

   ```java
   import java.util.Random;
   ```

2. Now, just like with the `Scanner`, you'll need to create a `Random` you can use. At the start of your **main method** add this line:

   ```java
   Random coin = new Random();
   ```

3. Now you need to actually toss the coin and store that result somewhere! Just like with the **Scanner** you're going to do both of those in one line, like this:

   ```java
   int toss = coin.nextInt(2);
   ```

   Notice a couple of things here:

   * The number that you gave Java is 2. Java includes the lower number \(0\) but not the higher number \(2\) when picking a number, so the numbers between 0 and 2 are 0 and 1.
   * While you put the result from the `Scanner` into a `String`, you store the result from this `Random` in an `int`, which is short for **Integer**. An integer is a whole number, so this `Random` won't ever give you fractions or decimals. You can make one that will if you need to though!

4. Go ahead and print out the result of your coin toss to check it's working. Run the program a few times to see that the number really is random, then delete the line that prints out the result. You'll add something back later, but you want it to say "heads" or "tails" not "1" or "0"!



