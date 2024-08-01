# DirectoryStructures305
```mermaid
%%{ init: { 'themeVariables': { 'fontFamily': 'Arial', 'fontSize': '16px', 'primaryColor': '#000000', 'edgeLabelBackground': '#ffffff', 'tertiaryColor': '#ffffff' }, 'flowchart': { 'curve': 'linear', 'direction': 'TB' } } }%%
flowchart TB
    subgraph AgileMethodology
        direction TB
        style AgileMethodology fill:#ffffff,stroke:#000000,stroke-width:2px

        Start([Project Initiation]) --> Planning([Planning])
        Planning --> Backlog([Product Backlog])
        Backlog --> SprintPlanning([Sprint Planning])
        SprintPlanning --> Design([Design])
        Design --> Development([Development])
        Development --> Testing([Testing])
        Testing --> Review([Sprint Review])
        Review --> Retrospective([Sprint Retrospective])
        Retrospective --> Increment([Product Increment])
        Increment --> SprintPlanning
    end

    style Start fill:#FFCC99,stroke:#000000
    style Planning fill:#FFCC99,stroke:#000000
    style Backlog fill:#FFCC99,stroke:#000000
    style SprintPlanning fill:#FF9999,stroke:#000000
    style Design fill:#99CCFF,stroke:#000000
    style Development fill:#99CCFF,stroke:#000000
    style Testing fill:#99CCFF,stroke:#000000
    style Review fill:#99CCFF,stroke:#000000
    style Retrospective fill:#99FF99,stroke:#000000
    style Increment fill:#FFFF99,stroke:#000000

```
Welcome to **DirectoryStructures305**! This repository showcases an innovative approach to representing workflows, procedures, and models using directory structures and shortcuts. By aligning folders with processes, decisions, and components of models, these structures mirror how we work and what we work on, providing a clear and organized view of complex systems. .lnk files represent relationships between different elements, offering a structured and interactive way to navigate these systems.

It's important to recognize that while these directory structures offer a starting point, they may not fit every individual or organizational need. Customization may be necessary to tailor the structures to your specific requirements, as there is no one-size-fits-all solution. If you need assistance with customizing these directory structures for your needs, feel free to contact me.

# Workflows Overview

The repository includes multiple examples to illustrate different workflow representation strategies:

| Workflow Type | Description |
| :------------------------- | :---------------------------------------------------------- |
| **Simple Linear Workflow** | A straightforward linear workflow from start to finish. |
| **Conditional Workflow** | A workflow with conditional branching, guiding the process based on specific conditions. |
| **Decision-Based Workflow** | A decision-based workflow with conditional logic leading to different paths. |
| **Cyclical Workflow** | A cyclical workflow that loops back to the beginning, creating a repeating process. |


## Workflow 1 (Simple Linear Workflow): 

