---
description: "Use when creating, editing, or registering a new assignment. Covers README structure, starter-code conventions, and config.json registration."
applyTo: "assignments/**"
---

# Assignment Authoring Guidelines

## Folder Structure

Each assignment lives in its own subfolder under `assignments/`:

```
assignments/
  <assignment-id>/
    README.md
    starter-code.py
    [optional extra files, e.g. data.csv]
```

Use lowercase, hyphen-separated folder names that match the `id` field in `config.json` (e.g. `python-basics`, `data-analysis`).

## README.md

Follow the template in `templates/assignment-template.md`. Key rules:

- Open with `# 📘 Assignment: <Title>`
- Include a `## 🎯 Objective` section — one or two sentences describing what the student will build or learn
- Break work into named tasks under `## 📝 Tasks`, each with:
  - A `### 🛠️ <Task Title>` heading
  - A **Description** paragraph
  - A **Requirements** bullet list phrased as "Completed program should: …"
  - Example input/output where helpful
- Use clear, encouraging language appropriate for high-school beginners

## starter-code.py

- Provide **function stubs only** — a docstring or comment explaining the task, then `pass`
- Do **not** include solutions or working logic
- Use snake_case for all function and variable names
- Target Python 3.10+; avoid advanced idioms beginners wouldn't recognise

```python
# Task 1
def greet_user():
    # Ask the user for their name
    # Print a personalised greeting
    pass
```

## Registering in config.json

Add an entry to the `assignments` array following this schema:

```json
{
  "id": "assignment-folder-name",
  "title": "Human-Readable Title",
  "description": "One sentence shown on the portal card.",
  "path": "assignments/assignment-folder-name",
  "dueDate": "YYYY-MM-DD",
  "attachments": [
    {
      "name": "Starter Code",
      "file": "starter-code.py",
      "type": "python"
    }
  ]
}
```

- `id` must match the folder name exactly
- `dueDate` uses ISO 8601 format (`YYYY-MM-DD`)
- Only list files in `attachments` that actually exist in the folder
- Additional attachment types used in this project: `"type": "csv"`
