# Contribution Guidelines

Thanks for helping curate this list. Please read these guidelines before opening a PR.

## What belongs on this list

This is a **curated** list, not a comprehensive directory. To be included, an actor should be:

- **Public** on the Apify Store.
- **Maintained** — the actor was modified in the last 12 months (or has stable, working runs).
- **Reliable** — does not consistently fail or return broken data.
- **Useful** — solves a real problem better than (or differently from) anything already on the list.
- **Fairly priced** — pricing is reasonable for the value delivered. We do not include obvious price-gouging actors.

We deliberately keep each category short. A category with 50 near-identical Instagram scrapers is not useful to a reader; 8 actors that cover different needs (profiles, posts, reels, hashtags, comments) is.

## What does NOT belong

- Private actors, demo actors, or actors with fewer than ~50 users (except in MCP Servers, where the category is too young for that threshold).
- Actors that have not run successfully in the last 30 days.
- Actors that are deprecated, broken, or labelled as such by their author.
- Pure self-promotion of unmaintained code.

## Format

Each entry follows this exact format:

```markdown
- [Actor Title](https://apify.com/USERNAME/ACTOR-NAME?fpr=2ayu9b) — 8-16 word honest description. *$X/result* `@USERNAME`
```

Rules:

1. **Title** — short, descriptive, no leading emojis. Drop everything after an em-dash if the title is long.
2. **URL** — must include the affiliate parameter `?fpr=2ayu9b`. See [Affiliate code policy](#affiliate-code-policy) below.
3. **Description** — 8 to 16 words. State what the actor scrapes and any meaningful limitations. No marketing fluff. No "best", "fastest", "most powerful".
4. **Pricing tag** — match the actor's current pricing model:
   - `*Free*` for free actors
   - `*$0.XX/result*` for pay-per-result
   - `*$X/mo rental*` for monthly rental
   - `*Pay per event*` when pricing is event-based and not easily summarised
5. **Username handle** — `` `@USERNAME` `` at the end, matching the Apify username.

## Affiliate code policy

Every Apify link in this list has the suffix `?fpr=2ayu9b`. This is the affiliate code of the list maintainer ([NexGenData](https://thenextgennexus.com/)). Apify pays the affiliate, not the user — affiliate-tagged links cost end users nothing. The revenue funds list maintenance (the categorisation, link-checking, and entry editing the maintainer does for free).

If you are the author of an actor and would prefer your entry use your own affiliate code (or no affiliate code at all), say so in your PR. We will honor that request without argument. The default tag exists because no-tag would mean the maintenance is unfunded; an author-specified tag is always fine.

## Submitting a PR

1. Fork the repo.
2. Edit `README.md` and add your entry to the right category, in roughly the right popularity order (most-used actors near the top of a category).
3. If your entry belongs to a category that doesn't exist yet AND the category would have at least 4-5 quality actors, open an issue first to discuss adding the category.
4. Keep PRs small — one actor, or a few actors in the same category, per PR.
5. In the PR description, include:
   - A link to the actor's Apify store page.
   - A link to a recent successful run (helpful but not required).
   - Brief context: why this actor is worth including over what already exists.

## Reporting broken or deprecated actors

If an actor on this list no longer works, open an issue (or PR removing it). Include:

- The actor URL.
- A link to a failed run, or a screenshot of the actor's Apify page showing deprecation.
- (Optional) A suggested replacement actor in the same niche.

## Style

- Use sentence case for category names (e.g. "Real Estate", not "REAL ESTATE").
- US English spelling.
- No em-dashes inside descriptions if avoidable (em-dash is used between the link and the description).
- No exclamation marks.
- No promises about quality the actor cannot deliver ("the only scraper you need", "infinitely scalable").

## Reviewer notes (for maintainers)

- Verify the affiliate tag is present.
- Verify the actor is public and has at least one successful run in the last 30 days.
- Check the description against the actor's README. Reject if the description oversells.
- Check pricing tag against the actor's current `pricingInfo`.
- Merge with a squash commit; commit message format: `Add [actor-title] to [category]`.

## Code of conduct

Be civil. Disagreements about whether an actor belongs are fine; personal attacks are not. The maintainer's call is final on inclusion disputes — if you disagree, fork the list.
