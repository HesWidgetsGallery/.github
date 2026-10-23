# Contributing to HesWidgetsGallery

Thank you for helping improve the HesWidgetsGallery projects. This guide
describes the shared expectations; a project README or `AGENTS.md` may add
more specific requirements.

## Before you start

- Search existing issues and pull requests to avoid duplicate work.
- Read the target repository's README, build guide, and license.
- For a larger change, open an issue first so the API and scope can be agreed
  on before implementation.
- Do not include secrets, generated credentials, private assets, or unrelated
  formatting changes in a pull request.

## Development workflow

1. Fork the repository or create a branch from the default branch.
2. Use a descriptive branch name, for example `fix/combo-box-focus` or
   `feat/navigation-view`.
3. Initialize documented submodules and configure the required Qt version and
   compiler.
4. Make the smallest coherent change. Preserve public API compatibility unless
   the pull request explicitly documents a breaking change.
5. Add or update tests and documentation for user-visible behavior.
6. Run the repository's formatter, build, and test commands locally.
7. Open a pull request using the template and explain what changed, why, and
   how it was verified.

## Qt/C++ expectations

- Follow the target repository's `.clang-format` and naming conventions.
- Prefer Qt types and ownership patterns that match the surrounding code.
- Keep UI behavior accessible from keyboard and high-contrast themes where
  applicable.
- Avoid blocking the GUI thread and document platform-specific behavior.
- Keep generated resources reproducible; include the generation command when a
  generated file must be committed.

## Commit and pull-request guidance

Use concise, imperative commit subjects. A conventional prefix such as
`fix:`, `feat:`, `docs:`, `test:`, or `refactor:` is encouraged when the
repository already uses it. Keep unrelated commits separate.

Pull requests should:

- describe the user-visible result;
- link related issues;
- include tests or a clear reason they are not applicable;
- mention supported platforms and Qt versions;
- include screenshots or a short recording for visual changes;
- call out API, behavior, migration, or license implications.

Maintainers may ask for a smaller scope, additional tests, or documentation
before merging. Reviews focus on correctness, maintainability, accessibility,
and consistency with the existing project.

## Reporting security issues

Do not open a public issue for a suspected vulnerability. Follow the process in
the [security policy](SECURITY.md).
