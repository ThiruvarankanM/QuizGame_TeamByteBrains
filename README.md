# QuizGame\_TeamByteBrains

This project is a simple AI-powered quiz game developed by our Team **ByteBrains**. It runs in the terminal and challenges users with multiple-choice questions, providing hints and AI-generated answers to help users learn effectively.

---

## 📌 Overview

The **QuizGame** is a terminal-based interactive quiz designed to test general knowledge. It offers:

* Multiple-choice questions with 4 options each.
* Immediate feedback on answers.
* A manual hint after the first wrong attempt.
* An AI-powered correct answer reveal after the second wrong attempt.

The AI integration uses Google’s Gemini language model to generate helpful feedback, improving user learning without giving away answers too soon.

---

## 🔍 Key Features

* Multiple-choice questions with four options (a, b, c, d)
* Tracks user score throughout the quiz
* Manual hints after the first incorrect answer to guide the player
* AI-generated correct answers after the second incorrect attempt
* Clear and simple console interface
* Built using the Jac programming language
* AI integration using Google Gemini model via API

---

## 🔧 Technologies & Tools Used

* **Jac Language** – The core language used to build and run the quiz logic
* **Google Gemini AI** – Provides AI-generated answer feedback using a cloud API
* **Python** – Used under the hood by Jac for AI API calls
* **Terminal/Console** – User interface for the quiz
* **VS Code** – Recommended editor for development and running Jac scripts

---

## ⚙️ How It Works

1. The game starts with a welcome message and a sequence of questions.
2. Each question is displayed with four answer options (a, b, c, d).
3. The user inputs their choice.
4. If the answer is correct:

   * A “Correct!” message is shown and the score increases.
5. If the answer is incorrect:

   * On the **first incorrect attempt**, the game provides a **manual hint** (a helpful clue related to the question).
   * On the **second incorrect attempt**, the game calls the **AI (Gemini)** to generate and display the **correct answer**.
6. This process repeats for all questions.
7. At the end, the final score and a performance message are displayed.

---

## 🤖 AI Integration Details

* The AI is triggered only on the second incorrect attempt for a question.
* It uses the **Gemini 1.5 Flash** model via Jac’s AI integration feature.
* The correct answer is passed as a prompt to the AI to generate a helpful response like:

  ```
  ✅ Correct answer: a
  ```
* This keeps the game engaging and provides users with intelligent feedback.

---

## 🔑 How to Get Your Gemini API Key

To enable AI features, you must get an API key from Google:

1. Visit [Google MakerSuite](https://makersuite.google.com/app) and sign in.
2. Click your profile picture in the top-right corner, then **API Keys**.
3. Generate a new API key and copy it.
4. Set it as an environment variable in your terminal before running the game:

```bash
export GEMINI_API_KEY="your_api_key_here"
```

(On Windows CMD: `set GEMINI_API_KEY=your_api_key_here`)

---

## 💻 Running the Quiz Game in VS Code

### Prerequisites

* Install [JacLang CLI](https://jaclang.com/docs/getting-started/installation/)
* Python 3.8 or above
* VS Code (recommended) with Jac extension (optional)

### Steps to Run

1. Clone or download the repository:

```bash
https://github.com/ThiruvarankanM/QuizGame_TeamByteBrains
```

2. Set your Gemini API key in your terminal:

```bash
export GEMINI_API_KEY="your_api_key_here"
```

3. Run the quiz:

```bash
jac run quiz_game.jac
```

4. Play the game interactively in the terminal!

---

## 🤝 Contribution

We welcome contributions! Feel free to add new questions, improve AI interaction, or enhance UI. Fork the repo and submit pull requests.

---

## 🛠 Built With

* Jac Language
* Google Gemini AI via API
* Python (for AI API interaction)
* Terminal / Console

---

## 📜 License

This project is licensed under the MIT License.

---

If you want, I can prepare the full markdown file ready for GitHub — just ask!
