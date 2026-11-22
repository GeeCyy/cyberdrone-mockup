# Local Project Boundaries & Constraints

## 1. SCOPE & SAFETY BOUNDARIES
* DIRECTORY LOCK: You are restricted entirely to this directory. Do not navigate up or alter external workspaces.
* CONTEXT DRIFT: Break complex tasks into small, isolated sub-steps. Pause and request explicit user approval before executing multi-file parallel agent tasks.
* AMBIGUITY TRIGGER: If a feature request lacks explicit data types, business logic, or clear visual requirements, you MUST pause and ask the user for clarification before generating files.
* LOOP PREVENTION: If a specific test or build command fails 3 times consecutively with the same or similar error output, you MUST halt execution, summarize what you attempted, and wait for human intervention.

## 2. EXECUTION WORKFLOW
* EXECUTION ORDER: When given a task, follow this exact sequence:
  1. Explore the relevant files using grep or view tools.
  2. Present a brief 3-bullet plan to the user.
  3. Wait for explicit user confirmation before writing any code. No exceptions.
  4. Write the code.
* VERIFICATION: Never mark a task as complete based on code compilation alone. You MUST execute the build command (`npm run build`) and verify that the build succeeds with zero errors before confirming completion.

## 3. DEVELOPMENT COMMANDS
* PACKAGE MANAGER: Check `package.json` to confirm the correct package manager (`npm`, `pnpm`, or `yarn`) before running any command. Never assume.
* Build project: `npm run build`
* Run linter: `npm run lint`
* Execute test suite: `npm test`
* Single file test: `npm test -- <path_to_file>`

## 4. PROJECT MAP & ARCHITECTURE
* Core Source: `src/` (All main execution logic lives here)
* Shared Utilities: `src/utils/` (Check here for existing helpers before writing redundant utilities)
* Production Builds: `dist/` (NEVER edit files inside this folder manually)

## 5. CODE STYLE & PATTERNS
* SYSTEM DESIGN: Refer to global configurations for naming conventions, styling preferences, and core language rules.
* DRY PRINCIPLE: Do not write new helper functions for date formatting, API fetching, or state management. Use the exact files located in `src/utils/`. If an adjustment is needed, modify the existing utility rather than wrapping it in a duplicate function.
