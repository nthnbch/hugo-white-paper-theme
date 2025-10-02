# Contributing to Hugo White Paper Theme

Thank you for your interest in contributing to Hugo White Paper Theme! This document provides guidelines for contributing to the project.

## How to Contribute

### Reporting Issues

- Check if the issue has already been reported
- Include a clear title and description
- Provide steps to reproduce the issue
- Include screenshots if relevant
- Mention your Hugo version and environment

### Suggesting Enhancements

- Open an issue with your suggestion
- Explain why this enhancement would be useful
- Provide examples of how it would work

### Pull Requests

1. Fork the repository
2. Create a new branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Test thoroughly
5. Commit your changes (`git commit -m 'Add amazing feature'`)
6. Push to your branch (`git push origin feature/amazing-feature`)
7. Open a Pull Request

## Development Setup

```bash
# Clone the repository
git clone https://github.com/nthnbch/hugo-white-paper-theme
cd hugo-white-paper-theme

# Run the example site
hugo server --source=exampleSite --themesDir=../..
```

## Coding Guidelines

### SCSS

- Use CSS custom properties for colors and sizes
- Follow existing naming conventions
- Keep selectors simple and specific
- Comment complex logic

### HTML Templates

- Follow Hugo best practices
- Keep templates DRY (Don't Repeat Yourself)
- Use partials for reusable components
- Comment non-obvious logic

### Documentation

- Update README.md for user-facing changes
- Update CHANGELOG.md following Keep a Changelog format
- Add comments in code for complex logic

## Questions?

Open an issue or discussion on GitHub. We're happy to help!

## License

By contributing, you agree that your contributions will be licensed under the MIT License.
