Here’s a README file for your Rust "Guessing Game" project, which you can use for GitHub:

---

# 🕹️ Guessing Game in Rust

This is a simple command-line guessing game built in Rust. The program randomly generates a secret number between 1 and 100, and the user has to guess it. After each guess, the program will tell the user whether their guess was too small, too big, or correct. It uses the `rand` crate for generating random numbers and the `colored` crate for colorful output feedback.

## ✨ Features
- Randomly generates a secret number between 1 and 100.
- User gets feedback on each guess: too small, too big, or correct.
- Colored terminal output: 
  - Red for incorrect guesses.
  - Green for a correct guess.

## 📦 Dependencies

The project uses the following external crates:
- [`rand`](https://crates.io/crates/rand): For random number generation.
- [`colored`](https://crates.io/crates/colored): For colored output in the terminal.

These dependencies will automatically be handled by `Cargo.toml`.

## 🚀 Getting Started

### Prerequisites

- Rust programming language installed on your system. If you don't have Rust installed, you can install it from the [official website](https://www.rust-lang.org/tools/install).

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/guessing_game_rust.git
   cd guessing_game_rust
   ```

2. Build the project using Cargo:
   ```bash
   cargo build
   ```

3. Run the project:
   ```bash
   cargo run
   ```

## 🛠 Usage

After running the program, you'll be prompted to guess a number between 1 and 100. Based on your input, the program will give you feedback. Keep guessing until you find the secret number.

### Example

```bash
$ cargo run
Guess the number!
Please input your guess.
50
You guessed: 50
Too small!
Please input your guess.
75
You guessed: 75
Too big!
Please input your guess.
63
You guessed: 63
You win!
```

## 📄 Code Breakdown

- The secret number is generated using `rand::thread_rng().gen_range(1..=100)` to get a random number between 1 and 100 (inclusive).
- User input is read using `io::stdin()`, and the input is then compared to the secret number.
- The `colored` crate is used to color the output:
  - Red for guesses that are too small or too big.
  - Green when the correct number is guessed.

## 🧰 How to Contribute

Feel free to fork this repository and submit pull requests. Any suggestions or improvements are welcome!

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Enjoy the game and happy guessing! 🎉
