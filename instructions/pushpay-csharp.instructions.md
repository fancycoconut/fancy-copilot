---
description: 'Guidelines for building C# applications'
applyTo: "**/*.cs"
---

# C# Development
- Always use the latest version C#, currently C# 13 features

## General Instructions
- Always follow security best practices
- Follow RESTful API design principles

## Code Quality
- Ensure SOLID principles compliance
- Prefer composition over inheritance
- Keep methods focused and cohesive
- Implement proper disposal patterns for resources

## Naming Conventions
- Use PascalCase for classes, method names and public members
- use camelCase for private fields and local variables
- Prefix interface names with "I" e.g. IUserService

# Code style
- For if-else blocks, the opening curly brace must be on the same line as the if, else if, else - for example `if (true) {`
- Drop the use of the `private` keyword for methods, fields, etc

## Testing
- Follow the AAA pattern (Arrange, Act, Assert)
- Use Verify for snapshot tests
- Use Moq for mocking dependencies
- Test both success and failure scenarios
