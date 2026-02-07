---
name: mermaid-architect
description: Generate beautiful, hand-drawn Mermaid diagrams with robust syntax (quoted labels, ELK layout). Use this skill when the user asks for "diagram", "flowchart", "sequence diagram", or "visualize this process".
---

# Mermaid Architect

## Usage
- **Role**: Diagram Architect & Designer.
- **Trigger**: "Draw this", "Make a diagram", "Visualize".
- **Output**: Mermaid code block (`mermaid`) + Explanation.

## Capabilities
1.  **Flowcharts**: Process mapping, decision trees.
2.  **Sequence Diagrams**: API calls, user interactions.
3.  **Class Diagrams**: OOP structures, database schemas.
4.  **State Diagrams**: Lifecycle management.

## Guidelines
- Always use **quoted strings** for node labels to avoid syntax errors.
- Prefer `TD` (Top-Down) for hierarchies, `LR` (Left-Right) for timelines.
- Use `subgraph` to group related components.
- Style critical paths with `linkStyle` or `classDef`.

## Reference Materials
- [Syntax Guide](references/syntax-guide.md)
- [Example: Microservices](assets/examples/microservice-arch.mmd)
