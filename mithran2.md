Hi team! Today, we will learn how to make our game talk to players and make smart choices.

**Plan for Today:**
*   **Methods:** `Scanner for nextInt()`, `Scanner for nextLine()`, `if-else if-else statements`, `nested if statements`
*   **Stretch:** `String methods like .trim() or .toLowerCase()`

---

*   **Scanner for nextInt()**
    *   `int num = input.nextInt();`
    *   This is like asking "How many?" and waiting for a number from you.
    *   You will type a number, and the computer will save it.
    *   This helps your game get numbers, like how many soldiers to train.

*   **Scanner for nextLine()**
    *   `String word = input.nextLine();`
    *   This is like asking "What is your name?" and waiting for words.
    *   You will type words, and the computer will save them.
    *   This helps your game get words, like a player's name or a command.

*   **if-else if-else statements**
    *   `if (score > 10) { ... } else if (score == 10) { ... } else { ... }`
    *   It's like saying: "If it's sunny, play outside. ELSE IF it's cloudy, read a book. ELSE, watch TV."
    *   Your program will do only one of these actions.
    *   This helps your game pick the right path based on what players do.

*   **nested if statements**
    *   `if (level > 5) { if (coins > 100) { ... } }`
    *   It's like saying: "IF you are big, THEN IF you have money, you can buy a toy."
    *   This lets your game make a choice inside another choice.
    *   This makes your game's choices extra smart.

---

*   **Stretch — String methods like .trim() or .toLowerCase()**
    *   `String cleanWord = word.trim().toLowerCase();`
    *   This is like cleaning up messy writing and making all letters small. " HELLO " becomes "hello".
    *   The words you type will be neat and easy for the computer to understand.
    *   This helps your game understand player commands better, even if they type " Go " or "GO".

---

**Your Turn!**

Let's build a small game piece by piece.
1.  **Start a new file.** Make a new file called `MyGame.java`.
    ```java
    import java.util.Scanner;
    public class MyGame {
        public static void main(String[] args) {
            // We will add more code here!
        }
    }
    ```
2.  **Get a number.** Inside `main`, let's ask for a number.
    ```java
    Scanner input = new Scanner(System.in);
    System.out.println("Type a number (1 or 2):");
    int choice = input.nextInt();
    input.nextLine(); // Fix for nextLine after nextInt
    ```
    *   If you run it now, it will ask for a number and then stop.

3.  **Get some words.** Next, let's ask for a name.
    ```java
    // ... after getting choice
    System.out.println("Type your name:");
    String name = input.nextLine();
    ```
    *   Now it asks for a number, then a name.

4.  **Clean up words (Stretch!).** Make the name neat.
    ```java
    // ... after getting name
    String cleanName = name.trim().toLowerCase();
    ```
    *   Now `cleanName` will be like "hero" even if you typed " HERO ".

5.  **Make choices!** Use `if-else if-else` to react to the number.
    ```java
    // ... after cleanName
    if (choice == 1) {
        System.out.println("You picked option 1.");
        // We will add more inside this if!
    } else if (choice == 2) {
        System.out.println("You picked option 2.");
    } else {
        System.out.println("Not a valid choice.");
    }
    input.close(); // Don't forget this!
    ```
    *   Run it. Type `1` or `2` or something else to see the different messages.

6.  **Add a smart choice (Nested if!).** Inside the `choice == 1` part, check the name.
    ```java
    // ... inside the if (choice == 1) { ... } block
    if (cleanName.equals("hero")) {
        System.out.println("Welcome, Hero!");
    } else {
        System.out.println("Hello, player!");
    }
    ```
    *   Now run it. Type `1` for the number. Then type ` HERO ` (with spaces or big letters) for the name. You should see "You picked option 1. Welcome, Hero!"

Why are choices important in a game?
