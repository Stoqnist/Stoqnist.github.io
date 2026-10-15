# CV SEO plan

Reviewed: 15 October 2026. Goal: make the professional CV crawlable, identifiable and discoverable for relevant name and engineering searches. Rankings, indexing and ChatGPT retrieval are not guaranteed.

## Priority and status

| Priority | Action | Status / next step |
| --- | --- | --- |
| 1 | Verify ownership and inspect the homepage in Google Search Console | Ownership confirmed by user screenshot. Homepage live inspection and indexing request are not yet confirmed. Inspect exactly `https://stoqnist.github.io/`. |
| 1 | Diagnose sitemap fetch status | Submitted by owner; screenshot says Couldn't fetch. Direct checks return HTTP 200, valid XML and application/xml. Open the sitemap report details before changing code. A Googlebot user-agent check does not prove access from Google's actual infrastructure. |
| 2 | Preserve initial HTML CV, headings, links and crawl permission | Verified; no client-side rendering required. Root canonical, robots rules and one-URL sitemap deployed. |
| 2 | Accurate search identity and previews | Descriptive CV/location title, ProfilePage/Person JSON-LD, Open Graph and Twitter metadata added. Only existing public CV facts and the verified GitHub URL are used. |
| 2 | Keep unrelated utility out of CV search results | reader.html marked noindex, follow; omitted from sitemap. Do not disallow it in robots.txt: crawlers must fetch it to see noindex. |
| 3 | Add external discovery paths | Repository README links to CV. Owner must set GitHub profile website and add LinkedIn Contact info/Featured link. Confirm these actions rather than assuming completion. |
| 3 | Strengthen professional identity/content | Owner to confirm preferred full professional name, public contact method and exact LinkedIn URL. Then update visible CV, title, description and JSON-LD consistently. Do not infer private details or add invented achievements. |
| 4 | Validate rendered experience and real performance | Responsive CSS, viewport, system fonts, no dependencies/analytics/external fonts. No measured Lighthouse or field Core Web Vitals score is available. Run PageSpeed Insights after deployment; fix measured mobile problems before adding assets. |
| 4 | Measure results | After indexing, review Search Console Pages, queries, impressions and clicks after 7–14 days; compare after 28 days. Low traffic may leave reports empty. No scheduled monitoring has been created. |
| 5 | Additional discovery channels | Once Google diagnostics are resolved, consider Bing Webmaster Tools verification/import and sitemap submission using the owner's account. Requires account access; not completed. |

## Owner execution sequence

1. In the verified URL-prefix property, paste `https://stoqnist.github.io/` in the top URL inspection bar. Test live URL, review fetch/indexing permissions and request indexing if available. If URL not in property appears again, compare the exact submitted scheme/hostname/path with the selected property.
2. Open the `/sitemap.xml` row and read its detailed fetch error. The live file is `https://stoqnist.github.io/sitemap.xml`. Retain the current submission while investigating; do not repeatedly remove and re-add it without evidence. If it reports an actual corrected failure, resubmit `sitemap.xml` in the prefix field.
3. Validate homepage JSON-LD with Google's Rich Results Test and inspect the rendered HTML in Search Console. Structured data does not guarantee enhanced search appearance.
4. Set https://github.com/settings/profile website to `https://stoqnist.github.io/`; add the same URL to LinkedIn Contact info or Featured. Confirm the public profile links work.
5. Confirm public professional identity/contact information before further CV content changes.
6. Run https://pagespeed.web.dev/ for the homepage, then review search performance after enough data accumulates.

## Maintenance

Keep Google's verification file unchanged and publicly reachable. Keep the sitemap limited to canonical pages intended for search. Do not add fabricated lastmod dates, keyword lists, rating/review schema, thin keyword pages or speculative personal facts. Keep accurate content over arbitrary SEO scores. A custom domain or llms.txt is not required to resolve the current indexing issue.

## References

- https://developers.google.com/search/docs/appearance/structured-data/profile-page
- https://developers.google.com/search/docs/appearance/snippet
- https://developers.google.com/search/docs/crawling-indexing/sitemaps/build-sitemap
- https://support.google.com/webmasters/answer/7451001?hl=en
- https://developers.openai.com/api/docs/bots
