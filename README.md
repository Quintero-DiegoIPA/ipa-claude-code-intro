# Getting Started with Claude Code — IPA Colombia

A practical onboarding guide for IPA Colombia Research Analysts who want to start using [Claude Code](https://docs.anthropic.com/en/docs/claude-code/overview) for Stata-based research workflows.

## What This Is

A self-contained Quarto HTML document (50–75 minutes) that takes you from zero to productive with Claude Code. It covers:

- **VS Code basics**: terminal, file explorer, extensions, navigation
- **Claude Code setup**: installation, API key, first run
- **Project instructions**: how `CLAUDE.md` and skills work
- **Security and PII rules**: what to never do with research data
- **Prompt engineering**: five patterns for effective Stata prompts
- **Two hands-on exercises**: debug a Stata error, write a descriptive statistics do-file

## Audience

Research analysts proficient in Stata who have never used VS Code or Claude Code. The guide assumes familiarity with IPA and DIME Analytics coding standards.

## How to Use

### Option 1: Read the rendered HTML

Download `claude-code-guide.html` and open it in any browser. The file is fully self-contained (no external dependencies).

### Option 2: Render from source

If you have [Quarto](https://quarto.org/docs/get-started/) installed:

```bash
quarto render claude-code-guide.qmd --to html
```

## Prerequisites

To follow the exercises in the guide, you need:

- Stata 17 or later (installed and licensed)
- A GitHub repository cloned locally
- Node.js 18 or later ([download](https://nodejs.org/))
- An Anthropic API key

## License

This guide is shared for internal IPA use. Contact the IPA Colombia MEL team for questions.
