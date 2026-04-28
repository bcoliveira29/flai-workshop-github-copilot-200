# GitHub Copilot Instructions

## Project Description

This is the **Mergington High School – Computer Science Portal**, an educational website for sharing homework assignments and coding exercises with students. Students can browse, view, and download assignments directly from the portal.

## Project Structure

- [`assignments/`](../assignments/) – One folder per assignment, each containing a `README.md` and `starter-code.py`
- [`templates/`](../templates/) – Reusable templates for new content
- [`assets/`](../assets/) – Website assets including CSS, JavaScript, and images
- [`index.html`](../index.html) – Main portal page; content is dynamically generated from [`config.json`](../config.json)

## Project Guidelines

- Maintain consistent styling across all pages
- Keep file and folder names descriptive and organized

## Educational Standards

When generating content for this project:

- **Learning-focused**: All content should be designed with clear learning objectives and appropriate difficulty levels
- **Student-friendly**: Use clear, encouraging language that motivates students

## Tech Stack

- **Frontend:** Vanilla HTML, CSS, and JavaScript (ES6+ classes, `fetch` API)
- **Backend:** None – static site driven by `config.json`
- **Assignments:** Python (beginner to intermediate level)

## Coding Conventions

### Python

- Target **Python 3.10+**
- Use clear, beginner-friendly code; avoid advanced idioms that introductory students wouldn't recognise
- Prefer `input()` / `print()` for interactive exercises
- Use descriptive variable and function names (snake_case)
- Keep functions small and focused on a single task

### JavaScript

- Use ES6+ syntax (classes, `async/await`, template literals)
- Follow the existing `AssignmentPortal` class pattern in `assets/js/script.js`
- No external libraries or frameworks – keep it vanilla
- Use camelCase for variables and functions

### HTML / CSS

- Keep markup semantic and accessible
- Follow the existing class naming style in `assets/css/styles.css`

## Assignment Files

When adding or editing assignments:

- Keep `starter-code.py` minimal – provide function stubs, not full solutions
- Write `README.md` files at a level appropriate for high-school beginners
- Register the new assignment in `config.json` under the `assignments` array, following the existing schema (id, title, description, path, dueDate, attachments)

## General Guidelines

- Prioritise readability and simplicity over cleverness
- Do not introduce external dependencies without a strong reason
- Keep all explanations and comments concise and student-friendly
