# AGENTS.md — PharmaForm AI

## Mission
Build PharmaForm AI as a production-grade, modular, testable platform for pharmaceutical formulation intelligence.

Primary goals:
- correctness
- maintainability
- low token waste
- small verified steps
- strong architectural consistency

## Working Language
- Default language for communication: Turkish
- Code, folder names, technical identifiers, and commit messages may stay in English
- Explanations to the user should be concise and in Turkish

## Operating Mode
- Default reasoning effort: medium
- Use low reasoning for boilerplate, simple file creation, straightforward CRUD, formatting, and predictable edits
- Use high reasoning only for architecture, domain modeling, migrations, security-sensitive code, performance bottlenecks, or root-cause debugging
- Never use deeper reasoning than necessary

## Token Efficiency Rules
- Do not explain obvious things
- Do not repeat the task back unless ambiguity blocks execution
- Do not generate long preambles
- Keep outputs short and execution-focused
- Prefer the smallest viable change
- Prefer editing existing files over rewriting large files
- Avoid speculative refactors
- Do not create duplicate helpers, configs, or abstractions
- Do not add dependencies unless clearly justified

## Execution Rules
- First inspect repository structure and existing conventions
- Follow existing naming, folder, typing, lint, and test conventions
- Before coding, identify the minimum necessary files to change
- Make changes in small, reviewable increments
- After changes, run the smallest relevant validation first
- If the full test suite is expensive, run targeted checks before broader checks

## Architecture Rules
- Preserve clean boundaries between frontend, backend, domain, and intelligence layers
- Keep domain logic out of UI components
- Keep framework glue thin
- Prefer explicit types and predictable interfaces
- Favor composition over premature abstraction
- Design for extension, but do not over-engineer

## Product Priorities
1. Correct pharmaceutical domain modeling
2. Stable backend architecture
3. Reliable and simple UI
4. Explainable rule/AI outputs
5. Optimization and polish later

## MVP Discipline
For early phases:
- no microservices
- no unnecessary infrastructure
- no excessive design system work
- no broad feature sprawl before core MVP is stable

## Quality Bar
Each meaningful change should aim to include:
- acceptance criteria satisfied
- lint/type/test pass for touched scope
- no dead code
- no placeholder TODO comments unless explicitly requested
- concise doc updates when behavior changes

## Response Format
For each task, respond briefly with:
1. What was changed
2. Files changed
3. Validation run
4. Real risk/blocker if any

## When Blocked
- Ask at most one precise question if truly blocked
- Otherwise choose the safest reasonable assumption and continue

## Project Context
PharmaForm AI is an AI-assisted pharmaceutical formulation, stability, and optimization platform.

Initial product focus:
- nasal formulations
- hydrogels
- nanoformulations

Core platform scope:
- formulation recommendation
- excipient compatibility analysis
- stability risk scoring
- DoE and optimization planning
- release kinetics analysis
- automated reporting

## Delivery Principle
Always optimize for:
- clarity
- maintainability
- low token waste
- high implementation value
- long-term product coherence
