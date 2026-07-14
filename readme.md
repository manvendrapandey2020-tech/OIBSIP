# Task 1: Online Reservation System

## 📌 Project Overview
A GUI-based railway reservation system built using Java Swing and JDBC. This application allows users to securely log in, book train tickets, and cancel existing reservations using an auto-generated PNR number.

## 🛠️ Tech Stack
* **Language:** Java
* **GUI Framework:** Java Swing
* **Database:** SQLite
* **Database API:** JDBC

## ✨ Features
1. **Authentication:** Secure login module that denies access to invalid credentials.
2. **Ticket Reservation:** Form validation, auto-population of train names based on train numbers, and dynamic PNR generation using UUID.
3. **Database Integration:** Utilizes `PreparedStatement` to safely insert and delete records, preventing SQL injection.
4. **Ticket Cancellation:** Fetch booking details instantly via PNR and confirm cancellation with a warning dialog.

## 🚀 How to Run
1. Ensure you have the `sqlite-jdbc` JAR file downloaded.
2. Compile the code: `javac -cp ".:sqlite-jdbc-x.x.x.jar" Prabhat_Task1.java` (Use `;` instead of `:` on Windows).
3. Run the application: `java -cp ".:sqlite-jdbc-x.x.x.jar" Prabhat_Task1`
4. **Default Login:** 
   * Username: `admin`
   * Password: `password123`
  


-------------------------------------------------



# Task 2: Number Guessing Game

## 📌 Project Overview
A console-based Java game where the system generates a random number and challenges the user to guess it within a limited number of attempts. The game features difficulty levels, attempt tracking, and a comprehensive scoreboard across multiple rounds.

## 🛠️ Tech Stack
* **Language:** Java
* **Environment:** Console Application
* **Core Concepts:** Loops, Conditionals, Exception Handling, `java.util.Random`, `java.util.Scanner`, `java.util.ArrayList`.

## ✨ Features
1. **Difficulty Levels:** 
   * Easy (1–50, 10 attempts)
   * Medium (1–100, 7 attempts)
   * Hard (1–200, 5 attempts)
2. **Dynamic Feedback:** Guides the user with "Too High!" or "Too Low!" hints after every incorrect guess.
3. **Robust Input Validation:** Prevents the program from crashing if the user enters non-integer text (handled via try-catch).
4. **Session Score Tracking:** Utilizes an `ArrayList` to maintain a history of rounds played, recording the difficulty and how many attempts it took to win.

## 🚀 How to Run
1. Open a terminal or command prompt.
2. Navigate to the directory containing the file.
3. Compile the code: `javac Prabhat_Task2.java`
4. Run the application: `java Prabhat_Task2`




------------------------------------------------------




# Task 3: ATM Interface System

## 📌 Project Overview
A console-based Object-Oriented simulation of an ATM machine. This application allows users to authenticate with a User ID and PIN, check their balance, withdraw and deposit cash, and transfer funds to other registered users. 

## 🛠️ Tech Stack
* **Language:** Java
* **Design Pattern:** Object-Oriented Programming (OOP)
* **Core Concepts:** Encapsulation, Class Interaction, Switch-Case Routing, Collections (`ArrayList`)

## ✨ Features
1. **Multi-Class Architecture:** Built using 5 distinct, modular classes (`ATM`, `Account`, `Transaction`, `Bank`, and `Prabhat_Task3`).
2. **Secure Authentication:** Prompts for User ID and PIN, locking the user out after 3 incorrect login attempts.
3. **Session State:** Dynamically tracks the logged-in user and operates purely on their instantiated `Account` object.
4. **Transaction Log:** Every deposit, withdrawal, and transfer automatically generates a `Transaction` object (stamped with the exact date/time) and is pushed into the user's transaction history.
5. **Logic Validation:** Prevents overdrawing by checking the balance prior to executing withdrawals or transfers.

## 🚀 How to Run
1. Open a terminal or command prompt.
2. Navigate to the directory containing the file.
3. Compile the code: `javac Prabhat_Task3.java`
4. Run the application: `java Prabhat_Task3`
5. **Testing Credentials:** 
   * User 1: ID = `user1`, PIN = `1234`
   * User 2: ID = `user2`, PIN = `5678`
  




--------------------------------





# Task 4: Online Examination System

## 📌 Project Overview
A fully-featured, GUI-based Online Examination System. Candidates can securely log in, update their profile, and take a multiple-choice examination under a strictly timed environment. The system features auto-submission mechanisms and robust session management.

## 🛠️ Tech Stack
* **Language:** Java
* **UI Framework:** Java Swing (`JFrame`, `JPanel`, `JRadioButton`)
* **Layout Management:** `CardLayout` for state transitions

## ✨ Features
1. **State-Driven UI:** Seamlessly swaps between Login, Profile, Exam, and Result screens without launching multiple windows.
2. **Session Management:** Utilizes `WindowListener` to intercept the window close event (`X` button) during an active exam, prompting the user for confirmation to prevent accidental data loss.
3. **Timer Thread:** Implements `javax.swing.Timer` to run a constant countdown (10 minutes) on the UI thread. Automatically submits the exam when the timer hits zero.
4. **State Persistence:** Preserves the candidate's selected answers dynamically as they navigate backward and forward through the test utilizing `Next` and `Previous` event bindings.
5. **Instant Analytics:** Calculates and displays the final score and exact time taken immediately upon submission.

## 🚀 How to Run
1. Open your terminal or command prompt.
2. Navigate to this directory.
3. Compile the code: `javac Prabhat_Task4.java`
4. Run the application: `java Prabhat_Task4`
5. **Default Credentials:** 
   * Username: `admin`
   * Password: `password`
  



--------------------------





# Task 5: Digital Library Management System

## 📌 Project Overview
A web-based library management system built entirely in Java without the need for heavyweight external servers like Tomcat. It implements a local HTTP server to handle REST API requests and serves an interactive HTML/CSS frontend to manage book catalogues and track library members.

## 🛠️ Tech Stack
* **Backend:** Java (`com.sun.net.httpserver`)
* **Database:** SQLite & JDBC
* **Frontend:** HTML, CSS, JavaScript (Fetch API)

## ✨ Features
1. **Self-Contained Web Server:** Bypasses traditional Servlet containers by dynamically routing HTTP contexts using core Java networking libraries.
2. **RESTful API:** Implements JSON-based API endpoints (`/api/books`) to decouple the backend data layer from the frontend rendering logic.
3. **Responsive UI:** Features a modern, styled frontend using CSS and vanilla JavaScript to dynamically populate the library catalogue.
4. **Relational Database Schema:** Maps complex UML multiplicities into SQLite, separating Books, Users, and Issued/Transaction ledgers.
5. **Memory Safety:** Implements strict `try-with-resources` closures across all database calls to prevent memory leaks during API fetch cycles.

## 🚀 How to Run
1. Ensure the `sqlite-jdbc` JAR file is in the same directory.
2. Compile: `javac -cp ".:sqlite-jdbc-x.x.x.jar" Prabhat_Task5.java` (Use `;` instead of `:` on Windows).
3. Run the application: `java -cp ".:sqlite-jdbc-x.x.x.jar" Prabhat_Task5`
4. Look at the terminal for the confirmation message, then open your web browser and navigate to `http://localhost:8080`.




---x----x----x----x----x----
