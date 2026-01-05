# Trivia

Interactive trivia quiz built with **HTML, CSS, and JavaScript**.  
The page lets users answer one multiple-choice question and one free-response question, with instant visual feedback based on their answers.
![alt text](image.png)

---

## Features

- 🎯 **Multiple choice question**
  - One correct answer, several incorrect options
  - Buttons turn **green** for a correct selection and **red** for an incorrect one
  - Feedback text (`Correct!` / `Incorrect`) appears under the question

- ✍️ **Free-response question**
  - Users type an answer into a text field
  - On submit, the input background turns **green** for a correct answer or **red** for an incorrect one
  - Feedback text appears under the question

- 💡 **DOM manipulation & event handling**
  - Uses JavaScript to:
    - Select elements via `document.querySelector` and `document.querySelectorAll`
    - Attach event listeners to buttons
    - Update styles and text content dynamically

---

## Tech Stack

- **HTML5** – page structure and content
- **CSS3** – layout and visual styling
- **JavaScript (ES6)** – interactivity and DOM manipulation
- *(Optional for local dev)*: `http-server` or any static file server

---

## Getting Started

1. Clone the repository

   ```bash
   git clone https://github.com/<your-username>/trivia.git
   cd trivia

2. Open the page
The simplest option is to just open index.html in your browser:
Double-click index.html, or
Right-click → “Open With” → your preferred browser
Optional (recommended for practice):
Run a lightweight HTTP server from the project directory:
# If you have http-server installed globally (Node.js)
http-server .

# Then visit the printed URL, e.g.
http://localhost:8080

### 🌐 Live Demo

**Live Demo:** https://your-render-domain-here.onrender.com

Project Structure

trivia/
├── index.html
├── style.css
├── README.md
└── screenshots/
    ├── pic1.png
    ├── pic2.png
    ├── pic3.png
    ├── pic4.png
    └── pic5.png

Implementation Details
Multiple-Choice Logic
Each answer button has either a .correct or .incorrect class.
JavaScript selects them using document.querySelectorAll() and attaches click listeners.
Correct answer: button turns green, feedback shows Correct!
Incorrect answer: button turns red, feedback shows Incorrect.
Free-Response Logic
User types into an <input> field and clicks Check Answer.
If the answer matches the expected value ("Switzerland"):
input background turns green
feedback shows Correct!
Otherwise:
input turns red
feedback shows Incorrect.