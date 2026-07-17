# Founder Intel (bring-your-own-AI edition)

Every program operator gets the same question from funders and boards: "What happened to your founders?" Almost nobody has a good answer, because tracking alumni is tedious and it always loses to this week's fires.

This pack turns that chore into a one-hour AI run. You give your AI this folder and your alumni roster; it scans the public web for what your founders went on to do (companies still alive, funding raised, press, launches, wins you never heard about) and hands you a report you can put in front of a funder.

## What you need

1. **An AI that can browse the web and read files.** Claude Code is what we built this with; any capable assistant with web search and file access works.
2. **Your roster as a CSV.** See `roster-template.csv` for the columns. More columns means better intel, but the scan runs with whatever you have, down to bare names.

## Quick start

1. Put your roster in this folder as `roster.csv`.
2. Open your AI in this folder and paste the prompt from `START-PROMPT.md`.
3. Read the report it produces. Spot-check every WIN by clicking its source link before you show the report to anyone.

## The honesty rules (read this part)

This pack is built around one fear: a report that says a founder raised money when they didn't, shown to a funder. So the protocol is strict about identity. Your AI is instructed to never attribute a finding to a founder without two independent matching anchors, to mark weak matches UNVERIFIED instead of guessing, and to capture a source URL for every win at the moment it's found. **A finding without a clickable source is not a finding.** If your report contains WINs with no links, the run went wrong; don't use it.

The scan reports what it finds with dates, including wins that predate your program. You decide what counts. That's an operator judgment, and no part of this pack makes it for you.

## Repeat runs

Keep the report the AI writes. Next quarter, run the same prompt again; the protocol tells the AI to read the previous report first and surface only what's new.

---

Built by [ELEDA](https://joineleda.org), the Entrepreneur-Led Economic Development Association, from the system we run on our own cohorts. If you'd rather we run it for you: [request access](mailto:cam@joineleda.org?subject=Founder%20Intel%20access).
