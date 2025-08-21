# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository contains an Espanso configuration file (`myBaseMatches.yml`) that defines text expansion shortcuts for development workflows. Espanso is a cross-platform text expander that replaces typed triggers with expanded text.

## File Structure

- `myBaseMatches.yml`: Main Espanso configuration file containing text expansion rules organized into categories:
  - CSS shortcuts (e.g., `/css*` expands to CSS reset)
  - Claude AI interaction shortcuts (e.g., `*Ftbl` for "in the format of a table")
  - Git command shortcuts (e.g., `-gc` expands to "git commit -m '$|$'")
  - Common word abbreviations (e.g., `/curr` expands to "currently")
  - React/Frontend development shortcuts (e.g., `***form` expands to a complete form template)
  - NPM command shortcuts (e.g., `/ill` expands to "npm install")

## Configuration Format

The YAML file follows Espanso's match configuration format:
- `trigger`: The text that triggers the expansion
- `replace`: The text that replaces the trigger
- `$|$` indicates cursor position after expansion

## Development Notes

- This is a configuration file, not executable code
- Changes should maintain YAML syntax and Espanso match format
- Test expansions work correctly in Espanso after modifications
- Categories are organized with comment headers for easy navigation