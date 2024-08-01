# DirectoryStructures305

Welcome to **DirectoryStructures305**! This repository showcases an innovative approach to representing workflows, procedures, and models using directory structures and shortcuts. Folders are designed to align with processes, decisions, and components of models, creating an organized structure that mirrors your workflow or organizational needs. .lnk files represent relationships between different elements, providing a structured and interactive way to navigate and understand complex processes and models.


## Overview

The repository includes multiple methods to illustrate different workflow strategies:

- **Method 1**: A straightforward linear workflow from start to finish.
- **Method 2**: A workflow with conditional branching, guiding the process based on specific conditions.
- **Method 3**: A cyclical workflow that loops back to the beginning, creating a repeating process.
- **Method 4**: A decision-based workflow with conditional logic leading to different paths.

## Directory Structure

```plaintext
.
├───method 1
│   ├───flowchart.bmp
│   ├───step 1
│   │   └───goto step 2.lnk
│   ├───step 2
│   │   └───goto step 3.lnk
│   ├───step 3
│   │   └───goto step 4.lnk
│   ├───step 4
│   │   └───goto step 5.lnk
│   └───step 5
├───method 2
│   ├───flowchart.bmp
│   ├───step 1
│   │   └───goto step 2.lnk
│   ├───step 2
│   │   ├───goto step 3a if x is true.lnk
│   │   └───goto step 3b if x is false.lnk
│   ├───step 3a
│   │   └───goto step 4.lnk
│   ├───step 3b
│   │   └───goto step 4.lnk
│   ├───step 4
│   │   └───goto step 5.lnk
│   └───step 5
├───method 3
│   ├───flowchart.bmp
│   ├───step 1
│   │   └───goto step 2.lnk
│   ├───step 2
│   │   └───goto step 3.lnk
│   ├───step 3
│   │   └───goto step 4.lnk
│   ├───step 4
│   │   └───goto step 5.lnk
│   └───step 5
│       └───goto step 1.lnk
└───method 4
    ├───flowchart.bmp
    ├───step 1
    │   └───goto step 2.lnk
    ├───step 2
    │   ├───goto step 1 if x is false.lnk
    │   └───goto step 3 if x is true.lnk
    ├───step 3
    │   └───goto step 4.lnk
    ├───step 4
    │   └───goto step 5.lnk
    └───step 5
```

## method 1 workflow

![image](https://github.com/FarisAlmutairi305/EpicConcepts305/raw/main/directory%20structure%20as%20flowchart/method%201/flowchart.bmp)

## method 2 workflow

![image](https://github.com/FarisAlmutairi305/EpicConcepts305/raw/main/directory%20structure%20as%20flowchart/method%202/flowchart.bmp)

## method 3 workflow

![image](https://github.com/FarisAlmutairi305/EpicConcepts305/raw/main/directory%20structure%20as%20flowchart/method%203/flowchart.bmp)

## method 4 workflow

![image](https://github.com/FarisAlmutairi305/EpicConcepts305/raw/main/directory%20structure%20as%20flowchart/method%204/flowchart.bmp)
