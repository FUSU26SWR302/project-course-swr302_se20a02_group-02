# Reflection

This document contains reflections on the use of AI tools during the project.

## Student: Hồ Thành Trung (DE190928)

### What worked well:
- AI tools (like Antigravity and Copilot) were extremely helpful in generating repetitive SQL queries and boilerplate code for the Backend.
- Using AI to manage Git operations and resolve large file errors (e.g., ignoring 100MB+ JDK and Maven binary files) saved a lot of debugging time.
- Prompting for template generation allowed the team to standardize the AI documentation format very quickly.

### What didn't work well:
- Sometimes AI generated incorrect path structures if the workspace context was not provided clearly.
- AI could not automatically push code when there were large binary files involved, requiring manual intervention to reset commits and update `.gitignore`.

### Key Learnings:
- Always review AI-generated code, especially database scripts (`data-sqlserver.sql`), to ensure it matches the specific business logic of the project (e.g., LuxeWay vehicle rental requirements).
- AI is a powerful assistant for DevOps tasks (like Git version control) but the developer must clearly specify the branch to avoid accidentally pushing to `main`.
