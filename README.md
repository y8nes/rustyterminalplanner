# ⟦ R.T.P ⟧ — Rusty Terminal Planner

A beautiful terminal-based daily planner with habit tracking, streaks, and a rich color theme.

**R.T.P** stands for **Rusty Terminal Planner** — built in Rust, lives in your terminal.

## Features

- **Input tasks interactively** — each gets a 1-hour time slot
- **Auto emoji** — detects task type (coding, meditation, workout, etc.)
- **Colored schedule** — see your full day laid out with time blocks
- **Weekly habit tracker** — visual grid showing streak progress
- **Task management** — mark done/skipped, add notes, track streaks
- **Daily summary** — progress bar + motivational feedback

## Requirements

- Rust (stable) — install from https://rustup.rs

## Build & Run

```bash
cd daily_planner
cargo run
```

Or build a release binary:

```bash
cargo build --release
./target/release/rtp
```

## Usage

1. Enter a start hour (e.g. `7` for 7:00 AM)
2. Type task names one by one — type `done` when finished
3. View your schedule, habit tracker, and summary
4. Use the menu to:
   - `[1]` Mark a task done
   - `[2]` Mark a task skipped
   - `[3]` Add a streak day to a habit
   - `[4]` Add a note to a task
   - `[5]` Reset a task to pending
   - `[q]` Quit

## Example Tasks

```
coding
meditation
workout
reading
journaling
```

## Dependencies

- `chrono` — date/time handling (listed in Cargo.toml)

> The visual theme uses ANSI escape codes — works best in a modern terminal (iTerm2, Alacritty, Windows Terminal, etc.)
