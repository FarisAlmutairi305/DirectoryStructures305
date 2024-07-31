# EpicConcepts305

Welcome to **EpicConcepts305**! This repository showcases an innovative approach to representing workflows and procedures using directory structures and shortcuts. The concept aims to mirro your workflow by creating folders aligned with the processes and decisions you have in your workflow. The next process is represented by creating a shortcut or `.lnk` file to provide a structured and interactive way to navigate complex processes.

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

