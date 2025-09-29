#Spec-kit-use-guide

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## Introduction

GitHub Spec Kit is an open-source toolkit designed for Spec-Driven Development (SDD), helping teams create clear, structured project specifications before coding. It integrates smoothly with AI coding assistants and tools like Windsurf, Gemini CLI, Codex, and GitHub Copilot to streamline project planning and implementation.

---

## Features

- Transform project ideas into detailed specs using `/specify`
- Generate technical plans via `/plan`
- Break plans into actionable tasks with `/tasks`
- AI-assisted code implementation from specs and tasks
- Supports Windsurf, Gemini CLI, Codex, and GitHub Copilot integrations

---

## Getting Started

### Prerequisites

- Git (v2.40+)
- Node.js (v18+ recommended)
- Python 3.10+ (optional, for advanced scripting)
- GitHub account configured with SSH (recommended)

### Installation

Clone the Spec Kit repository locally:
git clone https://github.com/github/spec-kit.git
cd spec-kit
Explore core template files:
ls templates/plan-template.md  spec-template.md  tasks-template.md
---

## Quick Start Guide

Replace `project-name` and `feature-name` accordingly throughout.

1. Initialize a new Spec Kit workspace (if starting fresh):
specify init project-name
2. Create a baseline specification for a feature:
specify /specify feature-name "Brief description of the feature to implement"
3. Generate the technical plan from the specification:
specify /plan feature-name
4. Create implementation tasks based on the plan:
specify /tasks feature-name
---

## Using Windsurf with Spec Kit for Coding

Windsurf enhances your coding by integrating with GitHub Spec Kit to assist in task generation and implementation.

1. **Connect Your GitHub Repository**

Make sure your GitHub repo with Spec Kit is cloned locally.

2. **Open Windsurf Editor**

Launch Windsurf and connect it to your local repository folder.

3. **Run Spec Kit Commands in Windsurf Terminal**

You can run Spec Kit commands inside Windsurf to interactively generate or implement tasks, e.g.:
specify /tasks feature-name
specify /implement feature-name
4. **Leverage AI Code Suggestions**

Use Windsurf’s AI-powered editor to get contextual code suggestions based on Spec Kit tasks and specs for faster development.

5. **Commit and Push Changes**

After implementing, commit your changes and push them back to GitHub to keep your specs and code synchronized.

For more details, watch the [Windsurf GitHub Spec Kit tutorial](https://youtu.be/XGiwp7RlV0c).

---

## Folder Structure

The Spec Kit workspace organizes project files as follows for clarity and version control:
.project-root/
├── .specify/
│   ├── memory/
│   ├── scripts/
│   ├── specs/
│   ├── templates/
├── specs/
├── plans/
├── tasks/
└── source-code/
---

## Useful Links

- [GitHub Spec Kit Repo](https://github.com/github/spec-kit)
- [Spec Kit Documentation & Templates](https://github.github.io/spec-kit/)
- [Windsurf GitHub Connection Tutorial](https://youtu.be/XGiwp7RlV0c)
- [Gemini CLI Discussion on Spec Kit Integration](https://github.com/google-gemini/gemini-cli/discussions/7905)
- [GitHub Copilot Official Site](https://github.com/features/copilot)
- [OpenAI Codex Overview](https://openai.com/index/introducing-upgrades-to-codex/)

---

## Contributing

Contributions to improve Spec Kit or integration documentation are welcome! Please open issues or submit pull requests to the official repository.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Visual Workflow Summary

1. Specify feature → 2. Plan technical design → 3. Generate tasks → 4. Implement with AI tools

All managed via Spec Kit CLI and integrated with AI coding assistants.

---
