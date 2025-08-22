# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository contains a modular Espanso configuration system that defines text expansion shortcuts for development workflows. Espanso is a cross-platform text expander that replaces typed triggers with expanded text.

## Architecture

The configuration uses a modular architecture with `BASEMATCHES.yml` as the main entry point that imports category-specific match files:

- `BASEMATCHES.yml`: Main configuration file that imports all other match files
- `claude_match.yml`: Claude AI interaction shortcuts and formatting requests
- `git_match.yml`: Git command shortcuts and workflows
- `css_match.yml`: CSS-related text expansions
- `react_match.yml`: React/Frontend development shortcuts
- `npm_match.yml`: NPM command shortcuts
- `common_words_match.yml`: Common word abbreviations
- `system_match.yml`: System-level shortcuts
- `navigation_match.yml`: Navigation-related shortcuts
- `terminal_match.yml`: Terminal command shortcuts

## Configuration Format

All YAML files follow Espanso's match configuration format:
- `trigger`: The text that triggers the expansion
- `replace`: The text that replaces the trigger
- `$|$` indicates cursor position after expansion
- Categories are organized with comment headers for easy navigation

## Development Notes

- This is a configuration system, not executable code
- Changes should maintain YAML syntax and Espanso match format
- Test expansions work correctly in Espanso after modifications
- When adding new matches, place them in the appropriate category file
- The modular structure allows for easier maintenance and organization of triggers by domain