# Title
Qdrant Database

## Summary
- Qdrant (read: quadrant) is a vector similarity search engine and vector database. It provides a production-ready service with a convenient API to store, search, and manage points—vectors with an additional payload Qdrant is tailored to extended filtering support. It makes it useful for all sorts of neural-network or semantic-based matching, faceted search, and other applications.

- Can it be used for persistence of documents for vector search?

## Context & Scope
- **Why now:** `It came with the n8n docker compose and should have a good integration with it out of the box`
- **Boundaries:** `Can it be used by me locally?`

## Research Questions
1. How can it be used?
2. Is it cost effective?
3. Does it have a UI via docker?
4. Does it have any libraries that allow dotnet or Go to be integrated with?
5. How does it plug in with AI agents

## Background Knowledge
- `Vector database that allows you to perform similarity search.`
- `<Links to existing documentation or previous experiments>`

## Method & Experiments
- **Approach:** `<Methods, tools, datasets, evaluation criteria>`
- **Experiments:**
  - `<Experiment 1 name>` — `<purpose, setup, expected outcome>`
  - `<Experiment 2 name>` — `<purpose, setup, expected outcome>`

## Findings
- Can be used to store documents 
- Has a free tier for hosted versions and is built on Rust, should be fast.
- Uses HTTP but has gRPC option.
- Is an alternative for PineConeDb
- Does not have a UI, just http api.

## Analysis
- **What worked:** `<Successful techniques or insights>`
- **What failed:** `<Issues, blockers, trade-offs>`
- **Interpretation:** `<What the results mean for the original questions>`

## Decisions & Recommendations
- `<Decision or recommendation>` — `<rationale + confidence level>`
- `<Open issues>` — `<what still needs investigation>`

## Next Steps
1. `<Immediate action item>` — `<owner/date if applicable>`
2. `<Follow-up research or validation>`
3. `<Long-term considerations>`

## Resources & References
- `[Qdrant Github](https://github.com/qdrant/qdrant)` — `the repository of the code`

## Changelog
- `2025-10-22` — `Initial glance at the technology and its purpose`
