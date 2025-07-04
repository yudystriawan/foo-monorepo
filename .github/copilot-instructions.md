# GitHub Copilot Instructions

## Package Management

This is a Yarn-based monorepo project. When installing new dependencies:

1. Always use `yarn` instead of `npm` for package installations
2. For workspace-specific dependencies, use `yarn workspace <workspace-name> add <package-name>`
3. For dev dependencies in a workspace, use `yarn workspace <workspace-name> add -D <package-name>`
4. For root-level dependencies, use `yarn add -W <package-name>`
5. For root-level dev dependencies, use `yarn add -W -D <package-name>`

## NX Commands

This project uses NX for building, testing, and linting. Always use NX commands for these operations:

1. To build a project: `nx build <project-name>`
2. To run tests: `nx test <project-name>`
3. To run e2e tests: `nx e2e <project-name>`
4. To lint a project: `nx lint <project-name>`
5. To serve an application: `nx serve <project-name>`
6. To run commands across multiple projects: `nx run-many --target=<command> --projects=<project-list>`
7. To run commands on affected projects: `nx affected:<command>`

## General Guidelines

- Follow the existing code style and patterns
- Use TypeScript for all new code
- Use kebab-case for file names (e.g., `user-profile.component.ts`)
- Use CamelCase for class names (e.g., `UserProfileComponent`)
