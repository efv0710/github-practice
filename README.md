```mermaid
stateDiagram
    direction LR
    [*] --> Waiting
    Waiting --> Processing
    Processing --> Successful
    state Processing {
        direction LR
        Incomplete --> Complete
    }
    Processing --> Failed
