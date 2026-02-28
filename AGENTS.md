```markdown
# AGENTS.md - AI Coding Agent Guidelines

These guidelines are designed to ensure the production of high-quality, maintainable, and robust AI coding agents. Adherence to these principles is mandatory for all development activities within this repository.

## 1. DRY (Don't Repeat Yourself)

*   **Avoid duplication of logic:** Implement reusable components and functions that handle core functionality across multiple agents.
*   **Parameterization:**  Use parameterized inputs and outputs to create adaptable agents.
*   **Abstraction:**  Define abstract interfaces for common operations and expose them through concrete implementations.
*   **Single Responsibility Principle:** Each agent should have a single, clearly defined purpose.

## 2. KISS (Keep It Simple, Stupid)

*   **Minimalism:** Strive for the simplest possible solution that effectively achieves the required functionality.
*   **Readability:**  Code should be easy to understand and follow.  Use clear variable names and comments where necessary.
*   **Efficiency:** Prioritize efficient algorithms and data structures.
*   **Single Responsibility:**  Each function or class should perform one specific task.

## 3. SOLID Principles

*   **Single Responsibility Principle:**  Each class or module should have one primary responsibility.
*   **Open/Closed Principle:**  The system should be extensible through new classes without modifying existing code.  (Limited use of dependency injection.)
*   **Liskov Substitution Principle:**  Replacing a base class with its derived class should not affect the correctness of the program.
*   **Interface Segregation Principle:**  Clients shouldn’t be forced to depend on methods they don’t use.
*   **Dependency Inversion Principle:**  High-level modules (like agents) should not depend on low-level modules (like specific data structures).

## 4. YAGNI (You Aren’t Gonna Need It)

*   **Avoid premature optimization:**  Focus on delivering working code first, then optimize later when performance becomes critical.
*   **Assume no future requirements:**  The system should be designed to be adaptable to future needs.
*   **Prioritize functionality over performance:**  Balance performance considerations with the overall goal of building a functional agent.

## 5. Development Workflow & Code Quality

*   **Unit Testing:** All code must be thoroughly unit tested.
*   **Test Coverage:** Achieve 80% minimum test coverage for all code. Automated tests should be implemented and executed regularly.
*   **Code Reviews:**  All code changes should be reviewed by at least two developers.
*   **Coding Standards:** Follow established coding style guidelines (documented in a separate file, `coding_standards.md`).
*   **Documentation:**  Provide clear and concise documentation for all agents and functions.
*   **Version Control:**  Use Git for version control.
*   **Static Analysis:** Utilize a static analysis tool (e.g., ESLint, pylint) to enforce coding standards and identify potential issues.
*   **Error Handling:** Implement robust error handling and logging.
*   **Parameter Validation:** Validate all inputs to prevent unexpected behavior and security vulnerabilities.
*   **Limit Code Length:**  Maximum code length: 180 lines.

## 6. File Structure & Organization

*   **`src/agents/`:** Contains the core agent logic.
*   **`src/data/`:** Contains data-related functions and classes.
*   **`src/utils/`:** Contains utility functions and classes (e.g., string manipulation, date formatting).
*   **`src/config/`:**  Contains configuration files for agents.
*   **`src/tests/`:**  Contains unit tests for all agents.
*   **`README.md`:**  Provide a comprehensive overview of the project, including setup instructions, usage examples, and contributing guidelines.

## 7.  Specific File Templates (Example)

*   `agent.py`:  Basic agent definition.
*   `data_manager.py`:  Data management functions.
*   `unit_test.py`:  Unit test framework.
*   `config.py`: Configuration management.

## 8.  Reporting & Metrics

*   **Code Coverage Reports:** Generate automated code coverage reports for each agent.
*   **Test Execution Reports:** Track test execution status and results.
*   **Linting Reports:**  Monitor linting rules and identify potential issues.

```