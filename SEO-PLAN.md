# CV SEO plan

Reviewed: 16 October 2026. Goal: make the professional CV crawlable, identifiable and discoverable for relevant name and engineering searches. Rankings, indexing and ChatGPT retrieval are not guaranteed.

## Priority and status

| Priority | Action | Status / next step |
| --- | --- | --- |
| 1 | Verify ownership and inspect the homepage in Google Search Console | DONE: ownership verified. Google live test passed on 15 October: URL available, page can be indexed, one valid ProfilePage item detected. Owner confirmed requesting indexing on 15 October. Actual indexing remains unconfirmed. |
| 1 | Diagnose sitemap fetch status | PENDING GOOGLE: details on 16 October said Sitemap could not be read, last read 15 October. Resubmission accepted on 16 October (screenshot). Direct check on 16 October returned HTTP 200, valid XML and application/xml. Do not repeatedly resubmit. Recheck after processing. A Googlebot user-agent check does not prove access from Google's actual infrastructure. |
| 2 | Preserve initial HTML CV, headings, links and crawl permission | Verified; no client-side rendering required. Root canonical, robots rules and one-URL sitemap deployed. |
| 2 | Accurate search identity and previews | Descriptive CV/location title, ProfilePage/Person JSON-LD, Open Graph and Twitter metadata added. Only existing public CV facts and the verified GitHub URL are used. Google live test confirmed one valid ProfilePage item. |
| 2 | Keep unrelated utility out of CV search results | reader.html marked noindex, follow; omitted from sitemap. Do not disallow it in robots.txt: crawlers must fetch it to see noindex. |
| 3 | Add external discovery paths | DONE: repository README link deployed. Screenshots on 16 October confirm CV website links on both GitHub profile and LinkedIn Contact info. |
| 3 | Strengthen professional identity/content | Owner to confirm preferred full professional name, public contact method and exact LinkedIn URL. Then update visible CV, title, description and JSON-LD consistently. Do not infer private details or add invented achievements. |
| 4 | Validate rendered experience and real performance | Responsive CSS, viewport, system fonts, no dependencies/analytics/external fonts. Performance measurement remains OPEN: PageSpeed API attempt on 16 October returned HTTP 429 RESOURCE_EXHAUSTED (service quota). No score was produced. Run https://pagespeed.web.dev/ with the live homepage using the web UI. No field Core Web Vitals data is available. |
| 4 | Measure results | After indexing, review Search Console Pages, queries, impressions and clicks after 7–14 days; compare after 28 days. Low traffic may leave reports empty. No scheduled monitoring has been created. |
| 5 | Additional discovery channels | Once Google diagnostics are resolved, consider Bing Webmaster Tools verification/import and sitemap submission using the owner's account. Requires account access; not completed. |

## Remaining execution sequence

1. Bing setup: open https://www.bing.com/webmasters/ and import the verified site from Google Search Console. Select only `https://stoqnist.github.io/`. Confirm the sitemap is imported; otherwise submit `https://stoqnist.github.io/sitemap.xml`. Use Bing URL inspection/submission for the homepage. This requires the owner's sign-in and consent and has not been completed.
2. Performance audit: open https://pagespeed.web.dev/, analyze `https://stoqnist.github.io/`, and review mobile and desktop results. The API was quota-blocked, so do not claim a performance score. Fix measured issues and verify the result.
3. Professional identity: screenshot shows LinkedIn URL `https://www.linkedin.com/in/stoyan-georgiev-georgiev/`, name Stoyan Georgiev and a contact email. The owner has not confirmed the preferred name or publishing email on the public CV. Keep the existing CV identity until confirmed; do not copy phone/birthday or other incidental contact-panel data.
4. Processing follow-up: on or after 19 October check Google homepage index status and sitemap read status. Do not repeat ownership verification, the successful live test, completed profile links or the indexing request without a new reason. This is a suggested review date, not an automation.
5. Results: review queries, impressions and clicks after 7–14 days; compare after 28 days. Actual indexing and traffic are outcomes to verify, not completed setup steps.

## Completion criteria

Technical deployment and external profile links are complete. Google live eligibility and structured-data validation are complete. Remaining setup: Bing and measured performance; content identity requires owner confirmation. Google processing and later search measurement remain pending. The plan must not be described as fully complete until these distinctions are resolved.

## Maintenance

Keep Google's verification file unchanged and publicly reachable. Keep the sitemap limited to canonical pages intended for search. Do not add fabricated lastmod dates, keyword lists, rating/review schema, thin keyword pages or speculative personal facts. Keep accurate content over arbitrary SEO scores. A custom domain or llms.txt is not required to resolve the current indexing issue.

## References

- https://developers.google.com/search/docs/appearance/structured-data/profile-page
- https://developers.google.com/search/docs/appearance/snippet
- https://developers.google.com/search/docs/crawling-indexing/sitemaps/build-sitemap
- https://support.google.com/webmasters/answer/7451001?hl=en
- https://developers.openai.com/api/docs/bots

- https://www.bing.com/webmasters/help/add-and-verify-site-12184f8b
