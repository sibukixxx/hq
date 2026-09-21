# hq

Repository-specific work follows the tracked README/configuration. No stable root build contract was verified during this migration, so this file intentionally avoids guessed commands.

## Commands
- Inspect `README.md`, root manifests, and CI before editing; use the commands already defined there.

## Shared rules
- Preserve the current runtime/module boundaries in tracked configuration.
- Do not commit secrets, local environment state, vendor directories, or generated build output unless intentionally tracked.
- Do not claim validation that was not run.

## Change-dependent checks
- Code: run the existing test/build command covering the changed area.
- Config/dependencies: validate the matching manifest/lockfile and CI path.

## Done
- Requested changes are in tracked source.
- Relevant existing checks pass, or exact unrun/failed checks are reported.
