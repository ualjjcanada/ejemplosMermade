# nuevoborrar

# mermaid
Include diagrams in your Markdown files with Mermaid
https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/


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