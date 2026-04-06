# Orchestration

This directory manages task tracking and project coordination.

## Files

- `task_backlog.jsonl` -- Machine-readable task backlog (one JSON object per line)
- `tasklist.md` -- Human-readable task console

## Backlog Format

Each line in `task_backlog.jsonl` is a JSON object:

```json
{
  "id": "unique-task-id",
  "description": "What needs to be done",
  "status": "pending",
  "priority": "P1",
  "isc": [
    "Criterion 1 | Verify: method",
    "Criterion 2 | Verify: method"
  ],
  "created": "2026-01-01T00:00:00Z"
}
```

## Status Values

- `pending` -- Not started
- `in_progress` -- Currently being worked on
- `done` -- Completed and verified
- `failed` -- Attempted but did not pass ISC verification
- `deferred` -- Postponed to a future phase

## Adding Tasks

Use `/backlog <description>` to add tasks from any session. The skill handles formatting and deduplication.
