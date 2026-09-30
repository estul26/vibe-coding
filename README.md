# vibe-coding

This repository is currently in the project-definition stage. Before implementation begins, the project should establish a clear public identity, an explicit architecture baseline, and a reproducible bootstrap prompt for Codex.

## Next Steps

### 1. Finalize the Project Name

Give the project a formal name that reflects its broader positioning rather than limiting it to a single feature such as memory.

Run a collision and discoverability check across:

- GitHub repositories
- General web search
- Go packages and modules
- npm
- PyPI
- Docker Hub and GHCR
- Domain availability
- Existing AI products and developer tools
- Preliminary trademark-risk checks

From that research, produce a shortlist of approximately **10 strong names** that are suitable for a public open-source project.

The final choice should include:

- A memorable project/brand name
- A clear, descriptive tagline
- Good searchability and discoverability
- Low risk of confusion with established projects or products
- Room for the project to grow beyond its initial feature set

### 2. Create `Architecture Baseline v0.1`

Produce the first formal architecture baseline for the project.

The baseline should define, at minimum:

- Project purpose and scope
- Core principles
- System boundaries
- Major components and responsibilities
- Data model and source-of-truth strategy
- Context, state, records, and memory boundaries
- APIs and integration points
- Storage strategy
- Identity, authentication, and authorization boundaries
- Privacy and security model
- Self-hosting and deployment model
- Extensibility model
- Observability and auditability
- Failure and recovery expectations
- Explicit non-goals
- Deferred scope
- Architecture Decision Record (ADR) process
- Acceptance criteria for the first implementation milestone

The purpose of `Architecture Baseline v0.1` is to create a stable reference that future implementation work must follow unless an intentional architecture decision changes it.

### 3. Create the Final Codex Bootstrap Prompt

After the project name and `Architecture Baseline v0.1` are complete, create a final bootstrap prompt for Codex.

The prompt should instruct Codex to:

- Treat the architecture baseline as authoritative
- Inspect the repository before making changes
- Preserve requirement traceability
- Work incrementally through explicit milestones
- Avoid silently expanding scope
- Record important architectural decisions
- Keep implementation, tests, documentation, and acceptance criteria synchronized
- Clearly report completed, partial, blocked, and deferred work
- Never claim a milestone is complete until its acceptance criteria pass
- Leave the repository in a reproducible and reviewable state after each milestone

The bootstrap prompt should be suitable for starting implementation in a fresh Codex chat without relying on hidden context from previous conversations.
