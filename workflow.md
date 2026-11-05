# Development Workflow

**Project:** Smart Nursery Assistant  
**Program:** IEEE WIE JS Mentorship Program 2026  
**Development Team:** Individual Developer  
**Project Duration:** 8 Weeks

---

## 1. Branch Strategy

The project will use Git branches to keep the main version stable and organize development work.

### Main Branch

- `main` will contain the stable and reviewed version of the project.
- Direct commits to `main` should be avoided.
- Only completed and reviewed changes should be merged into `main`.

### Working Branches

Separate branches will be created for different types of work:

| Branch Prefix | Purpose | Example |
|---|---|---|
| `feature/` | Adding a new feature | `feature/plant-identification` |
| `fix/` | Fixing an existing issue | `fix/image-upload` |
| `docs/` | Documentation updates | `docs/update-research` |
| `test/` | Adding or improving tests | `test/plant-classifier` |

Each branch should focus on one logical task to make changes easier to review and maintain.

## 2. Commit Conventions

Commit messages should be short, clear, and describe the actual change.

The following format will be used:

`type: short description`

Supported types:

- `feat:` New functionality.
- `fix:` Bug fixes.
- `docs:` Documentation changes.
- `test:` Test-related changes.
- `refactor:` Code restructuring without changing functionality.
- `chore:` Maintenance and configuration changes.

### Examples

- `docs: add business requirements document`
- `feat: implement plant image upload`
- `feat: add plant identification model`
- `fix: handle unsupported image formats`
- `test: evaluate plant classifier`
- `refactor: organize prediction functions`

Commits should represent meaningful changes rather than unrelated modifications grouped together.

## 3. Pull Request Rules

Pull Requests (PRs) will be used to review changes before merging them into `main`.

Since this is an individual project, the developer will perform a self-review before merging.

Each PR should include:

- A clear title describing the change.
- A short explanation of its purpose.
- The files or features affected.
- Tests or checks performed.
- Known limitations or unresolved issues.

### Review Checklist

Before merging a PR, check that:

- The changes match the intended task.
- No unrelated files or changes are included.
- Existing functionality has not been unintentionally broken.
- Relevant tests have been completed.
- No passwords, API keys, or private information have been included.
- Documentation has been updated when necessary.

Changes should only be merged after the self-review is complete and identified issues have been addressed or documented.

## 4. Development Environments

The project will use separate stages for development, testing, and demonstration.

### Development Environment

- Used for implementing features and experimenting with models.
- Runs locally on the developer's computer.
- May use sample images and development data.
- Changes and experiments should not be treated as validated results.

### Testing Environment

- Used to evaluate functionality and model performance.
- Uses separate validation and testing datasets.
- Includes unseen images and local nursery images reserved for independent evaluation.
- Used to identify errors, limitations, and unsupported cases.

### Demo Environment

- Used for presenting the working prototype during the mentorship program.
- Uses prepared sample images and test cases.
- Should demonstrate only implemented and tested functionality.
- Should not expose private user data or development credentials.

There is no production environment in the current project scope.

## 5. Data and Security Rules

- Dataset sources and licenses must be checked before using their data.
- Training, validation, and testing data must be separated appropriately.
- Images reserved for independent testing must not be used during model training or tuning.
- Personal or private nursery information should not be published in the public repository.
- API keys, passwords, and other secrets must never be committed to GitHub.
- Environment variables and secrets should be stored locally in a `.env` file when required.
- A `.env.example` file may be included with placeholder values, but must not contain actual credentials.

## 6. AI-Assisted Development Rules

AI tools may be used to support development, debugging, documentation, and code review.

However:

- AI-generated code must be reviewed and understood before being used.
- Important technical decisions should be documented.
- Model performance and predictions must be verified through actual testing.
- AI-generated claims about datasets, libraries, and model capabilities must be checked against reliable sources.
- AI tools should not automatically modify or approve important project decisions without the developer's review.

### AI Review Prompt

When requesting a review of a feature or code change, the AI assistant should be asked to:

- Identify missing requirements.
- Find unclear assumptions.
- Point out potential bugs and edge cases.
- Identify security, privacy, or data-handling risks.
- Highlight missing tests and evaluation gaps.

The AI reviewer should identify and explain the problems without rewriting the code or fixing them automatically. The developer will decide how to address the findings.

---

**Workflow Status:** Proposed development workflow for the Smart Nursery Assistant. It may be updated if project requirements or development needs change.