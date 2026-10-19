# morning-briefing-site

The public morning briefing. **This repo is generated — do not edit by hand.**

Contents are pushed every morning by the 5am job in
[`morning-briefing`](https://github.com/whalexander822/morning-briefing)
(`inbox-digest/publish.py`), which builds a sanitised copy of the digest and
commits it here. GitHub Pages serves the result.

## What is published

- News (newsletters) — subjects and links
- Jobs — listings and links
- Counts of what was processed
- The Raindrop shelf — saved repos, videos, training and ideas, as
  title + link + bucket

## What is never published

- `private.html` and `review.html` — direct and unclassified mail
- Email sender names
- Email snippets
- Raindrop notes, excerpts and cover images
- Any vote data

The sanitiser lives in `morning-briefing` → `inbox-digest/src/publish.py`.
The rules are enforced there, not by convention.

## Voting

There is no server here. Each vote button opens a pre-filled GitHub issue in
the private [`digest-votes`](https://github.com/whalexander822/digest-votes)
repo, which the 5am job reads and records.
