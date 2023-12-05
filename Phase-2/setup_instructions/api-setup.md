# Spectre API Application Setup Instructions

This document describes the steps to set up the Spectre API application in a development environment.

## Prerequisites

- Git
- Java JDK (for Java components)
- Appropriate C development tools (for C components)

## Steps

1. **Clone the Repository**:
   git clone [https://gitlab.com/spectre.app/api.git](https://gitlab.com/spectre.app/api.git)

2. **Build the Java Components**:

- Navigate to the `java` directory within the cloned repository.
- Run `./gradlew build` to build the Java components.

3. **Compile the C Components**:

- Navigate to the `c` directory.
- Use `make` or the provided build scripts to compile the C components.

4. **Running the API**:

- The specific steps to run the API will depend on how the API is designed to be launched.
- Typically, this involves running a Java `jar` file or executing a compiled C binary.

## Troubleshooting

- Ensure Java JDK and C development tools are correctly installed.
- Check for any missing dependencies or errors in the build process.
