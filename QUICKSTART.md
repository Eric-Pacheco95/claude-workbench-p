# Quickstart -- Your First 5 Sessions

## Prerequisites

- Claude Code CLI installed (`claude` command available)
- Git initialized (this repo)

## Session 1: Extract Wisdom

Feed Claude some content and capture the value.

```
claude
> /extract-wisdom <paste an article, transcript, or essay>
```

Look at the output: IDEAS, INSIGHTS, QUOTES, HABITS, REFERENCES, RECOMMENDATIONS. This is what every piece of content you consume can produce.

## Session 2: Capture a Learning Signal

After doing any meaningful work, capture what you learned.

```
> /learning-capture
```

This creates a signal file in `memory/learning/signals/`. Check it:

```
ls memory/learning/signals/
```

Signals are raw observations -- things you noticed, mistakes you made, patterns that worked.

## Session 3: Synthesize Your Signals

Once you have 5+ signals, synthesize them into themes.

```
> /synthesize-signals
```

This reads your signals and produces a synthesis document in `memory/learning/synthesis/`. Themes emerge that you didn't plan.

## Session 4: Build Something with the Full Pipeline

Try the build pipeline on a real project:

```
> /create-prd Build a CLI tool that converts markdown notes to flashcards
> /implement-prd
> /quality-gate
> /learning-capture
```

Each skill hands off to the next. The PRD defines ISC; implement-prd builds against them; quality-gate validates; learning-capture records what you learned.

## Session 5: Update Your Steering Rules

Now that you have signals and synthesis, update your steering rules.

```
> /update-steering-rules
```

This analyzes your learning history and proposes new rules for CLAUDE.md. You approve each one. These rules shape every future session.

## What's Next?

- Run `/help` to see all 34 skills grouped by workflow stage
- Try `/research <topic>` for web research with structured output
- Try `/red-team <idea>` to stress-test any plan or proposal
- Try `/first-principles <question>` for deep analytical thinking
- Read `CLAUDE.md` to understand the full system architecture
- Add your own skills with `/create-pattern`
