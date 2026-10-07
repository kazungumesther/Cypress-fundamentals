# Cypress Automation Fundamentals Assignment

A structured end-to-end (E2E) test automation project built using the **Cypress** framework. This repository contains a series of test suites designed to practice, validate, and document fundamental automation engineering patterns, concluding with an integrated mini-project.

## What I Learned & Implemented

### 1. Test Architecture & Hooks
*   **Test Organization:** Structured tests logically using `describe()` blocks for test suites and `it()` blocks for atomic test cases.
*   **Lifecycle Hooks:** Implemented `before()`, `beforeEach()`, `after()`, and `afterEach()` hooks to establish reliable test states, handle preconditions, and execute clean tear-down procedures.

### 2. Assertions & Validations
*   Used both implicit assertions (`should()`, `and()`) and explicit assertions (`expect()`) to build strict validation checkpoints.
*   Verified element existence, UI visibility, precise text matches, input values, and specific HTML DOM attributes.

### 3. Core Cypress Commands & Interactions
*   Simulated realistic user journeys using core commands: `cy.visit()`, `cy.get()`, `cy.type()`, `cy.click()`, `cy.clear()`, and `cy.select()`.
*   Handled scrolling actions using `cy.scrollIntoView()` to unlock lazy-loaded elements on long webpages.

### 4. Robust Locator Strategies
*   Traversed and selected targeted elements using specialized traversal commands: `.find()`, `.parent()`, `.children()`, `.closest()`, `.first()`, `.last()`, `.eq()`, and `.within()`.
*   Prioritized stable identifiers like custom `data-cy` attributes and `id` properties over long, fragile CSS selectors to prevent flaky tests.

### 5. Advanced UI Element Interactions
*   **Web Forms:** Automated interactive input fields, hidden password targets, checkboxes, radio selections, multi-select dropdown menus, and validation messages upon form submission.
*   **Data Tables:** Parsed dynamic grids to count columns and rows, read inner index data, and directly trigger buttons nested inside specific table rows.
*   **Browser & OS Simulation:** Tested native browser alerts, confirmation boxes, window reloads, and custom keyboard keystrokes (`Enter`, `Escape`, `Backspace`, arrow keys).
*   **File Uploads:** Integrated file handling plugins to upload documents seamlessly through target input forms.

### 6. Capstone Mini-Project
*   Combined all the independent automation skills into a single, cohesive end-to-end test script.
*   Modeled a real-world user workflow requiring asynchronous steps, continuous state management, complex assertions, and layered structural hooks.

---

## Directory Layout

```text
cypress-fundamental-assignment/
├── cypress/
│   ├── e2e/               # Test suites covering specific features
│   ├── fixtures/          # Mock data files (JSON)
│   └── support/           # Custom commands and global configuration configurations
├── node_modules/          # Local npm dependencies
├── cypress.config.js      # Global Cypress configuration configuration file
├── package.json           # Project manifest and execution script parameters
└── README.md              # Project documentation
```

---

## Getting Started

### Prerequisites
Make sure you have [Node.js](https://nodejs.org) installed locally.

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com
   cd cypress-fundamental-assignment
   ```

2. Install the necessary project dependencies:
   ```bash
   npm install
   ```

### Running the Tests

You can run the automation tests using either the interactive runner or headless command-line interface mode:

*   **Open Cypress Test Runner (UI Mode):**
    ```bash
    npx cypress open
    ```
*   **Run All Tests (Headless Mode):**
    ```bash
    npx cypress run
    ```
