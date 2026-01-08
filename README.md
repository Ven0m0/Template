# GitHub Repository Template

A clean, opinionated GitHub repository template with AI-assisted development tools, automated linting, and workflow configurations.

## Features

- **AI Development Tools**
  - Claude AI instructions (`CLAUDE.md`)
  - GitHub Copilot configuration (`.github/copilot-instructions.md`)
  - Specialized AI agents for bash, Python, Rust, and more
  - Custom prompts for common development tasks

- **Automated Workflows**
  - Unified linting with ShellCheck and Super-Linter
  - Config file validation and auto-fixing
  - Dependabot for dependency updates
  - CI workflow integration

- **Code Quality**
  - EditorConfig for consistent formatting
  - ShellCheck configuration
  - MegaLinter support
  - Git attributes for proper line endings

- **Issue & PR Templates**
  - Bug report template
  - Feature request template
  - Custom issue template
  - Pull request template

## Quick Start

### Using this Template

1. Click "Use this template" button on GitHub
2. Name your new repository
3. Clone your new repository locally
4. Customize the template for your project:
   - Update `CLAUDE.md` with project-specific instructions
   - Modify `.github/copilot-instructions.md` if needed
   - Edit workflows in `.github/workflows/` as required
   - Update issue/PR templates in `.github/ISSUE_TEMPLATE/`

### Repository Structure

```
.
├── .github/
│   ├── agents/              # AI agent definitions
│   ├── commands/            # Custom commands
│   ├── instructions/        # Language-specific AI instructions
│   ├── prompts/             # Reusable AI prompts
│   ├── workflows/           # GitHub Actions workflows
│   ├── ISSUE_TEMPLATE/      # Issue templates
│   ├── AGENTS.md            # Agent documentation
│   ├── copilot-instructions.md
│   ├── dependabot.yml
│   └── pull_request_template.md
├── .vscode/                 # VS Code settings
├── CLAUDE.md                # Claude AI instructions
├── LICENSE                  # MIT License
├── .editorconfig            # Editor configuration
├── .gitattributes           # Git attributes
├── .gitignore               # Git ignore patterns
├── .megalinter.yml          # MegaLinter configuration
└── .shellcheckrc            # ShellCheck configuration
```

## Available Workflows

### 1. Unified Linters (`aio.yml`)
Runs ShellCheck and Super-Linter on PRs and workflow dispatch. Automatically commits fixes.

### 2. CI (`ci.yml`)
Reusable CI workflow for shell projects.

### 3. Config Validation (`validate-configs.yml`)
Validates and auto-fixes YAML, TOML, JSON, and other config files.

### 4. Template (`template.yml`)
Generic workflow template for custom CI/CD pipelines.

## AI Agents

This template includes specialized AI agents for different tasks:

- **bash-expert**: Modern, secure Bash scripting
- **python.agent**: Python development best practices
- **rust.agent**: Rust development guidelines
- **critical-thinking**: Logic and reasoning analysis
- **refactoring-expert**: Code refactoring assistance
- **github-issue-fixer**: Automated issue handling

See `.github/AGENTS.md` for detailed agent descriptions.

## Customization

### Adding Custom Workflows

1. Create a new file in `.github/workflows/`
2. Use `template.yml` as a starting point
3. Customize for your specific needs

### Modifying AI Instructions

- Edit `CLAUDE.md` for project-specific Claude instructions
- Modify `.github/copilot-instructions.md` for Copilot behavior
- Add language-specific instructions to `.github/instructions/`

### Adjusting Linters

- Configure MegaLinter in `.megalinter.yml`
- Customize ShellCheck rules in `.shellcheckrc`
- Adjust Super-Linter settings in `.github/workflows/aio.yml`

## Best Practices

1. **Keep AI instructions up to date** - Update `CLAUDE.md` as your project evolves
2. **Enable Dependabot** - Automatically receive dependency update PRs
3. **Use issue templates** - Ensure consistent bug reports and feature requests
4. **Run linters locally** - Don't wait for CI to catch formatting issues
5. **Leverage AI agents** - Use specialized agents for specific tasks

## Requirements

- GitHub Actions enabled
- Recommended: GitHub Copilot or Claude Code access
- Optional: MegaLinter for comprehensive linting

## Contributing

1. Fork this repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

MIT License - see [LICENSE](LICENSE) for details.

## Related

- [Claude](https://www.anthropic.com/claude)
- [GitHub Copilot](https://github.com/features/copilot)
- [Super-Linter](https://github.com/super-linter/super-linter)
- [MegaLinter](https://megalinter.io/)
