# Mermaid Syntax Reference

## Flowchart
```mermaid
flowchart LR
    A[Start] --> B{Decision?}
    B -- Yes --> C[Process]
    B -- No --> D[End]
    C --> D
```
- **LR**: Left-to-Right layout
- **TD**: Top-Down layout
- `{}`: Rhombus (Decision)
- `[]`: Rectangle (Process)
- `()`: Rounded Rectangle

## Sequence Diagram
```mermaid
sequenceDiagram
    participant User
    participant System
    User->>System: Request Data
    activate System
    System-->>User: Return Data
    deactivate System
```
- `->>`: Solid line with arrow (Sync call)
- `-->>`: Dashed line with arrow (Async reply)
- `activate`/`deactivate`: Lifeline status

## Class Diagram
```mermaid
classDiagram
    class Animal {
        +String name
        +void eat()
    }
    class Dog {
        +void bark()
    }
    Animal <|-- Dog
```
- `<|--`: Inheritance
- `+`: Public
- `-`: Private
