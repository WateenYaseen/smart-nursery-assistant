# Smart Nursery Assistant — Development Rules

**Program:** IEEE WIE JS Mentorship Program 2026  
**Track:** AI & Programming  
**Status:** Project development conventions

## 1. Naming Conventions

- Use clear and descriptive English names for files, variables, functions, and components.
- Use `snake_case` for Python variables and functions.
- Use `PascalCase` for Python classes.
- Use names that explain the purpose of each component.

## 2. File and Folder Structure

- Keep frontend, backend, AI, data, and documentation files organized in their relevant folders.
- Keep documentation in the `docs` folder.
- Avoid placing unrelated functionality in the same file.
- Do not add unnecessary files or dependencies.

## 3. Code Quality

- Prefer simple, readable, and maintainable code.
- Keep functions focused on a clear responsibility.
- Add comments when they explain non-obvious logic or important decisions.
- Avoid unnecessary complexity.
- Review code before considering a feature complete.

## 4. Error Handling

The application should handle common problems, including:
- Missing or invalid images.
- Unsupported plant categories.
- Missing plant records.
- Failed or unavailable AI predictions.
- Missing care information.

Errors should be communicated through clear, useful messages. The system must not replace failed predictions with fabricated results.

## 5. Data and Model Rules

- Check dataset suitability and licensing before using data.
- Keep training, validation, and testing data appropriately separated.
- Reserve local nursery images for independent evaluation when possible.
- Document the model's supported categories and known limitations.
- Do not expose private nursery information or credentials publicly.
- Do not claim performance or accuracy that has not been evaluated.

## 6. AI-Assisted Development Rules

- Explain major proposed changes before applying them.
- Distinguish confirmed decisions from assumptions.
- Review generated code and documentation rather than accepting them automatically.
- Identify weaknesses, missing information, and possible risks.
- Ask the project owner when a requirement or decision is unclear.
- Do not silently change previously agreed requirements.

## 7. Never List

- Never invent project requirements, test results, dataset details, or model performance.
- Never add major features without discussing them with the project owner.
- Never choose an undecided database, framework, model, or deployment platform without explaining the options and trade-offs.
- Never claim an untested feature works.
- Never present image-based water estimates as actual measurements.
- Never expose private data, credentials, or secrets.
- Never remove project limitations or change decisions without making the change clear.

## 8. Decision Rule

**Ask instead of deciding on the project owner's behalf.**

This follows the Session One principle: when information is missing or a decision belongs to the project owner, ask rather than assume.