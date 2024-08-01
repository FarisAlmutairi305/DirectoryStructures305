# DirectoryStructures305

Welcome to **DirectoryStructures305**! This repository showcases an innovative approach to representing workflows, procedures, and models using directory structures and shortcuts. By aligning folders with processes, decisions, and components of models, these structures mirror how we work and what we work on, providing a clear and organized view of complex systems. .lnk files represent relationships between different elements, offering a structured and interactive way to navigate these systems.

It's important to recognize that while these directory structures offer a starting point, they may not fit every individual or organizational need. Customization may be necessary to tailor the structures to your specific requirements, as there is no one-size-fits-all solution. If you need assistance with customizing these directory structures for your needs, feel free to contact me.


## Overview

The repository includes multiple methods to illustrate different workflow strategies:

- **Method 1**: A straightforward linear workflow from start to finish.
- **Method 2**: A workflow with conditional branching, guiding the process based on specific conditions.
- **Method 3**: A cyclical workflow that loops back to the beginning, creating a repeating process.
- **Method 4**: A decision-based workflow with conditional logic leading to different paths.


## Workflow 1, and a directory structure aligned with it: 

![Simple Flowchart](https://github.com/user-attachments/assets/f8bd0360-35d1-4f55-bcc2-6b21f0401c8f)

```plaintext
.
Flowcharts
└───Simple Flowchart
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

## Workflow 2, and a directory structure aligned with it:

![Flowchart with 1 decision](https://github.com/user-attachments/assets/ffc492cd-12ec-4f55-af14-503bf4b0dfb0)

```plaintext
Flowcharts
└───Flowchart with 1 decision
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

## Workflow 3, and a directory structure aligned with it:

![Flowchart with 1 decision and 1 loop](https://github.com/user-attachments/assets/e61bb457-ca10-48f0-910c-e8f0e7905cc1)

```plaintext
Flowcharts
└───Flowchart with 1 decision and 1 loop
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

## Workflow 4, and a directory structure aligned with it:

![Endless Flowchart with 1 loop](https://github.com/user-attachments/assets/080390fe-3bae-4208-b4f4-5efe5d83f6d2)

```plaintext
Flowcharts
└───Endless Flowchart with 1 loop
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
