Hi friend! Today, we learn to make your game make smart choices based on what players type!

**Plan**

*   **Methods:** `Scanner.next()`, `Scanner.nextLine()`, `String.equals()`, `if-else if-else`, `Logical operators (&&, ||)`
*   **Stretch Methods:** `String.trim()`, `String.toLowerCase()`

---

*   **`Scanner.next()`**
    *   Code: `String word = myScanner.next();`
    *   Metaphor: It's like a tiny grabber for just one word.
    *   Result: If you type "go north", `word` will be "go".
    *   Why it helps: Gets the first command a player types.

*   **`Scanner.nextLine()`**
    *   Code: `String sentence = myScanner.nextLine();`
    *   Metaphor: It's like a long grabber for the whole line you type.
    *   Result: If you type "go north", `sentence` will be "go north".
    *   Why it helps: Gets the full instruction from the player.

*   **`String.equals()`**
    *   Code: `if (playerMove.equals("walk")) { ... }`
    *   Metaphor: It's like matching two Lego bricks to see if they are exactly the same.
    *   Result: The code inside `if` runs only if `playerMove` is "walk".
    *   Why it helps: Checks if a player's command matches a known word.

*   **`if-else if-else`**
    *   Code: `if (score > 10) { ... } else if (score > 5) { ... } else { ... }`
    *   Metaphor: It's like choosing different paths at a park based on signs.
    *   Result: Your game does different actions for different choices.
    *   Why it helps: Makes your game react differently to many player inputs.

*   **`Logical operators (&&, ||)`**
    *   Code: `if (age > 10 && hasKey) { ... }` or `if (rain || snow) { ... }`
    *   Metaphor: `&&` means "and" (both must be true). `||` means "or" (one can be true).
    *   Result: Code runs only when ALL things are true (`&&`) or if AT LEAST ONE thing is true (`||`).
    *   Why it helps: Checks many rules at the same time for complex actions.

---

*   **Stretch — `String.trim()`**
    *   Code: `String cleanInput = dirtyInput.trim();`
    *   Metaphor: It's like wiping dirt (extra spaces) off your shoes.
    *   Result: "  hello " becomes "hello".
    *   Why it helps: Your game understands commands even with extra spaces.

*   **Stretch — `String.toLowerCase()`**
    *   Code: `String smallInput = myInput.toLowerCase();`
    *   Metaphor: It's like turning all big letters into small letters.
    *   Result: "YES" or "Yes" becomes "yes".
    *   Why it helps: Your game understands "go" no matter how the player types it.

---

**Your turn!**
1.  Make a new Java file named `ChoicesGame.java`.
2.  Inside, make a `Scanner` and ask: "What do you want to do (explore/fight/rest)?"
3.  Read the player's full answer using `nextLine()`.
4.  Use `trim()` and `toLowerCase()` on their answer.
5.  Use an `if-else if-else` with `equals()` to check if they typed "explore", "fight", or "rest".
6.  For "explore", use `&&` to also check if they have "torch" (pretend `boolean hasTorch = true;`).
7.  Print what the game does for each choice!

What did you learn about making choices in code?
