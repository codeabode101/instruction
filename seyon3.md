Hello, game builders! Today, we learn to make a basic game window and make it listen to your key presses.

**Goal:** Make your game window work and respond to simple commands.

**Plan:**
*   **Methods:** `pygame.init()`, `pygame.display.set_mode((width, height))`, `pygame.display.set_caption('Your Game Title')`, `game loop (while running:)`, `pygame.event.get()`, `event.type == pygame.QUIT`, `pygame.key.get_pressed()`, `pygame.K_q`, `pygame.K_SPACE`, `screen.fill((R, G, B))`, `pygame.display.flip()`
*   **Stretch:** `Dynamically changing the window title based on key presses`

*   `pygame.init()`:
    *   Code: `import pygame; pygame.init()`
    *   Metaphor: Like turning on the main switch for all your toys.
    *   Result: Pygame gets ready. If it worked, you don't see anything yet!
    *   Why it helps: You need this to start any Pygame project.
*   `pygame.display.set_mode((width, height))`:
    *   Code: `screen = pygame.display.set_mode((600, 400))`
    *   Metaphor: Drawing the rectangle for your game screen.
    *   Result: A black window pops up!
    *   Why it helps: This makes your game window.
*   `pygame.display.set_caption('Your Game Title')`:
    *   Code: `pygame.display.set_caption('My Cool Game')`
    *   Metaphor: Writing your game's name on the top of the window.
    *   Result: The window's top bar says "My Cool Game".
    *   Why it helps: Gives your game a name.
*   `game loop (while running:)`:
    *   Code: `running = True; while running:`
    *   Metaphor: The game's heartbeat, always running until you stop it.
    *   Result: Your code inside this loop keeps checking things.
    *   Why it helps: Keeps your game alive and running.
*   `pygame.event.get()`:
    *   Code: `for event in pygame.event.get():`
    *   Metaphor: Checking a mailbox for letters (like key presses or mouse clicks).
    *   Result: Gets a list of things that happened (like a key press).
    *   Why it helps: Finds out what the player is doing.
*   `event.type == pygame.QUIT`:
    *   Code: `if event.type == pygame.QUIT: running = False`
    *   Metaphor: If a "close" button letter arrives, it's time to go home.
    *   Result: Clicking the 'X' on the window closes the game.
    *   Why it helps: Lets players close the game neatly.
*   `pygame.key.get_pressed()`:
    *   Code: `keys = pygame.key.get_pressed()`
    *   Metaphor: Asking "Which keys are *all* being held down right now?"
    *   Result: A list of keys currently pressed.
    *   Why it helps: Lets you know if a key is held down.
*   `pygame.K_q`:
    *   Code: `if keys[pygame.K_q]: running = False`
    *   Metaphor: Looking for the 'Q' key specifically.
    *   Result: If you hold 'Q', the game closes.
    *   Why it helps: A custom key to quit.
*   `pygame.K_SPACE`:
    *   Code: `if keys[pygame.K_SPACE]: print("Space!")`
    *   Metaphor: Looking for the Spacebar specifically.
    *   Result: If you hold Spacebar, a message might show.
    *   Why it helps: Lets you use Spacebar for actions.
*   `screen.fill((R, G, B))`:
    *   Code: `screen.fill((255, 0, 0))`
    *   Metaphor: Painting the whole game screen a new color.
    *   Result: The game background turns bright red.
    *   Why it helps: Changes your game's background color.
*   `pygame.display.flip()`:
    *   Code: `pygame.display.flip()`
    *   Metaphor: Showing your new painting to everyone.
    *   Result: You see all the changes you made on the screen.
    *   Why it helps: Makes your drawing visible to the player.

**Stretch — Dynamically changing the window title based on key presses:**
*   Code: `if keys[pygame.K_SPACE]: pygame.display.set_caption('Space Fun!')`
*   Metaphor: Writing a new title on your game window when you press a key.
*   Result: If you press Space, the window title changes to "Space Fun!".
*   Why it helps: Makes your game title react to player actions.

**Your turn!**
Create a file named `main.py` and write your code there:
```python
# Start your game code here
```
Make a game window that closes if you press 'Q' or the 'X' button, and changes its background color and title when you hold the Spacebar.

What color is your game window when you first open it?
