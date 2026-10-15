# Example integration diagram

```mermaid
flowchart LR
  A[On-prem source] -->|Batch file| B[Approved transfer boundary]
  B --> C[Validation and ingestion]
  C --> D[(Processed data store)]
  D --> E[Internal reporting]
```

This is fictitious; replace with verified system information.
