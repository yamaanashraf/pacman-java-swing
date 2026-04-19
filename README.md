<p align="center">
  <img src="https://i.pinimg.com/originals/b4/ee/c4/b4eec4d093adbe9d8a3cbb40d024836a.png" alt="Pac-Man" width="400">
</p>

# Pacman (Java)

Classic Pac-Man style game built with Java Swing: move around the maze, eat pellets, grab power pellets to turn the tables on ghosts, and aim for a high score.

## 🔗 Repository

👉 https://github.com/Yamaan-003/pacman-java-swing

---

## 🎮 How to play

| Action | Keys |
|--------|------|
| Move | **Arrow keys** |
| Alternate move (AZERTY style) | **Z** up · **Q** left · **S** down · **D** right |

On a QWERTY keyboard these are still the **Z, Q, S, D** keys (not WASD). Arrow keys work on any layout.

💡 Avoid getting caught by ghosts.  
💡 Eat **power pellets** (super pellets) to enter fright mode and eat ghosts for extra points.

---

## ⚙️ Requirements

- **Run the prebuilt JAR:** [Java 16+](https://www.java.com/en/download/) (JRE is enough)
- **Build from source:** [JDK 16+](https://adoptium.net/) (`javac` and `java` on your `PATH`)

---

## ▶️ Run the game (release JAR)

1. Open your Releases page:  
   👉 https://github.com/Yamaan-003/pacman-java-swing/releases  

2. Download the `.jar` file.

3. Run it:

```bash
java -jar pacman.jar
```

On Windows, you can also double-click the JAR if Java is configured.

---

## 🛠️ Build and run from source

Clone your repository:

```bash
git clone https://github.com/Yamaan-003/pacman-java-swing.git
cd pacman-java-swing
```

### 1. Compile

Linux / macOS:

```bash
mkdir -p out
javac -d out -encoding UTF-8 -sourcepath src/java src/java/game/GameLauncher.java
```

Windows:

```powershell
mkdir out
javac -d out -encoding UTF-8 -sourcepath src/java src/java/game/GameLauncher.java
```

---

### 2. Run

Windows:

```powershell
java -cp "out;src/resources" game.GameLauncher
```

macOS / Linux:

```bash
java -cp out:src/resources game.GameLauncher
`

---

## 📄 License

This project is licensed under the MIT License. See [LICENSE](LICENSE).
