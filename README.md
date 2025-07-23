# JUnit Testing Playground

A comprehensive Java repository demonstrating various JUnit testing techniques using **JUnit 4** and **JUnit Jupiter (JUnit 5)**. This project explores different testing scenarios, best practices, and advanced features of unit and integration testing in Java.

Whether you're learning JUnit or brushing up on testing patterns, this repo serves as a practical guide to writing clean, effective, and maintainable tests.

---

## Table of Contents

- [Features](#-features)
- [Test Types Covered](#-test-types-covered)
- [Project Structure](#-project-structure)

---

## Features

- Examples of **AAA Pattern (Arrange-Act-Assert)**
- **Regression Testing** and **Test Suites**
- **Assumptions** and conditional test execution
- **Assertions with AssertJ** for fluent assertions
- **Counter Tests** to validate state changes
- **Integration Tests** involving multiple components
- **JUnit Jupiter (JUnit 5)** features: nested tests, parameterized tests, lifecycle callbacks
- **Lifecycle Tests** showing setup/teardown behavior
- **System Tests** simulating end-to-end workflows
- **Calculator Application** as a running example for unit testing
- Mixed support for **JUnit 4** and **JUnit 5**

---

## Test Types Covered

| Test Type              | Description |
|------------------------|-----------|
| **AAA Test**            | Demonstrates the Arrange-Act-Assert pattern for clear test structure. |
| **Regression Test**     | Tests designed to catch bugs that reappear after fixes. |
| **Regression Test Suite** | A JUnit test suite bundling regression tests for batch execution. |
| **Assumption Test**     | Uses `assumeTrue()` etc. to conditionally run tests based on environment/runtime state. |
| **AssertJ Test**        | Leverages AssertJ for expressive, readable assertions (e.g., `assertThat(...).isEqualTo(...)`). |
| **Counter Test**        | Validates increment/decrement logic in stateful objects. |
| **Integration Test**    | Tests interactions between multiple classes/modules. |
| **JUnit Jupiter Test**  | Modern JUnit 5 tests using annotations like `@BeforeEach`, `@ParameterizedTest`, etc. |
| **Lifecycle Test**      | Shows the order and usage of lifecycle methods (`@BeforeAll`, `@AfterEach`, etc.). |
| **System Test**         | High-level test mimicking real user workflows across the application. |
| **Calculator Tests**    | Comprehensive unit tests for a simple calculator covering edge cases and operations. |

---

## Technologies Used

- **Java 17+** (or compatible version)
- **JUnit 4** (`junit:junit:4.13.2`)
- **JUnit Jupiter (JUnit 5)** (`org.junit.jupiter:*`)
- **Maven** (for dependency management and build)
- **AssertJ** (`org.assertj:assertj-core`) – Fluent assertions
- **Maven Surefire Plugin** – For running tests

---

## 🗂 Project Structure
```
src/
├── main/
│ └── java/
│ └── com/example/
│ ├── calculator/
│ │ └── Calculator.java
│ └── service/
│ └── CounterService.java
│
└── test/
└── java/
└── com/example/
├── aaa/
├── regression/
├── integration/
├── system/
├── assumptions/
├── assertj/
├── jupiter/
├── lifecycle/
└── suites/
└── RegressionTestSuite.java
```
Each folder contains relevant test classes demonstrating the specific concept.

---

## How to Run Tests

### Prerequisites
- JDK 17 or higher
- Apache Maven

### Steps

1. Clone the repository:
```bash
git clone https://github.com/JoshFerns2005/junit_test.git 
cd junit_test
```
2. Build and run all tests:
```
mvn test
```

# Acknowledgments
JUnit Team – junit.org
AssertJ Community – assertj.github.io
Inspired by best practices from Effective Unit Testing and Growing Object-Oriented Software, Guided by Tests
