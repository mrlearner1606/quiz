# AI Quiz Simulator (Free)

This project is a **web-based AI quiz simulator** designed to replicate the experience of **paid mock tests and exam simulations** used for **competitive exams and professional certifications**.

It supports:
- AI-generated quizzes using Pollinations
- Custom quiz uploads via `.txt` files
- Timer-based exam simulation
- Instant scoring and explanations

This provides a **free alternative** to paid quiz platforms.

---

## Features

- ✅ AI-generated quizzes by topic and difficulty
- 📁 Upload your own quiz files
- ⏱️ Configurable timer (exam-style)
- ✔️ Single-answer and multi-answer questions
- 💡 Instant feedback with explanations
- 📊 Detailed result summary after quiz completion
- 🌐 Runs entirely in the browser

---

## Prerequisite (For AI Quiz Generation)

To generate quizzes using AI, you have **two options**:

### Option 1: BYOP (Bring Your Own Pollen) - Recommended 🌸

The easiest way to use AI quiz generation with **zero setup**:

1. Click **"Connect with Pollinations"** in the app
2. Sign in using your **GitHub account**
3. Authorize the app (default: 10 pollen budget, 30-day expiry)
4. You're ready to generate quizzes!

**Benefits:**
- ✅ No manual API key management
- ✅ Pay only for what you use
- ✅ Secure OAuth flow
- ✅ Keys never exposed in server logs

### Option 2: Manual API Key

If you prefer to manage your own API key:

1. Go to: **https://enter.pollinations.ai**
2. Sign in using your **GitHub account**
3. After login, copy your **API key**
4. Enter it manually in the app

> **Note:** API keys are required **only for AI-generated quizzes**. Upload mode works without any API key.

---

## How to Use

Open the `index.html` file in a browser or access the deployed application.

You can use the app in **two modes**:

---

## Mode 1: AI Generate Quiz

This mode creates quizzes dynamically using AI.

### Steps

1. Select **AI Generate Quiz**
2. **Connect via BYOP** (recommended) or enter your API key manually
3. Enter:
   - Quiz topic (e.g., AWS, Python, SQL)
   - Number of questions
   - Difficulty level (Easy / Medium / Hard)
   - Timer duration (in minutes)
4. Click **Generate Quiz**

### Output

- AI-generated exam-style questions
- Automatic timer start
- Explanation shown after each submission
- Final score and detailed review

---

## Mode 2: Upload Quiz File

This mode allows you to upload a **predefined quiz** using a text file.

### Important Note on Connectivity

- Upload mode **does not require AI or API calls**
- However, since this is a **deployed web application**, it still requires:
  - Internet access to load the application
  - Browser support for file reading

> **Note:** No backend or server-side processing is used.

---

## Quiz File Format (`.txt`)

The quiz file must strictly follow the format below.

```txt
TIMER: 10

QUESTION: What is AWS?
A) A cloud platform
B) A database
C) A website
D) A programming language
TYPE: SINGLE
ANSWER: A
EXPLANATION: AWS is Amazon's cloud computing platform.
===END===

QUESTION: Which are programming languages?
A) Python
B) HTML
C) Java
D) CSS
TYPE: MULTIPLE
ANSWER: A C
EXPLANATION: Python and Java are programming languages. HTML and CSS are markup/styling languages.
===END===
```

### Rules

- `TIMER` appears only once at the top (minutes)
- Each question must include:
  - `QUESTION`
  - Four options (A–D)
  - `TYPE: SINGLE` or `MULTIPLE`
  - `ANSWER:` 
    - **SINGLE** → one option (e.g., `A`)
    - **MULTIPLE** → space-separated options (e.g., `A C`)
  - `EXPLANATION`
- Each question must end with `===END===`

### Starting an Uploaded Quiz

1. Select **Upload Quiz File**
2. Choose a valid `.txt` file
3. Click **Start Quiz**
4. Timer starts immediately

---

## Results and Evaluation

After completing the quiz:

- ✅ Total score is displayed
- 📝 Each question shows:
  - Your answer
  - Correct answer
  - Explanation
- 📈 Performance summary is generated

---

## Use Case

This application is intended for:

- 📚 Competitive exam preparation
- 🎓 Professional certification practice
- 🧪 Self-assessment and mock tests
- ⏰ Simulating real exam conditions

It offers a **free and customizable alternative** to paid quiz platforms.

---

## Security and Privacy

- 🔐 API keys are used only in the browser
- 🚫 No data is stored on a server
- 💻 Uploaded files are processed locally by the browser

---

## License

This project is provided for **educational and personal use**.

---

## Support

If you encounter any issues or have suggestions:

- Report issues via the project repository
- Contribute improvements via pull requests

---

**Enjoy learning with AI Quiz Simulator! 🎯**
