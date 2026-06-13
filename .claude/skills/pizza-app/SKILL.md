```markdown
# pizza-app Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches you the core development patterns and conventions used in the `pizza-app` repository, a TypeScript React application. You'll learn how to structure files, write and organize code, and follow the project's standards for imports, exports, and testing. This guide also provides suggested commands for common workflows.

## Coding Conventions

### File Naming
- Use **camelCase** for filenames.
  - Example: `pizzaMenu.tsx`, `orderForm.ts`

### Import Style
- Use **relative imports** for modules within the project.
  - Example:
    ```typescript
    import { PizzaMenu } from './pizzaMenu';
    ```

### Export Style
- Use **named exports** for components and utilities.
  - Example:
    ```typescript
    // pizzaMenu.tsx
    export const PizzaMenu = () => { /* ... */ };
    ```

### Commit Messages
- Freeform style, sometimes with prefixes.
- Average commit message length: ~49 characters.
  - Example: `Add toppings selector to order form`

## Workflows

### Creating a New Component
**Trigger:** When adding a new UI piece or feature  
**Command:** `/new-component`

1. Create a new file using camelCase (e.g., `pizzaList.tsx`).
2. Define your component using a named export.
    ```typescript
    export const PizzaList = () => { /* ... */ };
    ```
3. Import the component where needed using a relative path.
    ```typescript
    import { PizzaList } from './pizzaList';
    ```
4. Add or update a corresponding test file (e.g., `pizzaList.test.tsx`).

### Writing a Test
**Trigger:** When adding or updating features  
**Command:** `/add-test`

1. Create a test file with the pattern `*.test.*` (e.g., `orderForm.test.tsx`).
2. Write your tests using the project's preferred testing framework (framework not detected; check existing tests for patterns).
3. Ensure tests cover all new or changed functionality.

### Committing Changes
**Trigger:** When saving progress or completing a feature  
**Command:** `/commit`

1. Write a concise, descriptive commit message (~49 characters).
2. Optionally use a prefix for clarity.
    - Example: `Fix: update pizza size options in menu`
3. Commit your changes.

## Testing Patterns

- Test files follow the `*.test.*` naming convention (e.g., `pizzaMenu.test.tsx`).
- The testing framework is not specified; review existing test files for guidance.
- Place test files alongside the components they test or in a dedicated `__tests__` directory if present.

## Commands

| Command         | Purpose                                         |
|-----------------|-------------------------------------------------|
| /new-component  | Scaffold a new React component                  |
| /add-test       | Create a new test file for a component/feature  |
| /commit         | Guide for writing and formatting commit messages |
```
