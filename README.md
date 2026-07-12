# FFC-EX-my-missions.org

Subsistence Aviation Mission — FFC-supported charity website (static, GitHub Pages).

This repository holds a fully localized static capture of the former WordPress site at
`my-missions.org` (previously hosted on Hostinger), migrated as part of the FFC
Wave-1 WordPress-to-Pages program
([FFC-Cloudflare-Automation#702](https://github.com/FreeForCharity/FFC-Cloudflare-Automation/issues/702)).

## Hosting

- Deployed to GitHub Pages on the default URL:
  <https://freeforcharity.github.io/FFC-EX-my-missions.org/>
- Deployment runs from `.github/workflows/static.yml` on every push to `main`.
- No custom domain and no DNS changes are configured at this stage.

## Structure

Plain static HTML capture — no build step. 29 pages: home, About Us, Donate Now,
The Mission in Alaska, Homepage, plus the blog (posts under `/2018/`, `/2019/`,
`/2022/`, with category/author/date archive pages and pagination).

All CSS/JS/fonts/images are served from this repository (external font and analytics
hosts were localized or stripped during migration). Donation links go to the
charity's GivingFuel page (external navigation, unchanged).

## Maintenance

- Edit the HTML in place; every push to `main` redeploys.
- `linkcheck.yml` runs lychee weekly and on pushes/PRs to catch link rot.
- See the migration tracking issue in this repo for what was captured, stripped,
  and flagged during the WordPress-to-static conversion.

---

Supported by [Free For Charity](https://freeforcharity.org).
