```mermaid
stateDiagram-v2
    [*] --> Waiting
    Waiting --> Incomplete
    state Processing {
        Incomplete --> Complete
    }
    Complete --> Successful
    Complete --> Failed
