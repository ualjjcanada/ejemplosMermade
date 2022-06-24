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
    subgraph main
    7
    end;
    subgraph dev
    6
    end;
    subgraph HEAD
    7
    end;
    
```
