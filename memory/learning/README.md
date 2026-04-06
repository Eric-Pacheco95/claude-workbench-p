# Learning System

The learning loop is the core value engine. Every session should produce signals; signals compound into synthesis; synthesis updates steering rules.

## Directory Structure

```
memory/learning/
+-- signals/       # Raw observations from sessions (created by /learning-capture)
+-- synthesis/     # Periodic distillation (created by /synthesize-signals)
+-- failures/      # What went wrong + root cause (created by /self-heal)
```

## How It Works

1. **Capture**: Run `/learning-capture` at the end of meaningful sessions. This creates a signal file with what you observed, learned, or want to remember.

2. **Synthesize**: Once you have 5+ signals, run `/synthesize-signals`. This reads all unprocessed signals and produces a synthesis document identifying themes, patterns, and actionable insights.

3. **Steer**: Run `/update-steering-rules` to turn synthesis insights into CLAUDE.md steering rules that shape future behavior.

## Signal Format

```markdown
---
date: YYYY-MM-DD
source: session | research | failure
rating: 1-10 (how valuable is this observation?)
category: workflow | security | architecture | learning
---

What happened, what I learned, and why it matters.
```

## Tips

- Rate signals honestly. 4-6 is normal. 8+ is genuinely surprising insight. Don't inflation-rate.
- Failures are the highest-value signals. Always capture them.
- Run synthesis weekly for the first month, then biweekly as signal volume normalizes.
