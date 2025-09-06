Hi friends! Today we will learn to make a player move in our Pygame Zero game.

### Goal
We will learn how to make our player move around the screen!

### Plan
*   **Methods:** `def update():`, `keyboard.left`, `keyboard.right`, `actor.x, actor.y`, `min() and max()`
*   **Stretch:** `Adding vertical movement using keyboard.up and keyboard.down`

### Let's Learn!

*   `def update():`
    *   Code:
        ```python
        def update():
            print("Time passes!")
        ```
    *   Metaphor: This is like the game's heartbeat, always running.
    *   Result: "Time passes!" will show in the console over and over.
    *   Why it helps: We put all our movement code here so it checks many times a second.

*   `keyboard.left`
    *   Code:
        ```python
        if keyboard.left:
            print("Go left!")
        ```
    *   Metaphor: Like pressing a button.
    *   Result: "Go left!" shows in the console only when you hold the left arrow key.
    *   Why it helps: We use this to know when to move our player left.

*   `keyboard.right`
    *   Code:
        ```python
        if keyboard.right:
            print("Go right!")
        ```
    *   Metaphor: Like pressing another button.
    *   Result: "Go right!" shows in the console when you hold the right arrow key.
    *   Why it helps: We use this to know when to move our player right.

*   `actor.x, actor.y`
    *   Code:
        ```python
        player.x = player.x + 5
        ```
    *   Metaphor: Like telling your toy to slide five steps to the right.
    *   Result: Your `player` character moves right on the screen.
    *   Why it helps: This is how we change your player's spot on the screen.

*   `min() and max()`
    *   Code:
        ```python
        player.x = max(0, min(player.x, WIDTH))
        ```
    *   Metaphor: These are like invisible fences that keep your player inside the screen.
    *   Result: Your player will stop at the edge of the game screen, not go off.
    *   Why it helps: It makes sure your player doesn't disappear!

*   **Stretch — Adding vertical movement using keyboard.up and keyboard.down**
    *   Code:
        ```python
        if keyboard.up:
            player.y = player.y - 5
        if keyboard.down:
            player.y = player.y + 5
        ```
    *   Metaphor: Like using "up" and "down" buttons on a remote control.
    *   Result: Your player moves up when you press `up`, and down when you press `down`.
    *   Why it helps: Now your player can move in all directions!

### Your Turn!
Make a file called `game.py`. Add `WIDTH = 800` and `HEIGHT = 600` at the top. Add `player = Actor('alien')` below that (you need an `alien.png` image in your `images` folder, a blank one is fine for now!). Then, write an `update()` function that uses ALL the methods above to move your player left, right, up, and down, and keep it on screen!

### Final Question
What function runs all the time in Pygame Zero?
