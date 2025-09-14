# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview
This is a LaTeX-based resume repository using the moderncv document class. The main source file is `resume.tex` which compiles to `resume.pdf`.

## Commands
- **Build resume**: `pdflatex resume.tex`
- **Clean build artifacts**: `rm *.aux *.log *.out *.synctex.gz` (or let git ignore handle them)

## Architecture
- `resume.tex`: Main LaTeX source file containing resume content
- Uses moderncv document class with casual theme
- Includes commented sections for optional content (skills, previous experience, projects)
- Generated artifacts (aux, log, out, synctex.gz) are git-ignored
- PDF output is tracked in git

## Development Notes
- The resume uses custom commands like `\hlink{}` for consistent link formatting
- Large sections are commented out using `\begin{comment}...\end{comment}` blocks
- Personal information is defined at the top using moderncv commands
- Line spacing is set to 1.5x using `\onehalfspacing`