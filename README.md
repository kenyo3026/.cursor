# Cursor AI Rules

This directory contains Cursor AI agent rules and configuration files that define coding standards and development practices for this project.

## Overview

The `.cursor` folder is a Git repository that manages AI agent behavior and coding standards. These rules ensure consistent code generation, commit message formatting, and development workflows across the project.

## Rules

### 📝 [git-commit-standards.mdc](./rules/git-commit-standards.mdc)
**Git Commit Message Standards**

Defines strict formatting rules for commit messages:
- **Format**: `[TYPE] Verb description`
- **Types**: FEAT, FIX, DOCS, STYLE, REFACTOR, PERF, TEST, CHORE, REVERT
- **Rules**: English-only, present tense, verb base form
- **Reference**: Actively check past commits when project style is unknown

### 🚀 [incremental-development.mdc](./rules/incremental-development.mdc)
**Incremental Development Approach**

Core principle for code generation:
- **Start Simple**: Implement minimal viable version first
- **Build Incrementally**: Add complexity only when needed
- **Expand Gradually**: Add features in logical steps
- **Environment Setup**: Verify environment before first command execution

### 🌐 [coding-mics.mdc](./rules/coding-mics.mdc)
**Code Language Standards**

English-only policy for all code:
- Comments and documentation in English
- Variable and function names in English
- No non-English characters in code blocks

## Usage

These rules are automatically applied by Cursor AI when:
- Generating new code
- Creating commit messages
- Setting up development environments
- Following incremental development practices

## File Format

All rule files use Markdown format with YAML frontmatter:
```yaml
---
alwaysApply: true/false
description: Brief description of the rule
---
```

## Contributing

When adding or modifying rules:
1. Follow the existing format and structure
2. Keep descriptions concise and clear
3. Use English-only content
4. Test rules with actual AI interactions
5. Update this README when adding new rules

## Repository Structure

```
.cursor/
├── README.md                    # This file
└── rules/
    ├── coding-mics.mdc         # Language standards
    ├── git-commit-standards.mdc # Commit message rules
    └── incremental-development.mdc # Development approach
```

## Best Practices

- **Consistency**: All rules work together to ensure consistent development practices
- **Clarity**: Rules are written to be clear and actionable for AI agents
- **Flexibility**: Rules adapt to project-specific patterns when detected
- **Maintenance**: Regular review and updates based on project evolution
