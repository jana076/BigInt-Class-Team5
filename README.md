# BigInt-Class-Team5
A C++ implementation of an arbitrary precision `BigInt` class capable of storing and performing arithmetic on integers that exceed standard 64-bit integer limits (`long long`)
Numbers are stored internally as digit strings with sign tracking and processed digit by digit

## Features Implemented
- **Constructors & Assignment:** Default (`0`), `int64_t`, `std::string`, copy constructor, destructor, and self-assignment-safe `operator=`
- **Arithmetic Operators:** Signed addition (`+`, `+=`), subtraction (`-`, `-=`), long multiplication (`*`, `*=`), integer division (`/` , `/=`) with zero division exception handling, and modulus (`%`, `%=`)
- **Unary & Inc/Dec Operators:** Unary negation (`-x`), unary plus (`+x`), pre/post increment (`++x`, `x++`), and pre/post decrement (`--x`, `x--`)
- **Relational Operators:** Full comparison support (`==`, `!=`, `<`, `<=`, `>`, `>=`)
- **Stream I/O & Helpers:** `std::cout <<`, `std::cin >>`, `toString()`, leading-zero normalization, and negative zero prevention

## Team 5 Members & Task Distribution
- **Jana Mohamed Mahmoud (Team Leader):** Core private helpers (`removeLeadingZeros`, `compareMagnitude`), all constructors, `operator=`, code integration, and test suite verification
- **Mohamed Yasser Mohamed:** Signed addition operators (`+=`, `+`)
- **Mohamed Emad Younis:** Signed subtraction operators (`-=`, `-`) and unary operators (`-x`, `+x`)
- **Candy Hany Fawzy:** Long multiplication operators (`*=`, `*`)
- **Seif Eldin Ahmed Adel:** Integer division (`/`, `/=`) and modulus (`%`, `%=`)
- **Nour Raef Rabie:** Relational operators (`==`, `!=`, `<`, `<=`, `>`, `>=`), increment/decrement (`++`, `--`), `toString()`, and stream operators (`<<`, `>>`)

## Build & Run
Compile the project with C++17 and strict warning flags:

```bash
g++ -std=c++17 -Wall -Wextra main.cpp -o bigint
./bigint
