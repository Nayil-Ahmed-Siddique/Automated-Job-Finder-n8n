# automated-job-finder-n8n

flowchart LR
    A[Schedule Trigger] --> B1[RSS Read 1]
    A --> B2[RSS Read 2]
    A --> B3[RSS Read 3]

    B1 --> C[Merge Feeds]
    B2 --> C
    B3 --> C

    C --> D[Filter: Software Jobs]
    D --> E[Filter: Country]
    E --> F[Job Scoring Logic]
    F --> G[Quality Filter]
    G --> H[Prepare Email Content]
    H --> I[Send Email Alert]
