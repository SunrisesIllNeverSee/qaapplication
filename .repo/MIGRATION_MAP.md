# Migration Map — qaapplication

**Installed:** 2026-08-19
**Mode:** migrate
**Profile:** group

## Existing structure preserved

All existing root directories declared in `allowed_root_dirs_extra`:
- `01-inbox/` through `08-submitted/` — sequential numbered pipeline lanes
- `snapshots/` — pipeline snapshots (added to artifact_roots)
- `src/` — source code

All existing root files declared in `allowed_root_files_extra`:
- `_product.md`, `audit-log.md`, `tracker.md` — pipeline metadata

## Canon context

- Authority role: `implementation`
- Canon contexts: `moses`
- Authority owner: `search_authority`

## Migration steps (before enforce)

1. [ ] Run `repo_check.py --ci` until clean (currently clean)
2. [ ] Verify GitHub ruleset application (solo-fast)
3. [ ] Switch REPO.yaml mode from `migrate` → `enforce`

## Enforce readiness

Ready after ruleset verification — no structural defects.
