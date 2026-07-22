# AI Assistant Guidelines

## 1. Project Overview
This repository serves as a foundational frontend engineering environment optimized for AI-assisted development. The primary goal is to establish a robust baseline with best practices, allowing human engineers and AI coding assistants to collaborate seamlessly.

## 2. Tech Stack
- **Environment:** Node.js (LTS)
- **Version Control:** Git
- **Recommended IDE/Tooling:** Cursor, Claude Code, or VS Code with GitHub Copilot
- **Ecosystem:** Designed to accommodate React.js frontend applications (future scalability)

## 3. Coding Conventions
- **Naming:** 
  - Use `camelCase` for variables and functions.
  - Use `PascalCase` for React components.
  - Use `kebab-case` for file and directory names.
- **Style:** 
  - Prefer functional programming paradigms.
  - Use ES6+ syntax (const/let, arrow functions, destructuring).
  - Ensure strict TypeScript typing (if TypeScript is introduced).
- **Documentation:**
  - Write self-documenting code with descriptive variable names.
  - Add JSDoc comments for complex logic or public APIs.

## 4. Folder Structure
Maintain a modular, feature-based folder structure as the project grows:
```text
/
├── src/
│   ├── components/  # Reusable UI components
│   ├── hooks/       # Custom React hooks
│   ├── utils/       # Helper functions
│   └── assets/      # Static files (images, icons)
├── docs/            # Project documentation
├── .gitignore
├── CLAUDE.md
├── LICENSE
└── README.md
```

## 5. Git Workflow
- Follow the **Conventional Commits** standard (e.g., `feat:`, `fix:`, `docs:`, `chore:`).
- Keep commits small, atomic, and focused on a single change.
- Branch naming convention: `type/brief-description` (e.g., `feature/ai-integration`, `fix/header-styling`).

## 6. AI Usage Guidelines
- **Context is King:** Always read this `CLAUDE.md` file before proposing major architectural changes.
- **Code Generation:** When generating code, prioritize readability, maintainability, and accessibility (a11y).
- **Explanation:** Briefly explain *why* a particular approach was chosen when solving complex problems.
- **Refactoring:** Suggest refactoring if existing code violates the conventions outlined in this document.

## 7. Best Practices
- Keep dependencies to a minimum. Only introduce new libraries with strong justification.
- Write tests for critical utility functions.
- Avoid committing secrets or environment-specific configuration (use `.env` and ensure it's gitignored).