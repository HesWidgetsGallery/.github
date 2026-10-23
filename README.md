# HesWidgetsGallery organization community health files

This directory is the source for the shared community files used by the
[HesWidgetsGallery](https://github.com/HesWidgetsGallery) organization.

The organization profile lives in [`profile/README.md`](profile/README.md).
The files in this repository are intentionally repository-agnostic so they can
be reused by Qt/C++ projects across the organization.

## What is included?

- a bilingual organization profile;
- contribution, support, security, and code-of-conduct guidance;
- issue forms for bug reports and feature requests;
- a pull-request checklist and a shared `CODEOWNERS` policy;
- Dependabot configuration for GitHub Actions and the repository ecosystem;
- a lightweight GitHub Actions workflow that validates the community files.

When a project needs a more specific rule, add it to that project rather than
changing the organization defaults silently. Keep links and supported Qt
versions up to date when repositories move.
