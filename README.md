# Trivia

Interactive trivia quiz built with **HTML, CSS, and JavaScript**.  
The page lets users answer one multiple-choice question and one free-response question, with instant visual feedback based on their answers.

<img width="1908" height="1504" alt="image" src="https://github.com/user-attachments/assets/616216b7-2240-4fcf-a86b-c15e91ce59f6" />
<img width="1754" height="1462" alt="image" src="https://github.com/user-attachments/assets/49a9bfe4-d76b-419e-9bb2-43f4579a0f88" />
<img width="1754" height="1510" alt="image" src="https://github.com/user-attachments/assets/fa95461b-c8e3-46e2-8887-a385e334f4ac" />
<img width="1750" height="1528" alt="image" src="https://github.com/user-attachments/assets/b54d657f-cb17-4b41-a66a-22ee9ad3e465" />
<img width="1724" height="620" alt="image" src="https://github.com/user-attachments/assets/ef53beb4-eb45-40de-905a-ef6cd41730a7" />
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

1. **Clone the repository**

   ```bash
   git clone https://github.com/<your-username>/trivia.git
   cd trivia
2. **Run locally (easiest way)**
  Open index.html in your browser:
  Double-click index.html, or
  Right-click → Open With → choose your browser
3. **(Optional) Run using a local HTTP server**
  If you have http-server installed globally (Node.js):

    http-server .

Then visit the printed URL, for example:

### 🌐 Live Demo

**Live Demo:** https://your-render-domain-here.onrender.com

Project Structure
    http://localhost:8080

🌐 Live Demo
Live Demo: 
    
    https://your-render-app-here.onrender.com

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
📂 Project Structure
    
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
    

## Implementation Details

### 🧩 Multiple-Choice Logic
- Each answer button has either a `.correct` or `.incorrect` class  
- JavaScript selects all buttons using `document.querySelectorAll()`  
- Click listeners are attached to each button  
- **Correct answer:** button turns **green**, shows `Correct!`  
- **Incorrect answer:** button turns **red**, shows `Incorrect`

---

### ✍️ Free-Response Logic
- User types their answer into an input field  
- Clicking **Check Answer** compares the value  
- **Correct:** input turns **green**, feedback shows `Correct!`  
- **Incorrect:** input turns **red**, feedback shows `Incorrect`
