# Test Framework

This repository contains a Cypress test framework that employs the Page Object Model (POM) design pattern for enhanced maintainability and scalability of your test automation efforts. The framework is built using **Cypress version 12.14.0**.

## Repository Link

You can access the repository [here](https://github.com/Razib-R75/WSD_Assignment.git).


## Prerequisites

Before running the tests, ensure that you have the following installed:

- Node.js (version 14 or higher)
- npm (comes with Node.js)

## Installation

Follow these steps to set up the project:

1. Clone the repository:

   ```bash
   git clone https://github.com/Razib-R75/WSD_Assignment.git
   ```

2. Navigate to the project directory:

   ```bash
   cd WSD_Assignment
   ```

3. Initialize npm in the project:

   ```bash
   npm init -y
   ```

4. Install Cypress version 12.14.0:

   ```bash
   npm install cypress@12.14.0
   ```

## Running the Tests

To run the tests, you can use the following command:

1. Open the Cypress Test Runner:

   ```bash
   npx cypress open
   ```

   This command will launch the Cypress Test Runner, where you can select and run your tests interactively.

2. Alternatively, to run tests in headless mode, use:

   ```bash
   npx cypress run
   ```

   This command will execute all the tests in a headless browser environment.


### Page Object Model (POM)

Each page of the application is represented as a class within the `/pages` directory. Each class contains:

- Selectors for elements on the page
- Methods for actions that can be performed on those elements
- Assertions relevant to that page

This structure promotes reusability and a clear separation of concerns.

## Design Choices

1. **Page Object Model**: Using POM helps in creating a clear structure for the test code, making it easier to maintain. Changes in the UI require updates only in the page object classes, not throughout all test scripts.

2. **Cypress**: Cypress is chosen for its fast execution and powerful capabilities for end-to-end testing. It also provides an intuitive interface for debugging tests, which enhances developer productivity.

3. **Separation of Concerns**: The framework separates test logic from the implementation details, making it easier to read and understand. Test cases focus on user actions and validations rather than the mechanics of the application.

4. **Headless Mode**: Running tests in headless mode improves CI/CD pipeline performance, enabling faster feedback and integration.

## Contributing

Contributions are welcome! If you’d like to contribute to the project, please fork the repository and create a pull request. Make sure to update the README if you add new features or change existing ones.

