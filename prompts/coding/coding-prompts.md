# 💻 Coding & Development Prompts

Prompts for code generation, debugging, review, and software engineering tasks.

## Code Generation

### Generate Clean Python Function
```
Write a Python function that [description].

Requirements:
- Type hints on all parameters and return value
- Docstring with Args, Returns, and Example sections
- Handle edge cases: [list cases]
- Follow PEP 8 style guidelines
- Include input validation

Output only the function, no explanation.
```

### Generate REST API Endpoint
```
Create a [framework: FastAPI/Flask/Express] endpoint that:
- Method: [GET/POST/PUT/DELETE]
- Path: /api/v1/[resource]
- Request body: [schema]
- Response: [schema]
- Include input validation, error handling, and appropriate status codes
- Add OpenAPI docstring/comments
```

### Generate Database Schema
```
Design a [PostgreSQL/MySQL/MongoDB] schema for a [domain] application.

Entities: [list entities]
Relationships: [describe]

Include:
- Primary keys, foreign keys, indexes
- Created/updated timestamps
- Appropriate data types and constraints
- Migration-ready SQL (or Mongoose schemas)
```

### Generate Unit Tests
```
Write comprehensive unit tests for the following function using [pytest/jest/unittest]:

[paste function]

Cover:
- Happy path with typical inputs
- Edge cases (empty, None, boundary values)
- Error cases (invalid input, exceptions)
- Use descriptive test names (test_should_[behavior]_when_[condition])
- Use fixtures/mocks where appropriate
```

### Generate CLI Tool
```
Create a Python CLI tool using argparse/click that:
- Name: [tool name]
- Commands: [list commands]
- For each command: describe arguments, options, and behavior
- Include --help descriptions
- Add colored output (rich/click.echo)
- Handle errors gracefully with exit codes
```

## Code Review & Debugging

### Code Review
```
Review the following code for:
1. Bugs and logical errors
2. Security vulnerabilities (injection, secrets, auth)
3. Performance issues (N+1 queries, unnecessary loops, memory leaks)
4. Code style and readability
5. Missing error handling
6. Test coverage gaps

Rate severity: 🔴 Critical / 🟡 Warning / 🟢 Suggestion

Code:
[paste code]
```

### Debug This Error
```
I'm getting the following error:

Error message:
[paste error]

Relevant code:
[paste code]

Environment: [Python 3.x / Node.js / etc.]

Please:
1. Explain WHY this error occurs
2. Show the EXACT fix
3. Explain how to prevent it in the future
```

### Refactor for Production
```
Refactor this code to be production-ready:

[paste code]

Apply these principles:
- SOLID principles
- DRY (Don't Repeat Yourself)
- Proper error handling and logging
- Configuration via environment variables
- Type safety
- Documentation
```

### Explain Code
```
Explain this code line by line as if teaching a junior developer:

[paste code]

For each significant block:
1. What it does
2. Why it's done this way
3. Any gotchas or non-obvious behavior
```

## Architecture & Design

### System Design
```
Design a system for [use case].

Requirements:
- Expected traffic: [X] requests/second
- Data size: [X] records
- Availability: [99.9%/99.99%]

Include:
1. High-level architecture diagram (describe in text)
2. Component breakdown
3. Database choice and schema
4. API design
5. Caching strategy
6. Scaling approach
7. Monitoring & alerting
```

### Design Pattern
```
Implement the [pattern name] design pattern in [Python/TypeScript/Java] for [use case].

Include:
- Abstract base classes/interfaces
- Concrete implementations (at least 2)
- Usage example
- When to use vs. alternatives
```

## DevOps & Infrastructure

### Dockerfile
```
Create an optimized, production-ready Dockerfile for a [Python/Node.js/Go] application.

Requirements:
- Multi-stage build
- Non-root user
- Minimal image size (alpine-based)
- .dockerignore included
- Health check
- Environment variable configuration
- Proper layer caching order
```

### GitHub Actions CI/CD
```
Create a GitHub Actions workflow for a [language] project that:
1. Runs on push to main and PRs
2. Lints code with [linter]
3. Runs tests with coverage reporting
4. Builds Docker image
5. Deploys to [target] on main branch push
6. Caches dependencies between runs
```

### Kubernetes Manifest
```
Create Kubernetes manifests for deploying a [type] application:
- Deployment with [N] replicas
- Service (ClusterIP/LoadBalancer)
- ConfigMap for configuration
- Secret for credentials
- HPA for autoscaling
- Ingress with TLS
- Resource limits and requests
```
