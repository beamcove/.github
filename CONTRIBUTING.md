# Contributing to Beamcove Projects

> **First off, thank you!** Whether you're fixing a typo or refactoring the entire codebase, we appreciate your contribution.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Setup](#development-setup)
- [Pull Request Process](#pull-request-process)
- [Style Guidelines](#style-guidelines)
- [Community](#community)

## Code of Conduct

By participating in this project, you agree to abide by our [Code of Conduct](CODE_OF_CONDUCT.md). TL;DR: Be kind, be respectful, be professional. We're all here to build cool stuff together.

## How Can I Contribute?

### Reporting Bugs 🐛

Found a bug? First, check if it's already been reported in our [issue tracker](../../issues). If not, create a new issue using our bug report template. The more details you provide, the easier it is for us to fix it.

**Great bug reports include:**
- A clear, descriptive title
- Steps to reproduce the issue
- Expected vs. actual behavior
- Your environment (OS, browser, version)
- Screenshots or error logs (if applicable)

### Suggesting Features ✨

Have an idea for a new feature? We'd love to hear it! Open a feature request and tell us:
- What problem does this solve?
- How should it work?
- Why is this important to you?

Not all features will make it in, but every idea helps us understand what users need.

### Contributing Code 💻

Ready to write some code? Awesome! Here's how:

1. **Find an issue to work on** — Look for issues labeled `good first issue` or `help wanted`
2. **Fork the repository** — Create your own copy to work in
3. **Create a branch** — Use a descriptive name: `fix/broken-api-endpoint` or `feature/add-dark-mode`
4. **Write your code** — Follow our style guidelines (see below)
5. **Test your changes** — Make sure everything works and you haven't broken existing functionality
6. **Submit a pull request** — Fill out the PR template completely

### Improving Documentation 📚

Good documentation is as valuable as good code. Spot a typo? Found something confusing? Documentation PRs are always welcome!

## Development Setup

### Prerequisites

<!-- Adjust this section based on your actual tech stack -->

- Node.js (version X.X or higher)
- Git
- A sense of humor (highly recommended)

### Getting Started

```bash
# Clone your fork
git clone https://github.com/YOUR-USERNAME/REPOSITORY-NAME.git

# Navigate to the directory
cd REPOSITORY-NAME

# Add the upstream remote
git remote add upstream https://github.com/beamcove/REPOSITORY-NAME.git

# Install dependencies
npm install

# Run tests to make sure everything works
npm test

# Start developing!
```

### Running Tests

```bash
# Run all tests
npm test

# Run tests in watch mode
npm test -- --watch

# Run a specific test file
npm test path/to/test.js
```

## Pull Request Process

1. **Update documentation** — If your change affects how users interact with the project, update the docs
2. **Add tests** — New features should have tests. Bug fixes should include a test that would have caught the bug
3. **Follow the style guide** — Consistent code is happy code
4. **Keep it focused** — One PR should address one issue or add one feature
5. **Write a clear PR description** — Use our template and fill it out completely
6. **Be responsive** — Address review feedback promptly and professionally

### What Happens Next?

- A maintainer will review your PR (usually within a few days)
- They might request changes — don't take it personally!
- Once approved, your PR will be merged
- Your name will be added to the contributors list 🎉

## Style Guidelines

### Git Commit Messages

- Use the present tense ("Add feature" not "Added feature")
- Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
- Limit the first line to 72 characters or less
- Reference issues and pull requests liberally after the first line

**Good commit messages:**
```
Add user authentication endpoint

- Implement JWT token generation
- Add password hashing with bcrypt
- Include rate limiting for login attempts

Fixes #123
```

### Code Style

- **JavaScript/TypeScript**: We use [ESLint](https://eslint.org/) — run `npm run lint` before committing
- **Python**: We follow [PEP 8](https://pep8.org/) — use `flake8` to check your code
- **Formatting**: We use [Prettier](https://prettier.io/) for auto-formatting (if applicable)

**General principles:**
- Write self-documenting code (clear variable and function names)
- Add comments for complex logic, not obvious code
- Keep functions small and focused
- Avoid premature optimization

### Testing

- Write tests for new features
- Ensure all tests pass before submitting a PR
- Aim for meaningful test coverage, not just high percentages
- Test edge cases and error conditions

## Community

### Where to Get Help

- **Documentation**: Start here — most questions are answered in the docs
- **Discussions**: Join our [GitHub Discussions](https://github.com/orgs/beamcove/discussions) for questions and conversations
- **Issues**: For bugs and feature requests
- **Chat**: [Your chat platform] for real-time discussion

### Recognition

We believe in recognizing our contributors:
- All contributors are added to our README
- Significant contributions get a shoutout in release notes
- Regular contributors may be invited to join the core team

## Questions?

Still not sure about something? Don't be shy — open an issue with your question or join our discussions. We're here to help!

---

**Remember**: Contributing to open source should be fun. If it's not, something's wrong. Don't hesitate to reach out if you're stuck or frustrated.

Happy coding! 🚀
