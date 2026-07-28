# MustDo

A dark-themed personal dashboard for tasks, goals, nutrition, training, and daily wellness logs, all under one login.

<!-- TODO: add a screenshot or gif of the dashboard here -->

## What It Does

MustDo started as a todo list and grew into a small health-and-productivity tracker: one-off and recurring tasks, goals bucketed by timeframe, a nutrition and meal log, workout tracking with progressive overload, and daily body-weight, sleep, and mood logs.
A dashboard ties it together with streaks and trend sparklines.
It's built to stay boring on purpose - a single Go binary, plain HTML/CSS/JS with no build step, and Supabase for the database and auth.

## Tech Stack

- Go
- PostgreSQL (Supabase)
- Supabase Auth
- HTML / CSS / JS (no build step)
- Resend (email reminders)

## Install and Run

Requires Docker and the Supabase CLI.

```bash
supabase start                  # local Postgres + Auth stack
cp .env.example .env            # fill in values printed by `supabase start`
docker compose up --build
```

Open `http://localhost:8090`.
