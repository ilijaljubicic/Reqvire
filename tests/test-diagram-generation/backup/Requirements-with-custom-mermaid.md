# Test Requirements with Custom Mermaid

This is a requirements document specifically created for testing diagram generation.

## Section 1
```mermaid
graph TD;
  %% Graph styling
  classDef requirement fill:#f9d6d6,stroke:#f55f5f,stroke-width:1px;
  classDef verification fill:#d6f9d6,stroke:#5fd75f,stroke-width:1px;
  classDef externalLink fill:#d0e0ff,stroke:#3080ff,stroke-width:1px;
  classDef default fill:#f5f5f5,stroke:#333333,stroke-width:1px;

  d94b2c1859["Element 2"];
  click d94b2c1859 "Requirements-with-custom-mermaid.md#element-2";
  class d94b2c1859 requirement;
  2ac7edcf81["Element 1"];
  click 2ac7edcf81 "Requirements-with-custom-mermaid.md#element-1";
  class 2ac7edcf81 requirement;
  87ce6a6132["Element 3"];
  class 87ce6a6132 requirement;
  click 87ce6a6132 "Requirements-with-custom-mermaid.md#element-3";
  2ac7edcf81 -->|verifies| 87ce6a6132;
```


### Element 1

This is a test element with relations.

#### Relations
  * satisfies: [Element 2](#element-2)
  * verifies: [Element 3](#element-3)

### Element 2

This is another test element with relations.

#### Relations
  * tracedFrom: [Element 1](#element-1)

## Custom Mermaid Diagram Section

This section contains a custom mermaid diagram that should not be removed:

```mermaid
flowchart TD
    A[Start] --> B{Is it?}
    B -- Yes --> C[OK]
    C --> D[Rethink]
    D --> B
    B -- No --> E[End]
```

## Section 2
```mermaid
graph TD;
  %% Graph styling
  classDef requirement fill:#f9d6d6,stroke:#f55f5f,stroke-width:1px;
  classDef verification fill:#d6f9d6,stroke:#5fd75f,stroke-width:1px;
  classDef externalLink fill:#d0e0ff,stroke:#3080ff,stroke-width:1px;
  classDef default fill:#f5f5f5,stroke:#333333,stroke-width:1px;

  3651a8aa0b["Element 4"];
  click 3651a8aa0b "Requirements-with-custom-mermaid.md#element-4";
  class 3651a8aa0b requirement;
  87ce6a6132["Element 3"];
  click 87ce6a6132 "Requirements-with-custom-mermaid.md#element-3";
  class 87ce6a6132 requirement;
  2ac7edcf81["Element 1"];
  class 2ac7edcf81 requirement;
  click 2ac7edcf81 "Requirements-with-custom-mermaid.md#element-1";
  2ac7edcf81 -->|verifies| 87ce6a6132;
```


### Element 3

This is a third test element.

#### Relations
  * verifiedBy: [Element 1](#element-1)

### Element 4

This is a fourth test element with no relations.