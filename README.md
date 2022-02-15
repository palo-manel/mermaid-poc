# Mermaid POC

[Mermaid](https://github.com/mermaid-js/mermaid#readme) is a JavaScript based diagramming and charting tool that takes Markdown-inspired text definitions and creates diagrams dynamically in the browser. It supports a bunch of different common diagram types for software projects, including flowcharts, UML, Git graphs, user journey diagrams, and even the dreaded Gantt chart.

[Github has rolled out](https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/) a change that will allow you to create graphs inline using [Mermaid syntax](https://mermaid-js.github.io/mermaid/#/n00b-syntaxReference?id=syntax-structure).

## Simple flowchart

This is an example of a simple flowchart.

```mermaid
  graph TD;
      A-->B;
      A-->C;
      B-->D;
      C-->D;
```

## Advanced flowchart

This is an example of a more advanced flowchart, it uses different block shapes and arrow captions.

```mermaid
  flowchart TD;
      A[Deploy to Production] --> B{Is it Friday?};
      B -- Yes --> C[Do not deploy!];
      B -- No --> D[Run deploy.sh to deploy!];
      C ----> E[Enjoy your weekend];
      D ----> E[Enjoy your weekend];
```
