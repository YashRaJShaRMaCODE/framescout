# FrameScout feature roadmap

These are proposed additions to the existing catalog/search/filter/share/local-watchlist baseline. Impact and effort are estimates; competitor gaps are hypotheses based on the public review examples in [`MARKET_RESEARCH.md`](MARKET_RESEARCH.md). Interview users and clear content rights before committing to expensive data or AI work.

| # | Feature | User problem solved | Gap to test | Impact | Effort | Acceptance proof |
|---:|---|---|---|---|---|---|
| 1 | Watchlist decision shortlist with editable reasons | A large list still leaves users unsure what to watch tonight | General catalogs return too many choices | High | Medium | User creates a 3-title shortlist and sees why each fits |
| 2 | Mood and time filters using existing metadata | Users know their mood/time but not the title | Search starts from title/provider rather than viewing context | High | Medium | Filters work with keyboard and mobile, including no-match state |
| 3 | Two-person pick mode with private vetoes | Friends spend time negotiating a title | Social discovery can expose more profile activity than desired | High | Medium | Both people can shortlist/veto without public profiles |
| 4 | Explainable related-film reasons | Users cannot tell why a title was recommended | Recommendations can feel generic or opaque | High | Low | Every reason maps to a real shared genre/director field |
| 5 | Optional spoiler-labeled synopsis toggle | Plot details can spoil a first watch | Detail pages often expose full summaries immediately | High | Low | Implemented locally with a native, keyboard-accessible closed disclosure; page metadata uses non-plot details |
| 6 | Fast offline catalog snapshot | Poor connectivity breaks browsing | Server-first discovery is not available on a commute | Medium | Medium | Cached catalog opens read-only with clear freshness time |
| 7 | Watchlist notes and personal tags | Lists lack context like who recommended a film | Simple watchlists lack lightweight organization | Medium | Low | Notes stay device-local, export and delete with the item |
| 8 | Duplicate-safe Letterboxd CSV import | Switching tools requires manual re-entry | Export/import support differs across products | High | Medium | Preview duplicates, invalid rows, and final merge before writes |
| 9 | Watchlist backup integrity check | A JSON backup can be incomplete or stale | Cross-device state needs trust and recoverability | High | Low | Validates schema/count and offers restore preview |
| 10 | Shareable themed collection cards | Clubs need a clean link for a screening theme | Public list sharing may require an account | Medium | Medium | Public link includes no private watchlist data |
| 11 | Locally computed taste map | Fans cannot see patterns across saved titles | Paid stats may be excessive for casual discovery | Medium | Medium | Aggregate summary runs on-device and explains data used |
| 12 | Accessibility preferences for poster/list density | Poster grids can be hard to scan or read | Visual browsing can make text-heavy alternatives easier | Medium | Medium | User can choose compact/list mode, keyboard and screen reader verified |
| 13 | Catalog provenance and freshness panel | Users cannot tell how current a title record is | Aggregators hide source/freshness context | High | Medium | Each record exposes verified source and update date |
| 14 | Club curator workspace with CSV/PDF export | A host needs a simple screening handout | Consumer tools lack organizer outputs | Medium | High | Export only rights-cleared fields and pass a club pilot review |
| 15 | Optional natural-language discovery | Users struggle to translate a mood into filters | Basic search needs exact metadata terms | Medium | High | Uses a licensed catalog, no invented facts, opt-in, and cost cap |

**Build order:** validate #1–#4 with users first. Add authentication, payments, AI, cross-device sync, and commercial catalog feeds only after demand and licensing are established. None of these 15 proposals is marked implemented by this roadmap alone.
