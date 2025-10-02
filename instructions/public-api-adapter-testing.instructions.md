---
description: 'Guidelines for writing tests with xunit for Public API Adapter'
applyTo: "**/*.cs"
---

# PublicApiAdapter Tests

Your goal is to help me write effective unit tests with XUnit, covering both standard and data-driven testing approaches.

## Project Setup
- The test project is at `/tests/PublicApiAdapter.Tests`
- Create test classes that match the classes being tested (e.g. `CalculatorTests` for `Calculator` or `UserServiceSpecs` for `UserService`)
- Use .NET SDK test commands: `dotnet test` for running tests

## Standard Tests
- Keep tests focused on a single behavior
- Avoid testing multiple behaviors in one test method
- Use clear assertions that express intent
- Include only the assertions needed to verify the test case
- Make tests independent and idempotent (can run in any order)
- Avoid test interdependencies

## Assertions
- Use `Assert.Equal` for value equality
- Use `Assert.Same` for reference equality
- Use `Assert.True`/`Assert.False` for boolean conditions
- Use `Assert.Contains`/`Assert.DoesNotContain` for collections
- Use `Assert.Matches`/`Assert.DoesNotMatch` for regex pattern matching
- Use `Assert.Throws<T> `or await `Assert.ThrowsAsync<T>` to test exceptions
