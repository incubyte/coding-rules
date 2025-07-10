## Development Approach
- **TDD**: Write tests first, follow red-green-refactor cycle
- **Tidy First**: Clean code structure before adding features
- **Small iterations**: Work in tiny, safe steps

## Three Laws of TDD
1. Don't write production code until you have a failing unit test
2. Don't write more of a unit test than is sufficient to fail
3. Don't write more production code than is sufficient to make the test pass

## TDD Cycle with Verification
**RED-GREEN-REFACTOR** with mandatory test execution:

1. **RED**: Write failing test → **RU** → Verify it fails → Commit
2. **GREEN**: Write minimal code → **RU**N→ Verify it passes → Commit  
3. **REFACTOR**: Improve code → **RU** → Verify still passes → Commit

**⚠️ Critical**: NEVER assume tests pass/fail - always run them to verify!

## Architecture & Clean Code Principles

### Domain-Driven Design (DDD) Boundaries
- **Domain-specific organization** over technological boundaries
- Structure by business domains: `users/`, `leads/`, `conferences/`, `meetings/`
- **NOT** by tech layers: `controllers/`, `services/`, `repositories/`

### Clean Code Standards
- **Single Responsibility Principle**: Each module has one reason to change
- **Clear naming**: Functions and variables should be self-documenting
- **Small functions**: Do one thing well
- **Domain language**: Use business terminology in code
- **Proper abstractions**: Hide implementation details behind clear interfaces

### Boundary Guidelines
- **Domain**: Business logic, entities, value objects
- **Application**: Use cases, commands, queries
- **Infrastructure**: Database, external APIs, frameworks
- **Shared**: Common utilities used across domains
