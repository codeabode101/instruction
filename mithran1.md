**Goal:** Today, we learn to make a basic window for your game!

**Plan:**
*   **Methods:** `JFrame (constructor)`, `setTitle()`, `setSize()`, `setDefaultCloseOperation()`, `setVisible()`
*   **Stretch:** `setLocationRelativeTo(null)`, `JLabel`

*   **JFrame (constructor)**
    *   Code: `JFrame myWindow = new JFrame();`
    *   This is like getting an empty box. (Makes a window object.)
    *   Why it helps: It's the first step!

*   **setTitle()**
    *   Code: `myWindow.setTitle("My Game");`
    *   Like writing "My Game" on your box. (Title bar shows "My Game".)
    *   Why it helps: Tells players your game's name.

*   **setSize()**
    *   Code: `myWindow.setSize(400, 300);`
    *   Like picking how big your box is. (Window is 400 wide, 300 tall.)
    *   Why it helps: Sets your game's screen size.

*   **setDefaultCloseOperation()**
    *   Code: `myWindow.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);`
    *   Like telling the box: "If 'X' is clicked, stop the program!"
    *   Why it helps: Your game closes correctly.

*   **setVisible()**
    *   Code: `myWindow.setVisible(true);`
    *   Like opening your box for all to see! (Window appears on screen.)
    *   Why it helps: Players can see your game.

*   **Stretch — setLocationRelativeTo(null)**
    *   Code: `myWindow.setLocationRelativeTo(null);`
    *   Magic! Your box jumps to the middle of the screen.
    *   Why it helps: Makes your game window neat.

*   **Stretch — JLabel**
    *   Code: `JLabel helloText = new JLabel("Hello!"); myWindow.add(helloText);`
    *   Adds text "Hello!" inside the window. (Like a sticky note.)
    *   Why it helps: Shows messages to players.

**Your turn:**
Make `MyGameApp.java`. Use ALL methods. Title `My Fun App`. Size 500x350. Text `Welcome!`.

**Final question:** What command makes your window appear?
