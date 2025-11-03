# 🎓 React Intern Take-Home Assignment

## 🧭 Objective

Build a small React app that:

-   Renders multiple **courses** from JSON (each with topics and subtopics in Markdown or text format).
    
-   Uses **Tailwind CSS** for clean, responsive styling.
    
-   Includes a minimal **admin surface** (read-only users list).
    
-   Deployed publicly (e.g. Vercel or Netlify) and shared via a **public GitHub repo**.
    

---

## ⚙️ Tech Stack

-   **React + Vite** (JavaScript or TypeScript)
    
-   **Tailwind CSS**
    
-   **Markdown renderer** (e.g., `react-markdown`)
    
-   **Client-only** (no backend; localStorage is allowed)
    

---

## 📂 Data Model

The app should load data from JSON files (e.g. `courses.json`). You can find these in the `src` directory.

### Example Course Structure

```json
{
  "title": "Full Stack Web Development Bootcamp",
  "subtitle": "Master frontend and backend development",
  "description": "A complete bootcamp covering HTML, CSS, JavaScript, React, Node.js, databases, and deployment. Build real-world web applications from scratch.",
  "difficulty": "INTERMEDIATE",
  "learningObjectives": [
    "Build responsive websites with HTML and CSS",
    "Create interactive web applications with JavaScript",
    "Develop modern frontends with React",
    "Build RESTful APIs with Node.js and Express",
    "Work with databases and authentication"
  ],
  "coverImageUrl": "https://example.com/images/fullstack-course.jpg",
  "authorId": 1,
  "topics": [
    {
      "title": "Frontend Fundamentals",
      "description": "Learn the basics of HTML, CSS, and responsive design",
      "orderIndex": 1,
      "subtopics": [
        {
          "title": "HTML Basics",
          "content": "Introduction to HTML5 tags, semantic markup, and document structure. Learn how to create well-structured web pages.",
          "orderIndex": 1
        },
        {
          "title": "CSS Styling",
          "content": "Master CSS selectors, box model, flexbox, and grid. Create beautiful responsive layouts.",
          "orderIndex": 2
        },
        {
          "title": "Responsive Design",
          "content": "Learn media queries, mobile-first design, and cross-browser compatibility.",
          "orderIndex": 3
        }
      ]
    },
    {
      "title": "JavaScript Essentials",
      "description": "Master JavaScript fundamentals and modern ES6+ features",
      "orderIndex": 2,
      "subtopics": [
        {
          "title": "Variables and Data Types",
          "content": "Understand JavaScript data types, variables (let, const, var), and type coercion.",
          "orderIndex": 1
        },
        {
          "title": "Functions and Scope",
          "content": "Learn function declarations, expressions, arrow functions, and closure concepts.",
          "orderIndex": 2
        },
        {
          "title": "Async JavaScript",
          "content": "Master promises, async/await, and handling asynchronous operations.",
          "orderIndex": 3
        }
      ]
    },
    {
      "title": "React Development",
      "description": "Build modern web applications with React",
      "orderIndex": 3,
      "subtopics": [
        {
          "title": "React Components",
          "content": "Learn functional components, JSX syntax, and component composition.",
          "orderIndex": 1
        },
        {
          "title": "State Management",
          "content": "Master useState, useEffect, and state management patterns.",
          "orderIndex": 2
        },
        {
          "title": "React Router",
          "content": "Implement client-side routing and navigation in React applications.",
          "orderIndex": 3
        }
      ]
    }
  ]
}
```

---

## ✅ Must-Haves

### 1\. Course Explorer & Renderer

-   Left sidebar: list of **courses** → click to show topics → click to show subtopics.
    
-   Main area: render the selected subtopic’s **content or Markdown**.
    
-   Include **breadcrumbs** (Course → Topic → Subtopic).
    
-   Implement **search/filter** by course or topic title.
    
-   Clean, responsive layout with **Tailwind CSS**.
    

### 2\. Basic Admin Surface

-   “Admin” tab or route that shows a **read-only list of users** (from JSON).
    
-   Show friendly **empty/loading/error** states if data is missing or invalid.
    

### 3\. UX & Accessibility

-   Keyboard navigation and ARIA-friendly labels.
    
-   Clear heading hierarchy in rendered Markdown.
    
-   Graceful empty states (e.g., “No topics yet”).
    

### 4\. Project Hygiene

-   Built with **Vite**.
    
-   Clear folder structure and minimal dependencies.
    
-   **README** should explain:
    
    -   How to run/build/deploy
        
    -   Key design choices
        
    -   Which features are implemented
        

### 5\. Deployment

-   Share a **public GitHub repo** and a **live demo link** (Vercel or Netlify).
    

---

## 🌟 Nice-to-Haves (Implement both if possible)

### A. Progress Tracking

-   Checkbox or toggle to mark a subtopic as completed.
    
-   Persist completion state in **localStorage**.
    
-   Show completion percentage at topic and course levels.
    

### B. Markdown Extras

-   Support **code blocks** with syntax highlighting.
    
-   Support **tables**, **blockquotes**, and **callouts**.
    

---

## 💡 Bonus

> Not required but will earn extra credit if implemented cleanly.

-   **Create/Edit Course (client-only)**
    
    -   Minimal form to add a course with multiple topics and subtopics.
        
    -   Persist to **localStorage**.
        
    -   Include “Reset Data” to restore defaults.
        
-   **Route-based deep links** (URL reflects selected course/topic/subtopic).
    
-   **Import/Export JSON** (download/upload updated data).
    

---

## 📊 Evaluation Rubric

| Criteria | Description |
| --- | --- |
| **Correctness** | Data correctly mapped to UI, Markdown renders properly |
| **Code Quality** | Clear component structure, state management, and readability |
| **Styling & UX** | Clean Tailwind usage, responsive design, good a11y |
| **Data Handling** | Safe JSON reads, error handling, localStorage usage |
| **Polish** | README clarity, deployment reliability, attention to detail |
| **Nice-to-Haves** | Progress tracking & Markdown extras implemented effectively |

---

## 🚀 Submission

-   **Public GitHub repo** with source code.
    
-   **Live deployment link** (Vercel/Netlify).
    
-   Include in the README:
    
    -   Overview of the project
        
    -   Architecture summary (key components/state)
        
    -   Setup instructions
        
    -   Features implemented (mark nice-to-haves)
        
    -   Known issues or improvements
        
