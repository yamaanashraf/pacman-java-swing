<p align="center">
  <img src="https://i.pinimg.com/originals/b4/ee/c4/b4eec4d093adbe9d8a3cbb40d024836a.png" alt="Pac-Man" width="400">
</p>

# Pacman (Java)

Classic Pac-Man style game built with Java Swing: move around the maze, eat pellets, grab power pellets to turn the tables on ghosts, and aim for a high score.

## How to play

| Action | Keys |
|--------|------|
| Move | **Arrow keys** |
| Alternate move (same keys as **ZQSD** on AZERTY) | **Z** up · **Q** left · **S** down · **D** right |

On a QWERTY keyboard these are still the **Z, Q, S, D** keys (not WASD). Arrow keys work on any layout.

Avoid getting caught by ghosts. Eat **power pellets** (super pellets) to enter fright mode and eat ghosts for extra points.

## Requirements

- **Run the prebuilt JAR:** [Java 16+](https://www.java.com/en/download/) (JRE is enough).
- **Build from source:** [JDK 16+](https://adoptium.net/) (`javac` and `java` on your `PATH`).

## Run the game (release JAR)

1. Open the [**Releases**](https://github.com/lucasvigier/pacman/releases) page for this project.
2. Download the **`.jar`** file attached to a release (the exact filename may vary by release).
3. In a terminal, `cd` to the folder that contains the JAR, then run (replace the name if yours differs):

   ```bash
   java -jar pacman.jar
   ```

   On Windows you can also double-click the JAR if `.jar` files are set to open with Java.

## Build and run from source

Clone or download this repository, then from the **project root** (the directory that contains `src/java` and `src/resources`):

**1. Compile**

Create an `out` directory, then compile.

Linux / macOS:

```bash
mkdir -p out
javac -d out -encoding UTF-8 -sourcepath src/java src/java/game/GameLauncher.java
```

Windows (Command Prompt or PowerShell):

```powershell
mkdir out
javac -d out -encoding UTF-8 -sourcepath src/java src/java/game/GameLauncher.java
```

**2. Run**

Use a classpath that includes both compiled classes and `src/resources` (sprites and level data).

- **Windows:**

  ```powershell
  java -cp "out;src/resources" game.GameLauncher
  ```

- **macOS / Linux:**

  ```bash
  java -cp out:src/resources game.GameLauncher
  ```

The main class is `game.GameLauncher`.

## Project notes

- **UI:** Java Swing (`javax.swing`).
- **Design patterns used in the codebase:** Factory, State, Strategy (ghost behavior), and Observer (score / UI updates).

Upstream repository: [github.com/lucasvigier/pacman](https://github.com/lucasvigier/pacman).

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE).
