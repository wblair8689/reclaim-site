# Reclaim: marketing plan

Drafted Nov 17, 2026 for review. This is the brief for any model (or person) doing marketing work on Reclaim (reclaimdiskspace.com). Read this file first. The Marketing Simplified hub reads it before writing posts and the Monday report.

## The goal

**Organic search sales.** Grow search traffic to the Mac storage guides and turn it into $5+ purchases of Reclaim. The measure that counts is **purchases** (the `purchase` event on `thanks.html`), then visits that reach the buy button.

## What Reclaim is

A Mac disk space cleaner and analyzer (macOS 15+). It shows what is filling the disk and clears it out safely: caches, old installers, large files, unused apps. Trash first, so nothing is deleted until the user confirms. An on-device Apple Intelligence assistant ("What is this?") explains any file in plain English with a safe / be-careful verdict. 100% on the Mac: no cookies, no uploads. **Pay what you want from $5, one-time, free updates, 30-day refund.** Static site on GitHub Pages, so there is no server.

## Audience

People whose Mac says "Storage almost full" or who see a huge "System Data" in Settings. They search in plain words ("what is System Data on Mac", "how to clear cache on Mac", "delete Xcode DerivedData") and want to know what is safe to delete. Two groups:

1. **Everyday Mac users** who don't know what is taking the space and are afraid of deleting the wrong thing.
2. **Developers** (Xcode caches, DerivedData, simulators, node_modules), who are happy to read a precise guide and pay $5.

## Where we start (as of Nov 17, 2026; check the hub's Monday report for current numbers)

| Thing | State |
|---|---|
| Site | Landing page, thanks page, and four guides: what is System Data on Mac, clear cache on Mac, delete Xcode DerivedData, free up space on Mac |
| SEO basics | Sitemap, robots, search tags, Bing verification, schema.org SoftwareApplication |
| Analytics | The hub's cookieless tracker on all pages (Nov 16); GoatCounter also still running |
| Purchases | `thanks.html` sends one `purchase` per tab |
| Social | HeyCatch trial (SPEC.md, section 9): it makes the posts and Reddit/X reply drafts, and Bill approves them there |
| Blog | HeyCatch can write articles; they reach the site by PR |
| Brief | This file |

## Strategy in five sentences

1. Win the questions people search before buying: a guide per question, written for the person with a full disk.
2. Every guide ends on a clear next step: find it with Reclaim, with the buy button one scroll away.
3. Fix technical SEO first (titles, descriptions, internal links, structured data), since a small static site can't afford wasted pages.
4. Measure from search to purchase with the hub, so each guide is judged on sales, not just visits.
5. Leave social and Reddit/X replies to HeyCatch during the trial; the hub compares purchases per source at the end.

## Rules for every executor

1. **Accuracy first.** Disk-cleanup advice can break a Mac. Every instruction in a guide must be correct for macOS 15 and later and say what it deletes. Test paths and menu names before publishing; never say a folder is safe to delete if you haven't checked.
2. **Honest claims.** Don't promise a number of gigabytes. Don't say Reclaim does anything it doesn't. Pricing is pay what you want from $5; refunds within 30 days.
3. **Privacy as a feature.** Reclaim runs on the Mac, with no cookies and no uploads. Say so; never contradict it with a tracker that uses cookies.
4. **No fake growth.** No fake reviews, bought links, comment spam, or posing as a customer. Reddit and forum replies must say who wrote them, follow each community's self-promotion rules, and be drafted for Bill to post under his own name.
5. **Apple names.** Use "Mac", "macOS", "Apple Intelligence" correctly; don't imply Apple endorsement.
6. **Static site.** New pages go in as PRs to reclaim-site (a folder with `index.html`, added to `sitemap.xml`, with a title, description, canonical, and a link from `guides/index.html`). Match the style of the existing guides (`guides/guide.css`).
7. **Ask Bill before** spending money, creating an account, accepting terms, or changing prices.

## Phases and targets

Targets are goals to steer by, not promises. Replace them with real numbers once the first Monday reports give a baseline.

| Phase | Dates | Focus | Gate to move on |
|---|---|---|---|
| 0. Baseline and technical SEO | Nov 17 – Dec 15, 2026 | First reports. Audit titles, descriptions, internal links and schema on every page. Add a short FAQ with FAQ schema where it fits. Submit the sitemap in Search Console and Bing | Hub SEO issues at zero; search impressions visible |
| 1. Fill the guide set | Dec 2026 – Feb 2027 | New guides from real searches (see the list below), one every week or two, each with a clear call to action | 10 guides live; first guide ranking on page one for its query |
| 2. Win and refresh | Mar – May 2027 | Update guides when macOS changes. Improve those with traffic but few purchases. Add comparison pages only if honest | Steady purchases from search each week |
| 3. Widen | From Jun 2027 | Decide on HeyCatch social vs the hub; consider a Mac App Store listing or other channels | Per-source purchase comparison done |

## Guide ideas (verify each against real search demand first)

- How to find the largest files on a Mac
- How to delete old iOS backups on Mac
- How to clear the Downloads folder / old installers (.dmg)
- How to remove leftover files after uninstalling an app
- Xcode simulators and archives taking space
- Docker disk usage on Mac
- Mail and Messages attachments taking space
- Is it safe to delete ~/Library/Caches?
- What is "Purgeable" space on Mac?
- Mac storage full but nothing to delete

## What the hub does here

- Weekly SEO crawl and open issues in the Monday report; may open fix PRs.
- Compares visits and purchases by page and by source (search, HeyCatch posts, tracked links).
- Turns merged PRs and new guides into changelog entries and, if Bill wants, post drafts.
- Reclaim's social accounts, if added, start in review.

## Open questions for Bill

- Search Console set up for reclaimdiskspace.com?
- Keep GoatCounter once the hub's counts are trusted?
- Is there a release cadence worth announcing (version history on the site)?
