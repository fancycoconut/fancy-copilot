---
description: 'Guidelines for building C# applications'
applyTo: '**'
---

# C# Development
- Always use the latest version C#, currently C# 14 features

## General Instructions
- Make only high confidence suggestions when reviewing code changes
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
- If there are multiple uppercase characters in the name, only the first letter will be upper case for example `DTO` becomes `Dto`, `API` becomes `Api`

# Code style
- Apply code-formatting style defined in `.editorconfig`
- Do not use the suffix `Async` to mark async methods

## Testing
- Follow the AAA pattern (Arrange, Act, Assert)
- Use Verify for snapshot tests
- Use Moq for mocking dependencies
- Test both success and failure scenarios
