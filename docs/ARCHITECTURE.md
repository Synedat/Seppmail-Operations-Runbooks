# Architecture

    Focus on recovery paths, decision gates, change evidence and communications.

    ## Overview diagram

    ```mermaid
flowchart TD
    A[Change request] --> B[Pre-checks]
    B --> C[Implementation]
    C --> D[Validation]
    D --> E[Evidence and rollback decision]
    E --> F[Closure / post-incident review]
```

    ## Design prompts

    - Which trust boundaries exist?
    - Which identities or tokens cross those boundaries?
    - Which dependencies are external and need explicit monitoring?
    - What is the fallback mode if a dependency is unavailable?
    - Which artefacts form the minimum evidence pack for change and recovery?
