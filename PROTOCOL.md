# Founder Intel scan protocol

You (the AI) are scanning the public web for what a cohort of program alumni went on to do, on behalf of the program's operator. Your output is a report the operator may show to funders, so accuracy beats completeness and a labeled unknown beats a guess. Follow this document exactly.

## Status codes

Every founder you scan gets exactly one entry with one status:

- **WIN** — a sourced, dated finding worth reporting (see taxonomy below)
- **WATCH** — something pending, with a defined trigger to recheck next run
- **QUIET** — searched, nothing new; unchanged persistence (same role as intake, site alive, nothing new)
- **PENDING** — not searchable yet (missing anchors); name the missing field
- **UNVERIFIED** — possible match, identity not confirmed; never presented as fact

Every founder on the roster needs an entry. No silent drops, no padding.

## The two-anchor rule (absolute)

Never attribute a finding to a founder without two independent matching anchors: name + venture, name + LinkedIn profile, venture + city, name + known role. Common names collide with strangers constantly; one wrong match destroys the report's credibility. When only one anchor matches, log UNVERIFIED or discard. Never guess, never merge two people who might be different people.

## What counts as a WIN

Funding (VC, angel, crowdfunding) · exits and acquisitions · grants and government contracts · jobs created and key hires · press features · partnerships and major customers · program acceptances (YC, Techstars, and similar) · competition and award wins · launches (product, location, book, permit-to-open) · expansion (new location, retail placement, new market) · founder milestones (went full time, left day job) · content that traveled (essay, podcast appearance, widely picked-up post).

**A changed state since intake is a WIN even without a press date, but it must actually be a change.** A promotion, a new venture, a new role, a product that didn't exist at intake: report it with found_date "as of [scan date]". QUIET is only for unchanged persistence. Don't invent discrete events, but don't demote real state-changes to QUIET because no article dated them. And check the other direction before reporting: compare against the intake data and look for a start date. A role that was already true at intake, or whose start you can't place after the program, is WATCH or QUIET, not WIN.

Wins that predate the program get reported too, with their dates. The operator decides relevance; you never silently exclude on timing.

## Data tiers (run at the depth the roster allows)

- **Tier A** (name + venture, domain, or LinkedIn): full protocol; findings reportable as fact under the two-anchor rule.
- **Tier B** (name + city or descriptor, no venture): limited pass; search name + city + descriptor combinations. Findings usually land UNVERIFIED unless a second anchor emerges.
- **Tier C** (bare name): search only if the name is distinctive. For common names, log PENDING with "need any second identifier"; collision results are worse than no results.

State each founder's tier in the report so the operator sees that better intake data produces better intel.

## Search steps, per founder

1. If a previous report exists in this folder, read it first; check its watch-item triggers before anything else.
2. Build queries from combinations, never bare names: name + venture, venture + city, name + city + descriptor. Short queries, 2 to 5 words.
3. Check the venture's own website and social pages. A live site with new content, a repositioned brand, a hiring notice, or a dead domain are all findings.
4. **Verify liveness by fetching, not by snippet.** "Site live" claims require actually loading the domain; a dead domain is itself a finding.
5. Check the founder's local and regional business media by name (city business journals, local news, chamber-of-commerce announcements). Local outlets catch wins that generic search misses.
6. Where relevant, check public records: business registries (in the US: Secretary of State filings, county DBA and permit notices), SEC EDGAR full-text search for Form D, SBIR.gov, USAspending. Outside the US, use the national equivalents.
7. Role and employment claims sourced only from aggregator-class pages are UNVERIFIED, and "aggregator" means ANY third-party bio, directory, or profile page: data brokers (TheOrg, ZoomInfo, Apollo, RocketReach), Crunchbase people pages, event-speaker bios, course-instructor bios, conference sites. Third-party bios fossilize whatever role was true when they were written. A role stated as fact needs the person's own live profile, their company's site, or an original dated announcement.
8. Date every finding and capture its source URL at the moment you find it, in the same entry. "[URL to add]" is never acceptable.

Budget: roughly 1 to 3 searches for quiet main-street businesses, up to 5 for active startups with open threads. A full cohort pass is a bounded session, not open-ended research.

## Guardrails

- Never fabricate or embellish. Nothing found is a fine result; QUIET is a legitimate status.
- Never editorialize about causation. Report the event and its date; the operator judges what the program had to do with it.
- If results conflict or look like SEO noise, prefer original sources (the company's own site, the filing, the named outlet) over aggregators.
- If the operator has flagged anyone as excluded or private, honor it in every output.

## Acceptance bar

Before handing over the report, check all three:

1. Every WIN has a source URL the operator can click.
2. Zero unverified claims stated as fact.
3. Every roster founder accounted for with a status.

If the roster's data is too thin to clear this bar honestly, say so in the report's gaps section: name the fields that would fix it (usually LinkedIn URLs), per founder. That's a useful result, not a failure.

## Report format

Use the structure in `report-example.md`: a compact dashboard first (tracked, wins, watch, pending), then one line per founder with status and finding, then the watch list with triggers, then intake gaps. Keep prose minimal; the operator reads the board, not paragraphs. Save the report as a dated markdown file in this folder; on repeat runs, report only what's new since the previous report.
