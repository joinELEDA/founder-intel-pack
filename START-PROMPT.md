# Paste this prompt into your AI

Copy everything below the line into your AI assistant, opened in this folder.

---

Read PROTOCOL.md in this folder and follow it exactly. Then read roster.csv.

Scan every founder on the roster per the protocol's search steps. Hard rules, non-negotiable:

- Two-anchor rule for identity: never attribute a finding to a founder without two independent matching anchors. When in doubt, UNVERIFIED or omit. Never guess.
- Every founder on the roster gets exactly one entry with a status (WIN, WATCH, QUIET, PENDING, or UNVERIFIED). No silent drops.
- Every WIN carries a source URL captured at the moment you found it.
- Verify "site live" claims by actually fetching the domain, not by trusting a search snippet.
- Role claims sourced only from third-party bio, directory, or profile pages (data brokers, Crunchbase, event-speaker bios, course-instructor bios) are UNVERIFIED. Stating a role as fact requires the person's own live profile, their company's site, or an original dated announcement.
- A changed state since intake (new role, new venture, promotion, shipped product) is a WIN with found_date "as of [today]". QUIET is only for unchanged persistence. But verify it IS a change: a role already held at intake, or one whose start date you can't place after the program, is WATCH or QUIET, not WIN.
- Report wins that predate the program with their dates; the operator decides what counts.

If a report file from a previous run exists in this folder, read it first and report only what's new.

When done, write the report as `founder-intel-report-[today's date].md` in this folder, using the structure in report-example.md. Then give me a one-line summary: founders scanned, WIN / WATCH / QUIET / PENDING / UNVERIFIED counts, and the report file path. Before finishing, verify the acceptance bar in PROTOCOL.md and tell me plainly if the run failed any part of it.
