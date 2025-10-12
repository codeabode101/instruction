**Goal:** Today, we will make our game character move up and down!

**Plan:**
*   **Methods:** `character_rect.y += speed`, `character_rect.y -= speed`, `if keys[pygame.K_UP]:`, `if keys[pygame.K_DOWN]:`
*   **Stretch:** `Combining horizontal and vertical movement for diagonal motion`

Let’s make your character move!

*   **`if keys[pygame.K_UP]:`**
    *   Code: `if keys[pygame.K_UP]:`
    *   Metaphor: Pressing Up. Game knows you want to go up.
    *   Result: Your character gets ready to go higher.
    *   Why it helps: Checks if you pressed the Up arrow.

*   **`character_rect.y -= speed`**
    *   Code: `character_rect.y -= speed`
    *   Metaphor: Float up like a balloon.
    *   Result: Your square moves higher on the screen.
    *   Why it helps: Actually moves your character upwards.

*   **`if keys[pygame.K_DOWN]:`**
    *   Code: `if keys[pygame.K_DOWN]:`
    *   Metaphor: Pressing Down. Game knows you want to go down.
    *   Result: Your character gets ready to go lower.
    *   Why it helps: Checks if you pressed the Down arrow.

*   **`character_rect.y += speed`**
    *   Code: `character_rect.y += speed`
    *   Metaphor: Drop down like a heavy rock.
    *   Result: Your square moves lower on the screen.
    *   Why it helps: Actually moves your character downwards.

**Stretch — Diagonal Movement**
*   Code: `if keys[pygame.K_UP] and keys[pygame.K_LEFT]:`
*   Metaphor: Move two ways at once, like a squirrel.
*   Result: Your character moves up and left at the same time.
*   Why it helps: Lets your character move diagonally.

**Your turn!**
1.  Open your `game.py` file.
2.  Before your main game loop, add your character and speed:
    ```python
    character_rect = pygame.Rect(250, 150, 50, 50)
    speed = 5
    ```
3.  Inside your game loop, after `keys = pygame.key.get_pressed()`, add:
    ```python
    if keys[pygame.K_UP]:
        character_rect.y -= speed
    if keys[pygame.K_DOWN]:
        character_rect.y += speed
    ```
4.  Make sure you draw `character_rect` (e.g., `pygame.draw.rect(screen, (255, 0, 0), character_rect)`).
5.  Run your game. Press UP and DOWN. If your red square moves, it worked!

What keys do you press to make your character move up and down?
