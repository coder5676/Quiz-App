# Quiz-App
Quiz App build using React js
# 🎯 React Quiz App

A simple and interactive quiz application built with **React.js**.  
Users can attempt quiz questions, view results, and track their performance in real-time.  
Deployed using **GitHub Pages**.

---

## 🚀 Features
- 📖 Multiple-choice quiz questions
- ⏳ Timer-based questions
- 📝 Tracks selected answers
- 📊 Displays results and score at the end
- ⚡ Fast and responsive UI
- 🌐 Hosted on GitHub Pages

---

## 🛠️ Tech Stack
- **React.js** – UI framework
- **React Router DOM** – Routing (Quiz / Result pages)
- **CSS / Tailwind (if used)** – Styling
- **GitHub Pages** – Deployment
- 
 # The quiz data looks like this

-## 📑 JSON Question Data Example
Questions are stored in a JSON file (`data.json`) like this:

```json
 {
  "About": {
    "topic": "Introduction to Web Development",
    "time":60,
    "questions": [
      {
        "id": 1,
        "question": "What does HTML stand for?",
        "options": [
          "HTML stands for Hyper Text Markup Language, the standard language for creating and structuring content on the World Wide Web.",
          "HTML stands for High Transfer Machine Learning, a machine learning framework used for data science and artificial intelligence.",
          "HTML stands for Home Tool Markup Language, a term used to describe a home design application for interior decorators.",
          "HTML stands for Hyperlinks and Text Markup Language, a tool used only for linking and text formatting on the internet."
        ],
        "correctAnswer": "HTML stands for Hyper Text Markup Language, the standard language for creating and structuring content on the World Wide Web."
      },
      {
        "id": 2,
        "question": "Which language is used for styling web pages?",
        "options": [
          "HTML is mainly used for structuring web content but does not provide advanced styling capabilities for layout or design purposes.",
          "jQuery is a JavaScript library that helps in manipulating HTML elements but it is not used primarily for styling web pages.",
          "CSS, or Cascading Style Sheets, is the language used to style web pages by controlling colors, fonts, layouts, and responsiveness.",
          "XML is a markup language designed to store and transport data but it is not intended for styling web content or interfaces."
        ],
        "correctAnswer": "CSS, or Cascading Style Sheets, is the language used to style web pages by controlling colors, fonts, layouts, and responsiveness."
      },
      {
        "id": 3,
        "question": "Which tag is used to create a hyperlink in HTML?",
        "options": [
          "The <a> tag in HTML defines a hyperlink, allowing users to navigate from one page or resource to another on the web.",
          "The <link> tag is primarily used to define relationships to external resources such as CSS files, not for clickable hyperlinks.",
          "The <href> tag is not a valid HTML element but rather an attribute used inside anchor tags to specify link destinations.",
          "The <hyper> tag does not exist in HTML and therefore cannot be used to define hyperlinks or navigation links on websites."
        ],
        "correctAnswer": "The <a> tag in HTML defines a hyperlink, allowing users to navigate from one page or resource to another on the web."
      },
      {
        "id": 4,
        "question": "Which HTML tag is used to display an image?",
        "options": [
          "The <img> tag is the correct HTML element used to display images on web pages by specifying the image source with the src attribute.",
          "The <image> tag might sound correct but it is not a valid HTML tag and will not render images in a browser environment.",
          "The <pic> tag is also not a valid HTML element and cannot be used to embed images into a website or web application.",
          "The <src> tag is not valid as src is actually an attribute used within the <img> element to define the file path of images."
        ],
        "correctAnswer": "The <img> tag is the correct HTML element used to display images on web pages by specifying the image source with the src attribute."
      },
      {
        "id": 5,
        "question": "Which CSS property is used to change text color?",
        "options": [
          "The color property in CSS is specifically used to set the text color of elements, making it essential for web page design and readability.",
          "The text-color property is not valid in CSS, and attempting to use it will not apply any text color styling in web browsers.",
          "The font-color property is also invalid in CSS as the official and correct property name for text coloring is simply color.",
          "The background-color property changes the background shade of an element and does not directly affect the visible color of text."
        ],
        "correctAnswer": "The color property in CSS is specifically used to set the text color of elements, making it essential for web page design and readability."
      },
      {
        "id": 6,
        "question": "In JavaScript, which keyword is used to declare a variable?",
        "options": [
          "The var keyword in JavaScript is traditionally used to declare variables, although newer standards introduced let and const for better scoping.",
          "The int keyword is not used in JavaScript because the language does not require explicit type declarations for variables or primitive values.",
          "The string keyword is not valid for declaring variables in JavaScript, although it represents a data type used within the language.",
          "The declare keyword is not part of standard JavaScript syntax and cannot be used to define or declare variables in normal programs."
        ],
        "correctAnswer": "The var keyword in JavaScript is traditionally used to declare variables, although newer standards introduced let and const for better scoping."
      },
      {
        "id": 7,
        "question": "Which HTML element is used for the largest heading on a web page?",
        "options": [
          "The <h1> element represents the most important heading on a page, typically used as the main title or top-level heading in HTML documents.",
          "The <h6> element is the least important heading tag in HTML, used for subtopics and rarely used as a page’s main heading.",
          "The <heading> element is not a valid HTML element, and using it will not render proper headings or titles on a webpage.",
          "The <head> element is used to contain metadata such as styles, scripts, and titles but not for displaying headings to the user."
        ],
        "correctAnswer": "The <h1> element represents the most important heading on a page, typically used as the main title or top-level heading in HTML documents."
      },
      {
        "id": 8,
        "question": "Which HTML element is used to create an unordered list?",
        "options": [
          "The <ul> tag is used to define an unordered list in HTML, where items are typically displayed with bullet points by default.",
          "The <ol> tag is specifically used to define ordered lists, where items are automatically numbered rather than shown with bullet points.",
          "The <li> element is used inside either ordered or unordered lists to define each individual list item but does not create lists alone.",
          "The <list> element does not exist in HTML and is therefore invalid for creating any type of lists on a web page."
        ],
        "correctAnswer": "The <ul> tag is used to define an unordered list in HTML, where items are typically displayed with bullet points by default."
      },
      {
        "id": 9,
        "question": "Which symbol is used for comments in CSS?",
        "options": [
          "In CSS, comments are written using the /* comment */ syntax, and everything between these markers is ignored by the browser.",
          "Using // comment is common in JavaScript, but CSS does not recognize double slashes for comments and will throw errors instead.",
          "HTML comments use the <!-- comment --> format, but this style is not valid inside CSS stylesheets and cannot be applied.",
          "The # symbol is often used for IDs in CSS selectors but does not work as a valid comment syntax in stylesheets."
        ],
        "correctAnswer": "In CSS, comments are written using the /* comment */ syntax, and everything between these markers is ignored by the browser."
      },
      {
        "id": 10,
        "question": "Which JavaScript operator is used for strict equality comparison?",
        "options": [
          "The === operator in JavaScript checks both value and data type equality, ensuring comparisons are accurate and avoiding unexpected results.",
          "The = operator is used to assign values to variables and is not valid for comparing values in JavaScript expressions or conditions.",
          "The == operator only checks value equality, performing type coercion, which may lead to unexpected or incorrect comparison outcomes.",
          "The != operator is used to check inequality between values but does not perform strict comparison involving both value and type."
        ],
        "correctAnswer": "The === operator in JavaScript checks both value and data type equality, ensuring comparisons are accurate and avoiding unexpected results."
      }
    ]
  }
}


---

