# Copilot instructions for this LaTeX CV project

Treat this repository as a maintainable software project, not a one-off document. Keep the CV modular, reusable, and easy to tailor for different roles.

## Project goals
- Build a professional, ATS-friendly CV that is easy to maintain.
- Keep content separate from presentation.
- Prefer reusable abstractions over duplicated formatting.
- Keep the repository buildable and version-controlled.
- Support future variants such as backend Java, banking, or consulting CVs.

## Repository structure
- Use main.tex as the document entry point.
- Put content in sections/.
- Put reusable styling and commands in styles/.
- Keep assets in assets/.
- Keep generated output in output/.

## Editing conventions
- Keep section files focused on content rather than layout logic.
- Avoid inline formatting in section files when a reusable command already exists.
- Prefer defining reusable commands in styles/resume.sty or related style files instead of repeating raw LaTeX formatting.
- When adding new content, use the existing structure and naming conventions.
- Keep changes small and localized unless a broader refactor is clearly required.

## LaTeX and styling guidance
- Preserve ATS-friendly design choices: clear headings, strong readability, minimal graphics, and no complex tables or multi-column layouts.
- Favor standard, simple typography and whitespace over decorative effects.
- Keep the CV concise and suitable for one or two pages.
- Make styling changes in style files rather than editing content files to adjust appearance.
- If a repeated pattern appears in multiple sections, extract it into a reusable command.

## Content workflow
- Update the relevant section file for content changes, such as experience, skills, projects, or certifications.
- Only update main.tex when adding or reorganizing sections.
- Keep section content expressive but free of layout-specific implementation details.
- Preserve the existing modular build flow when adding new sections.

## Build and validation
- Ensure changes still compile successfully with the project build command.
- Prefer keeping the repository in a buildable state after each change.
- Preserve compatibility with the existing GitHub Actions workflow and LaTeX toolchain.

## Quality bar
- Favor maintainability and clarity over cleverness.
- Keep the codebase readable and well documented.
- Make changes that are easy for future maintainers to understand.
- Treat the CV as a portfolio-quality example of structured engineering work.
