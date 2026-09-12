# ♟️ Personal Chess System (Java)

A complete console-based Chess system built entirely in Java. This project was developed focusing on Object-Oriented Programming (OOP), layer organization, and exception handling.

## 🎯 About the Project
The game follows a standard board game architecture and implements chess rules such as:
- Basic piece movements and capturing.
- Allowed move validation according to each piece's rules.
- Separation of logical concerns:
  - **Boardgame Layer**: Generic structure for rows, columns, pieces, and the board matrix.
  - **Chess Layer**: The chess game specialization, including the pieces (King, Queen, Rook, Bishop, Knight, Pawn) and match/turn logic.

## 🚀 How to Run

You will need to have [Java (JDK)](https://www.oracle.com/java/technologies/downloads/) installed on your machine.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/nlopesr/personal-chessjava.git
   ```
2. **Navigate to the project directory and compile the files:**
   ```bash
   cd personal-chessjava
   mkdir bin
   javac -d bin $(find ./src -name "*.java") # Linux/Mac
   # On Windows (PowerShell):
   # Get-ChildItem -Recurse -Filter *.java .\src | Select-Object -ExpandProperty FullName | Out-File sources.txt -Encoding UTF8; javac -d bin @sources.txt
   ```
3. **Start the game:**
   ```bash
   java -cp bin application.Program
   ```

## 🛠️ Technologies Used
- **Java SE:** The core language of the entire project.
- **Git:** Code versioning.
- **Advanced OOP:** Inheritance, Polymorphism, Encapsulation, Enumerations, and Custom Exceptions.

## 📖 How to Play
- When the program is started, the initial board is printed to the console.
- Enter the source position (e.g., `e2`) and press Enter.
- Enter the target position (e.g., `e4`) and press Enter.
- The terminal will be cleared, the move will be executed, and the board will be printed again for the next turn.
