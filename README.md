# nuevoborrar

# mermaid
[Include diagrams in your Markdown files with Mermaid](https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/)   

[Mermaid website](https://mermaid-js.github.io/mermaid/) 

```mermaid
  graph TD;
      A-->B;
      A-->C;
      B-->D;
      C-->D;
```

```mermaid
    flowchart TD;

    A[Process] --> B{Condition?};
    B -- Yes --> C[Another Process];
    B -- No --> D[Exit Process];
    C ----> E{Another Condition?};
    E -- Yes --> F[Etc...];
    E -- No --> G[Etc...];

```

```mermaid
    sequenceDiagram

    participant Alice
    participant Bob
    Alice->>John: Hello John, how are you?
    loop Healthcheck
        John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts <br/>prevail!
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!
```    

```mermaid
    pie

    title Key elements in Product X
    "Calcium" : 42.96
    "Potassium" : 50.05
    "Magnesium" : 10.01
    "Iron" :  5
```

Con enlaces incluidos

```mermaid
    flowchart LR;
    A-->B;
    B-->C;
    C-->D;
    D-->E;
    click A "http://www.github.com" _blank
    click B "http://www.github.com" "Open this in a new tab" _blank
    click C href "http://www.github.com" _blank
    click D href "http://www.github.com" "Open this in a new tab" _blank
```

```mermaid
    flowchart RL;
    2-->1;
    3-->2;
    4-->3;
    5-->3;
    6-->5;
    7-->6;
    7-->4;
    subgraph dev
    6
    end;
    subgraph otro[" "]
      direction TB
      id1(HEAD) -.-> id1(main)
      id1(main) -.-> 7
      style id1 fill:#f9f,stroke:#333,stroke-width:1px
    end;
    
```

Git detailed graph as a flowchart:

```mermaid
   flowchart RL;
    3((9817e0))-->1((e137e9));
    4((ae3e0f))-->3;
    id2(main) -.-> idHead
    id1(HEAD) -.-> id2(main)
    idHead((e2d9e6))-->6;
    idHead-->4;
    5((a1fbcd))-->3;
    52((86d91f))--> 5
    6((711a58))-->52;
    subgraph branchDev[" "]
      id3(dev) -.-> 6
    end
    
    style id1 fill:#b8dbbc,stroke:#333,stroke-width:1px
    style id2 fill:#f96,stroke:#333,stroke-width:1px
    style id3 fill:#f90,stroke:#333,stroke-width:1px
    style idHead fill:#b8dbbc
    style branchDev fill:#fff,stroke:#333,stroke-width:0px
    
```
    
