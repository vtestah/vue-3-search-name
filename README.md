  # Vue 3 Name Search 🔍

  A name search component with suggestions, built with Vue 3 and TypeScript. Perfect for projects requiring autocomplete search functionality.

  <img width="658" height="348" alt="image" src="https://github.com/user-attachments/assets/56d47ccb-8f5e-4618-ba3c-c07bddd48b6a" />

  ## Tech Stack

  - **Vue 3** (Composition API)
  - **TypeScript**
  - **Vite** (Bbild and development)
  - **SCSS** (Styling framework)
  - **Vitest** (Testing)
  - **ESLint**, **Prettier**, **Stylelint** (Linting and formatting)
  - **Husky**, **lint-staged**, **commitlint**, **Commitizen** (Commit checks and formatting)

  ## Description

  This component provides functionality for name search with suggestions. The user types into the search field, and the component automatically displays matching results that can be selected using the mouse or keyboard.

  Features:
  - Highlighting of matched results.
  - Support for navigation keys (`ArrowUp`, `ArrowDown`, `Enter`, `Escape`).
  - **Debounce** functionality to improve performance.
  - A responsive and accessible interface for screen readers.

  ## Demo

  You can see an example of the component in action in the [available demo](https://vofronte.github.io/vue-3-search-name/).

  ## Installation and Setup

  ### 1. Make sure you have the following tools installed:
  - [Node.js](https://nodejs.org/en/download/) (version 18 or above)
  - [Yarn](https://yarnpkg.com/getting-started/install) (or npm/pnpm)

  ### 2. Clone the repository and install dependencies:

  ```bash
  git clone https://github.com/vofronte/vue-3-search-name.git
  cd vue-3-search-name
  yarn install
  ````

  ### 3. Start the dev server:

  ```bash
  yarn dev
  ```

  The project will be available at [http://localhost:5173](http://localhost:5173).

  ### 4. For testing:

  Run the tests:

  ```bash
  yarn test
  ```

  ### 5. For linting and formatting:

  * Linting (ESLint + Stylelint):

    ```bash
    yarn lint
    ```

  * Formatting (Prettier):

    ```bash
    yarn format
    ```

  ### 6. For commits, use:

  ```bash
  yarn commit
  ```

  This script runs Commitizen and helps you create commits with the correct format.

  ### 7. To build the project:

  ```bash
  yarn build
  ```

  ## Using the Component

  ```vue
  <NameSearch @select="handleNameSelect" />
  ```

  Example handler for name selection:

  ```ts
  const handleNameSelect = (name: string | null) => {
    console.log('Selected name:', name)
  }
  ```

  ### Component Props:

  * `inputId`: A unique identifier for the input field.
  * `names`: An array of names to search.
  * `debounceMs`: Debounce delay in milliseconds before performing the search.

  ## Component Testing

  **Vitest** is used for testing. You can run the tests using the `yarn test` command.
