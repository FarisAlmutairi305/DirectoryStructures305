# DirectoryStructures305

Welcome to **DirectoryStructures305**! This repository showcases an innovative approach to representing workflows, procedures, and models using directory structures and shortcuts. By aligning folders with processes, decisions, and components of models, these structures mirror how we work and what we work on, providing a clear and organized view of complex systems. .lnk files represent relationships between different elements, offering a structured and interactive way to navigate these systems.

It's important to recognize that while these directory structures offer a starting point, they may not fit every individual or organizational need. Customization may be necessary to tailor the structures to your specific requirements, as there is no one-size-fits-all solution. If you need assistance with customizing these directory structures for your needs, feel free to contact me.


## Overview

The repository includes multiple examples to illustrate different workflow and model representation strategies:

1 - **Simple Linear Workflow**: A straightforward linear workflow from start to finish.
2 - **Conditional Workflow**: A workflow with conditional branching, guiding the process based on specific conditions.
3 - **Decision-Based Workflow**: A decision-based workflow with conditional logic leading to different paths.
4 - **Cyclical Workflow**: A cyclical workflow that loops back to the beginning, creating a repeating process.


## Workflow 1 (Simple Linear Workflow): 

![Simple Flowchart](https://github.com/user-attachments/assets/d3e5a61f-947e-4949-8101-fde703d61b37)

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

![Flowchart with 1 decision](https://github.com/user-attachments/assets/443f200d-ecf1-4263-8f13-b85a6c36c213)

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

![Flowchart with 1 decision and 1 loop](https://github.com/user-attachments/assets/0c604705-eac3-46a9-a43a-e241af405e37)

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

![Endless Flowchart with 1 loop](https://github.com/user-attachments/assets/e68ebfc2-440e-4481-93dd-a4fa6cb415d7)

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
## Learn More

[Video: Organize Your Files](https://datamanagement.hms.harvard.edu/plan-design/directory-structure)
