# Founder Intel (bring-your-own-AI edition)

People who support founders for a living get measured on the success of their founders. Tracking that success is the hard part: Google Alerts don't work, and following everyone on LinkedIn isn't enough. Wins happen in other cities, on other platforms, years after your program ends.

This pack turns that chore into a one-hour AI run. You give your AI this folder and your alumni roster; it scans the public web for what your founders went on to do (companies still alive, funding raised, press, launches, wins you never heard about) and hands you a report you can put in front of a funder.

| ![A plain spreadsheet of alumni names, ventures, and cities](assets/roster-in.png) | ![A Founder Intel report: wins, watch items, and statuses, each with a source](assets/report-out.png) |
|:--:|:--:|
| **1. You send your alumni roster** | **2. You get back a report you can hand a funder** |


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

**Treat the report as a tip sheet, not gospel.** If you've graduated 400 founders, you were never going to Google all of them. Founder Intel's job is to point at the handful worth a closer look: the one who quietly had an exit, the one whose company just did something awesome. Before you repeat any finding, take that closer look yourself. Open the source link, check their LinkedIn, run a search of your own. Verifying is your half of the work, and it's minutes per founder instead of hours across the whole roster.

## Fair warning: this is early

We use this system on our own cohorts and it works, but the self-serve version is young and there's some artfulness in getting it set up well: roster quality matters, AI models vary, and the first run usually teaches you something about your own data. If you hit friction, that's expected, and we want to hear about it (open an issue or email us). If you'd rather skip the setup entirely, [we'll run it for you](mailto:cam@joineleda.org?subject=Founder%20Intel%20access).

## Repeat runs

Keep the report the AI writes. Next quarter, run the same prompt again; the protocol tells the AI to read the previous report first and surface only what's new.

---

Built by [ELEDA](https://joineleda.org), the Entrepreneur-Led Economic Development Association, from the system we run on our own cohorts. If you'd rather we run it for you: [request access](mailto:cam@joineleda.org?subject=Founder%20Intel%20access).
