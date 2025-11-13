# 🐍 Snake Game – Java Project

## 📘 Introduction

This Snake Game is a graphical desktop application developed in Java as part of the Object Oriented Programming (OOP) – 2CS21002 course in my 2nd year.
The project recreates the classic Snake arcade game with smooth motion, keyboard control, and score tracking using Java Swing and AWT for the graphical interface.

The game demonstrates key OOP concepts such as encapsulation, abstraction, and inheritance, while also showcasing real-time event handling and GUI programming skills.

---

## 🎯 Objective

The main objective is to demonstrate **Object-Oriented Programming concepts**—such as **encapsulation**, **abstraction**, **inheritance**, and **polymorphism**—while building an interactive and visually appealing Java application.

The project provides hands-on experience in:

* GUI development with Java Swing
* Event-driven programming using `KeyListener`
* Real-time game loop management using `Timer`
* Collision detection and coordinate-based logic

---

## ⚙️ Technologies and Tools Used

| Component               | Technology/Tool                              |
| ----------------------- | -------------------------------------------- |
| Programming Language    | Java (JDK 17 or higher)                      |
| GUI Framework           | Swing and AWT                                |
| IDE Used                | Visual Studio Code / IntelliJ IDEA / Eclipse |
| Image Handling          | javax.imageio.ImageIO                        |
| Timer and Event Control | java.util.Timer, java.awt.event.KeyAdapter   |

---

## 🧩 Core Classes and Design Overview

### 1. **Main.java**

* Entry point of the program.
* Extends `JFrame` to create the main window.
* Adds the `Game` panel and sets frame size, title, and properties.

### 2. **Game.java**

* The main game logic and rendering component extending `JPanel`.

* Handles:

  * Snake movement
  * Collision detection
  * Food (cherry) spawning
  * Score calculation
  * Game states (RUNNING, PAUSED, GAME_OVER, NOT_STARTED)

* Implements a **game loop** using `TimerTask` to update and repaint the game at fixed intervals.

### 3. **Snake.java**

* Manages snake’s direction, movement, and tail segments.
* Handles:

  * Adding new tail segments when food is eaten.
  * Preventing illegal moves (e.g., turning back on itself).

### 4. **Point.java**

* Represents coordinates of the snake’s head, tail, and cherry.
* Includes helper functions:

  * `move(Direction d, int value)`
  * `intersects(Point p, int tolerance)`
  * `equals(Point p)`

### 5. **Enums:**

* `Direction` – Defines movement direction (UP, DOWN, LEFT, RIGHT).
* `GameStatus` – Represents current game state (NOT_STARTED, RUNNING, PAUSED, GAME_OVER).

---

## 🕹️ Game Controls

| Key                      | Action                       |
| ------------------------ | ---------------------------- |
| **Arrow Keys (↑ ↓ ← →)** | Move Snake                   |
| **P**                    | Pause / Resume Game          |
| **Enter**                | Restart after Game Over      |
| **Any Key**              | Start Game from Title Screen |

---

## 📈 Game Flow

1. **Start Screen:** Displays the title “SNAKE GAME” and waits for any key press.
2. **Running State:** Snake starts moving automatically; player controls direction using arrow keys.
3. **Eating Food:** When the snake eats a cherry, score increments, and the snake grows longer.
4. **Game Over:** Triggered if the snake collides with the wall or itself.
5. **Restart:** Press *Enter* to reset the game and start again.

---

## 🧠 Object-Oriented Concepts Implemented

| Concept           | Implementation                                                          |
| ----------------- | ----------------------------------------------------------------------- |
| **Encapsulation** | Snake’s position and movement logic are contained within its own class. |
| **Abstraction**   | Game status and rendering are separated from the backend logic.         |
| **Inheritance**   | GUI class `Game` inherits `JPanel` to draw and update visuals.          |
| **Polymorphism**  | `KeyAdapter` overrides event methods for user input behavior.           |

---

## 📷 Screenshots 

You can include images like:

##**Start Screen**
<img width="973" height="748" alt="Image" src="https://github.com/user-attachments/assets/54acaac2-6e04-4ff8-b97e-7c56c2d27d87" />
* 
##**Gameplay**
<img width="981" height="751" alt="Image" src="https://github.com/user-attachments/assets/f404d7b6-922c-4eaf-939b-a73422687eff" />
* 
##**Game Over Screen**
<img width="982" height="749" alt="Image" src="https://github.com/user-attachments/assets/9afa7e3e-e0ec-44b3-ae5f-e6b7f815fd55" />
* 


---

## 🚀 How to Run the Project

### Step 1 – Ensure Java 17 is installed

```bash
java -version
javac -version
```

If your default runtime is Java 8 but compiler is Java 17, run using the JDK 17 binary directly:

```bash
& "C:\Program Files\Eclipse Adoptium\jdk-17.0.13.11-hotspot\bin\java.exe" Main
```

### Step 2 – Compile the source

```bash
javac Main.java
```

### Step 3 – Run the game

```bash
java Main
```

---

## 🏗️ Future Improvements

* Add background music and sound effects.
* Implement different difficulty levels (speed increases).
* Include save/load of best score.
* Add menu and instructions screen.

---

## 🏁 Conclusion

This Snake Game project successfully demonstrates core **Object-Oriented Programming** principles through a fun and interactive GUI-based application.
It highlights the effective use of **Swing**, **event handling**, and **timing control**, combining logic and design into a cohesive software model.

---

