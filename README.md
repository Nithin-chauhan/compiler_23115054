# compiler_23115054
Triangle Perimeter TAC Compiler project using Flex, Bison, and C++. 
🔺 Triangle Perimeter TAC Compiler
This project is a simple compiler that takes triangle expressions in the form triangle(a, b, c); and generates:

✅ Three Address Code (TAC)
⚙️ Optimized Code to Compute Perimeter
🖥️ Perimeter Output from Register-Like Flow

Built using Flex and Bison in C++, this compiler shows how source code is broken down, compiled into intermediate code, and executed.

📥 Installation Guide (Windows with MSYS2)
🔧 Step 1: Install MSYS2 Terminal
👉 Download & install MSYS2 from the official site:
🔗 https://www.msys2.org/wiki/MSYS2-installation/
Follow all steps, including environment setup and initialization.

🛠️ Step 2: Install Required Tools
Open MSYS2 terminal and run:

bash
Copy
Edit
pacman -Su                   # Update all packages  
pacman -S base-devel gcc     # Install base tools and compiler  
pacman -S flex bison         # Install Flex and Bison  
pacman -S git                # (Optional) Version control  
🛠 Build Instructions
Make sure flex, bison, and g++ are installed.

To compile the project:

bash
Copy
Edit
make
This will:

Generate lexer and parser files

Compile the entire source

Output an executable: triangle

🚀 How to Use
Run the compiler:

bash
Copy
Edit
./triangle
Enter your triangle expression in this format:

c
Copy
Edit
triangle(3, 4, 5);
✅ Example Output
Section	Output
Input	triangle(3, 4, 5);
Three Address Code	t1 = 3
t2 = 4
t3 = 5
t4 = t1 + t2
t5 = t4 + t3
Perimeter = t5
Final Output	Perimeter value = 12
### 📁 Project Structure
.
├── lexer.l         # Lexer (Flex)

├── parser.y        # Parser + TAC generation (Bison)

├── main.cpp        # Entry point

├── Makefile        # Build script

├── README.md       # You're here!
⚙️ Optimization Potential
Although this compiler does not yet optimize complex arithmetic, it lays the foundation for:

Pattern	Future Optimization Suggestion
a + b + c	Use of accumulator registers
Triangle Inequality	Add validation before computing
if and while	Add control flow parsing
📸 Screenshots
Add screenshots of terminal output or generated TAC here.
![Screenshot 2025-04-06 152554](https://github.com/user-attachments/assets/b9242e17-9bb4-4b7f-b181-c5e6cf7e834f)
### Nithin lavudya

🎓 B.Tech CSE, NIT Raipur

🌐 GitHub: Nithin-chauhan

🔗 LinkedIn: Nithin Lavudya

📜 License
MIT License – Free to use, improve, or extend!

