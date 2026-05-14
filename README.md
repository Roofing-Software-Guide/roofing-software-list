# roofing-software-list

A public, structured directory of every roofing software product Roofing Software Guide tracks — categories, pricing tiers, integrations, vendor URLs.

This repo is the data behind the reviews at **[roofingsoftwareguide.com](https://roofingsoftwareguide.com)**. We publish it openly so contractors, journalists, and analysts can cite it, fork it, or build on it.

## Why this exists

There is no single up-to-date public list of roofing software vendors. Contractors waste hours comparing products that don't even fit their stack (residential vs commercial, solo vs crew, estimating-first vs CRM-first). This repo is our attempt to fix that.

## Structure

- `roofing-software.json` — the master list, one object per product, with category, pricing tier, integrations, and metadata
- `categories.json` — controlled vocabulary for product categories
- `CHANGELOG.md` — what changed and when (so cited versions are reproducible)

## Schema

Each entry in `roofing-software.json`:

```json
{
  "slug": "vendor-name",
  "name": "Vendor Name",
  "url": "https://vendor.com",
  "categories": ["estimating", "crm"],
  "audience": ["residential", "commercial"],
  "pricing_tier": "mid",
  "free_trial": true,
  "integrations": ["quickbooks", "stripe"],
  "rsg_review_url": "https://roofingsoftwareguide.com/reviews/vendor-name/",
  "last_verified": "2026-05-13"
}
```

Pricing tiers are coarse on purpose: `free` · `low` (<$100/mo) · `mid` ($100–$500/mo) · `high` ($500+/mo) · `enterprise` (custom). Exact prices change too often to maintain in a public list.

## Contributing

If you spot a missing vendor or stale data, open an issue with the vendor URL. We verify against the vendor's own site or pricing page before merging.

## License

Data is published under **CC BY 4.0** — free to use with attribution to [Roofing Software Guide](https://roofingsoftwareguide.com).

## Maintained by

[Roofing Software Guide](https://roofingsoftwareguide.com) — independent roofing software reviews. Editor: [Matt Richardson](https://www.linkedin.com/in/matt-richardson-81b06a400/).
# roofing-software-list
Public structured directory of roofing software products tracked by Roofing Software Guide — categories, pricing tiers, integrations, vendor URLs. CC BY 4.0.
