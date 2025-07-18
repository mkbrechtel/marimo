# Marimo MCP Development Repository Structure

This repository contains the development work for adding MCP (Model Context Protocol) support to Marimo.

## Repository Structure

- **Main Directory (`.`)**: Contains the project proposal and feature specifications
  - `README.md`: Project overview and proposal
  - `CLAUDE.md`: Coding agent instructions
  - `feature-*.md`: Individual feature specifications

- **Worktree (`./marimo/`)**: Contains the actual Marimo codebase
  - This is a git worktree of the main Marimo repository
  - Currently on branch: `marimo/feature/mcp`

## Development Workflow

1. **All code changes must be made in the worktree** (`./marimo/`)
2. **Feature branches**: We develop on `marimo/feature/mcp` branch
3. **Commits**: All commits should be made within the worktree directory
4. **Upstream tracking**: The `marimo/main` branch tracks `upstream/main` from the official Marimo repository

## Important Notes

- Never commit changes in the root directory when working on Marimo code
- Always `cd ./marimo` before making code changes
- The feature branch `marimo/feature/mcp` is where all MCP-related development happens
- Use `git status` within the worktree to check the state of your changes

## Branch Structure

- `main`: Contains the project proposal and documentation
- `marimo/main`: Tracks the upstream Marimo main branch
- `marimo/feature/mcp`: Feature branch for MCP development (in worktree)