**Flowchart:**
![Simple Flowchart](https://github.com/user-attachments/assets/693e2f85-45df-42b6-a3c3-78cd8603f2d0)

**Flowchart by Mermaid:**
```mermaid
%%{ init: { 'flowchart': { 'curve': 'linear' } } }%%
flowchart LR

Start(start) --> A[process A]
A --> B[process B]
B --> C[process C]
C --> D[process D]
D --> End(end)

style Start fill:#E5BEFB
style End fill:#E5BEFB

style A fill:#FBBEBE
style B fill:#FBBEBE
style C fill:#FBBEBE
style D fill:#FBBEBE
```

**Directory Structure based on the flowchart:**
```plaintext
Workflows
└───Simple Linear Workflow
    ├───start
    │   └───goto process A.lnk
    ├───process A
    │   └───goto process B.lnk
    ├───process B
    │   └───goto process C.lnk
    ├───process C
    │   └───goto process D.lnk
    ├───process D
    │   └───goto end.lnk
    └───end
```

## Workflow 2 (Conditional Workflow):

**Flowchart:**
![Flowchart with 1 decision](https://github.com/user-attachments/assets/e6683b9e-2e1f-4c27-a45d-e3c2ae78f0c9)

**Flowchart by Mermaid:**
```mermaid
%%{ init: { 'flowchart': { 'curve': 'linear' } } }%%
flowchart LR

Start(start) --> A[process A]
A --> X{decision X}
X --> |yes| B[process B]
X --> |no| C[process C]
B --> D[process D]
C --> End(end)
D --> End(end)

style Start fill:#E5BEFB
style End fill:#E5BEFB

style A fill:#FBBEBE
style B fill:#FBBEBE
style C fill:#FBBEBE
style D fill:#FBBEBE

style X fill:#FBBEBE
```

**Directory Structure based on the flowchart:**
```plaintext
Workflows
└───Conditional Workflow
    ├───start
    │   └───goto process A.lnk
    ├───process A
    │   └───goto decision X.lnk
    ├───decision X
    │   ├───goto process B if x is true.lnk
    │   └───goto process C if x is false.lnk
    ├───process B
    │   └───goto process D.lnk
    ├───process C
    │   └───goto end.lnk
    ├───process D
    │   └───goto end.lnk
    └───end

```

## Workflow 3 (Decision-Based Workflow):

**Flowchart:**
![Flowchart with 1 decision and 1 loop](https://github.com/user-attachments/assets/f67d9494-f131-4855-a21e-8ede25c8a84d)

**Flowchart by Mermaid:**
```mermaid
%%{ init: { 'flowchart': { 'curve': 'linear' } } }%%
flowchart LR

Start(start) --> A[process A]
A --> X{decision X}
X --> |yes| B[process B]
X --> |no| C[process C]
B --> D[process D]
C --> A
D --> End(end)

style Start fill:#E5BEFB
style End fill:#E5BEFB

style A fill:#FBBEBE
style B fill:#FBBEBE
style C fill:#FBBEBE
style D fill:#FBBEBE

style X fill:#FBBEBE
```

**Directory Structure based on the flowchart:**
```plaintext
Workflows
└───Decision-Based Workflow
    ├───start
    │   └───goto process A.lnk
    ├───process A
    │   └───goto decision X.lnk
    ├───decision X
    │   ├───goto process B if x is true.lnk
    │   └───goto process C if x is false.lnk
    ├───process B
    │   └───goto process D.lnk
    ├───process C
    │   └───goto process A.lnk
    ├───process D
    │   └───goto end.lnk
    └───end
```

## Workflow 4 (Cyclical Workflow):

**Flowchart:**
![Endless Flowchart with 1 loop](https://github.com/user-attachments/assets/c2332b68-2b52-454c-81e4-d020f206aa36)

**Flowchart by Mermaid:**
```mermaid
%%{ init: { 'flowchart': { 'curve': 'linear' } } }%%
flowchart LR

Start(start) --> A[process A]
A --> B[process B]
B --> C[process C]
C --> D[process D]
D --> A

style Start fill:#E5BEFB

style A fill:#FBBEBE
style B fill:#FBBEBE
style C fill:#FBBEBE
style D fill:#FBBEBE
```

**Directory Structure based on the flowchart:**
```plaintext
Workflows
└───Cyclical Workflow
    ├───start
    │   └───goto process A.lnk
    ├───process A
    │   └───goto process B.lnk
    ├───process B
    │   └───goto process C.lnk
    ├───process C
    │   └───goto process D.lnk
    └───process D
        └───goto process A.lnk
```
# Learn More

1. [Video: Organize Your Files](https://datamanagement.hms.harvard.edu/plan-design/directory-structure)
2. [Blog: Directory Structure](https://dpbestflow.org/file-management/directory-structure)
3. [Research Data Management - File Organization](https://guides.nyu.edu/data_management/file-org)
4. [Directory Structures for researchers, with examples](https://ubco-biology.github.io/Procedures-and-Guidelines/directory-structures.html)
