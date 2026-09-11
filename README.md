# cloud-itonami-lei-549300ttcxzogzm2ey83

> **Independent third-party archive/analysis. Not affiliated with, endorsed by, or sponsored by INDUSTRIA DE DISEÑO TEXTIL, S.A..**

This repository archives the publicly published legal notice of **INDUSTRIA DE DISEÑO TEXTIL, S.A.** (ES), with source-url and retrieval-date provenance, per
ADR-2607110300 (`cloud-itonami-lei-corporate-tos-catalog`, `com-junkawasaki/root`).
Read-only reference/archive repository — not a governed Advisor/Governor actor.

- LEI: `549300TTCXZOGZM2EY83` (GLEIF entity status ACTIVE, registration ISSUED)
- Source: https://www.inditex.com/itxcomweb/es/en/info/legal
- Retrieved: 2026-07-25T05:18:09Z
- SHA-256 of archived text: `c77ab136a0b7cd73a0cd663b7752f2e2284a807345e2f39e345a7733364ffd1b`

Acquired by `scripts/lei-acquire.cljs` as part of the worldwide-broadening
continuation that followed the 2026-07-25 coverage audit, which found the
catalog's real reach was 27 countries with the United States at 55%.

## Verified registry facts

`facts.edn` records what GLEIF publishes about this LEI — the entity record, its
managing LOU and that LOU's accreditation, the Spanish public register that
corroborated it, its ISO 20275 legal form, a count of its instrument identifiers
with each one listed, and a count of its direct children with each one listed —
with `:source/url` and `:source/retrieved-at` next to every value. Fifteen
entities across seven distinct URLs, nine requests, all re-fetched on every run.

Three things in this record are worth reading before drawing conclusions from it.

**The instrument-identifier count is two, and both are listed.** The cited ISIN
page was fetched and the whole collection fit in one page, so each identifier is
also recorded below the count as its own `:fact/kind :security` entity. Where a
count in this file is zero, `:source/note` says whether it is a measured zero, so
a bare number is never ambiguous between "GLEIF maps nothing here" and "nobody
asked".

**GLEIF reports a parent for this entity, and this file does not record it.**
Both parent-reporting-exception endpoints answer `404` — which means not "no
parent" but the opposite: there is no *exception* to report because an actual
parent is reported. `direct-parent` and `ultimate-parent` both name PONTEGADEA
INVERSIONES SL (`959800U254WM470TRW79`, ES, ACTIVE), and neither is fetched by
the generator, so neither appears below. The six `:fact/kind :direct-child`
entities describe what this entity consolidates; nothing here describes what
consolidates it. Reading this file as a complete relationship graph would be
wrong in exactly that direction.

  - https://api.gleif.org/api/v1/lei-records/549300TTCXZOGZM2EY83/direct-parent
  - https://api.gleif.org/api/v1/lei-records/549300TTCXZOGZM2EY83/ultimate-parent

  This is a gap in the shared generator (`scripts/lei-verify-facts.cljs` in
  `com-junkawasaki/root`), not in this repository's copy of it, so it is the same
  gap in every sibling archive whose entity reports a parent. Closing it means
  changing the canonical and re-vendoring across the family, which is a
  deliberate pass and not this one.

**Two recorded values are third-party websites GLEIF publishes**
(`:issuer/website`, `:authority/website`), not sources this repository fetches.
They are facts about GLEIF's record and are checked against GLEIF like any other
value; whether those sites answer from any given network is a separate question
and not one this repository claims.

`nbb scripts/verify-facts.cljk` re-fetches those sources and compares. It exits
`0` when the live registry still agrees, `1` when a citation is dead or a value
drifted, and `3` when it could not check at all (sources unreachable, `facts.edn`
missing or unreadable) — a run that could not answer must not look like a pass.
`--write` regenerates the file through the same builder the check uses, so it
cannot drift from its own generator.
