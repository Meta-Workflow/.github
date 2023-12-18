# Meta-Workflow

This project's goal is to create the best workflow by combining open-source tools.

## Structure

Repositories are used to support different parts of the workflow. They are made to be modular such that any part of the workflow can be swapped with ease.

There are X different types of workflow component:
* Meta
* Application
* Tool
* Testing
* Version Control
* Documentation
* IDE

The workflow uses a bottom-up approach, meaning the lower level components do not depend on the higher-level components, but the higher-level components depend on the lower-level components since it they stitch them together.

Some components overlap, but another goal of this project is to ensure this overlap is handled smoothly.

### Meta
This component is the top-level that brings the pipeline to life. It puts every stage together.

### Application
This level is for organizing a file/folder structure for a given application. For example, an FPGA application directory structure.

### Tool
These are the specialized tools for the application. For example, when a closed-source FPGA place & route tool is needed.

### Testing
This component is for all the different types of testing needed by the application. It includes unit, integration and regression testing.
Note that the testing scripts and structure is handled on the application level, and this part is about using testing tools.

### Version Control
This component is used to keep track of the code and documentation (versioning).

### IDE
A centralized environment where the full workflow can take place.



## Currently supported

### Meta
* Jenkins

### Application
* FPGA
* Embedded C
* Embedded C++

### Tool
* Vivado
* Vitis
* STM32CubeIDE

### Testing
* TODO

### Version Control
* Git

### Documentation
* TODO

### IDE
* VSCode
