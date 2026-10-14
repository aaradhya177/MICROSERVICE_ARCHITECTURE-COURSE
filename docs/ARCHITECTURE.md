# Architecture decision record

## Decision

Use a static, buildless single-page application with a structured JavaScript content model.

## Rationale

The product requires rich client interactions but no authenticated server state. Static delivery minimizes supply-chain and runtime complexity, starts instantly, and keeps progress explicitly browser-local. Hash routing works on static hosting without rewrite configuration. Curriculum data remains separate from renderers so lessons can be expanded or migrated to Markdown later.

## Trade-offs

The current code display is styled but does not parse syntax tokens, and examples run locally rather than in an unsafe in-browser executor. Search is in-memory, appropriate for 90 lessons. A future authenticated edition should move progress behind a versioned API while retaining an offline cache.

