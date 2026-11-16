# ADR-001: Clear catalog rights before commercial use

- **Status:** Accepted
- **Date:** 2026-11-17

## Context

The current Django catalog displays film metadata and poster URLs. The public repository and a working demo do not prove that the owner has commercial redistribution rights for catalog records, descriptions, or artwork. TMDB's API FAQ says its free API use is non-commercial and requires attribution; commercial use requires a separate arrangement.

## Decision

Keep FrameScout an educational/free discovery demo until each displayed field and image has a documented license suitable for the intended commercial use. If paid catalog functionality is pursued, obtain written rights first or replace the feed with a rights-cleared source. Do not scrape competitors.

## Consequences

- No paid plan, paid recommendations, or commercial catalog promise is enabled by this ADR.
- The README and product pages must state the actual current limitations.
- Revisit after written rights and a qualified buyer pilot are documented.

## Source

[TMDB API FAQ](https://developer.themoviedb.org/docs/faq)
