Hello, Future Game Maker!

**Goal:** Learn to make a Pygame window and take basic player input.

**Plan:**
*   **Methods:** `import pygame`, `pygame.init()`, `pygame.display.set_mode`, `pygame.display.set_caption`, `game loop`, `pygame.event.get()`, `event.type == pygame.QUIT`, `pygame.key.get_pressed()`, `pygame.K_SPACE`, `screen.fill`, `pygame.display.flip()`.
*   **Stretch:** Dynamic window title.

**Teach each Method:**
*   `import pygame`
    *   `import pygame`
    *   Opens a game toolbox.
    *   Pygame functions are ready.
    *   Starts building your game.
*   `pygame.init()`
    *   `pygame.init()`
    *   Wakes Pygame up.
    *   Game system is ready.
    *   Prepares your game setup.
*   `pygame.display.set_mode((width, height))`
    *   `screen = pygame.display.set_mode((600, 400))`
    *   Draws your screen size.
    *   A black window appears.
    *   This is your game's main view.
*   `pygame.display.set_caption('Your Game Title')`
    *   `pygame.display.set_caption('My Game')`
    *   Names your window.
    *   "My Game" shows at the top.
    *   Sets your game's title.
*   `game loop (while running:)`
    *   `running = True\nwhile running:`
    *   Game repeats actions fast.
    *   Game runs constantly.
    *   Keeps your game active.
*   `pygame.event.get()`
    *   `for event in pygame.event.get():`
    *   Listens for player actions.
    *   Gets player's clicks or keys.
    *   Allows player interaction.
*   `event.type == pygame.QUIT`
    *   `if event.type == pygame.QUIT: running = False`
    *   Checks for 'X' button click.
    *   The game window closes.
    *   Lets players exit the game.
*   `pygame.key.get_pressed()`
    *   `keys = pygame.key.get_pressed()`
    *   Checks for held keys.
    *   Finds which keyboard keys are down.
    *   Good for continuous player movement.
*   `pygame.K_SPACE`
    *   `if keys[pygame.K_SPACE]: print("Jump!")`
    *   This means the Spacebar key.
    *   An action happens (like jump).
    *   Assigns a key for player action.
*   `screen.fill((R, G, B))`
    *   `screen.fill((255, 0, 0))`
    *   Paints your screen.
    *   Background turns red.
    *   Sets the main scene color.
*   `pygame.display.flip() / .update()`
    *   `pygame.display.flip()`
    *   Shows new drawings.
    *   Changes appear on screen.
    *   Updates the game view for players.

**Stretch — Dynamically changing the window title based on game state**
*   `pygame.display.set_caption(f'Score: {score}')`
*   Changes the window title live.
*   The title shows game state (e.g., score).

**Your turn:**
*   Make a file: `my_game.py`.
*   **1. Window!** Add this code:
    ```python
    import pygame
    pygame.init()
    screen = pygame.display.set_mode((600, 400))
    pygame.display.set_caption('My First Game')
    ```
    Run it! You'll see a black window flash for a second.
*   **2. Keep it!** Add this code after the last part. *Replace* any `pygame.quit()` you might have.
    ```python
    running = True
    while running:
        for event in pygame.event.get():
            if event.type == pygame.QUIT:
                running = False
        screen.fill((0, 150, 250)) # Blue background
        pygame.display.flip()
    pygame.quit()
    ```
    Run it! A blue window stays until you click 'X'.
*   **3. Spacebar!** Before `running = True`, add `score = 0`. Inside the `while running:` loop (before `screen.fill`), add this code:
    ```python
    keys = pygame.key.get_pressed()
    if keys[pygame.K_SPACE]:
        score += 1
        pygame.display.set_caption(f'My First Game - Score: {score}')
    ```
    Run it! Press Spacebar. Watch the score in the title go up!

**Final question:** What does `pygame.init()` do?
