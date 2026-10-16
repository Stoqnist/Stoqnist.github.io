# CV SEO plan

Reviewed: 16 October 2026. Goal: make the professional CV crawlable, identifiable and discoverable for relevant name and engineering searches. Rankings, indexing and ChatGPT retrieval are not guaranteed.

## Priority and status

| Priority | Action | Status / next step |
| --- | --- | --- |
| 1 | Verify ownership and inspect the homepage in Google Search Console | DONE: ownership verified. Google live test passed on 15 October: URL available, page can be indexed, one valid ProfilePage item detected. Owner confirmed requesting indexing on 15 October. Actual indexing remains unconfirmed. |
| 1 | Diagnose sitemap fetch status | PENDING GOOGLE: details on 16 October said Sitemap could not be read, last read 15 October. Resubmission accepted on 16 October (screenshot). Direct check on 16 October returned HTTP 200, valid XML and application/xml. Do not repeatedly resubmit. Recheck after processing. A Googlebot user-agent check does not prove access from Google's actual infrastructure. |
| 2 | Preserve initial HTML CV, headings, links and crawl permission | Verified; no client-side rendering required. Root canonical, robots rules and one-URL sitemap deployed. |
| 2 | Accurate search identity and previews | Descriptive CV/location title, ProfilePage/Person JSON-LD, Open Graph and Twitter metadata added. Uses owner-confirmed professional identity and GitHub/LinkedIn URLs. Google live test confirmed one valid ProfilePage item. |
| 2 | Keep unrelated utility out of CV search results | reader.html marked noindex, follow; omitted from sitemap. Do not disallow it in robots.txt: crawlers must fetch it to see noindex. |
| 3 | Add external discovery paths | DONE: repository README link deployed. Screenshots on 16 October confirm CV website links on both GitHub profile and LinkedIn Contact info. |
| 3 | Strengthen professional identity/content | DONE: owner explicitly approved Stoyan Georgiev, stoqnist@gmail.com and https://www.linkedin.com/in/stoyan-georgiev-georgiev/ on 16 October. Published in visible CV and matching search/social metadata and Person JSON-LD. |
| 4 | Validate rendered experience and real performance | Responsive CSS, viewport, system fonts, no dependencies/analytics/external fonts. Mobile PageSpeed audit confirmed by screenshot on 16 October, report time 14:56:41: Performance 100, Accessibility 100, Best Practices 100, SEO 100; agentic browsing 2/2. These are automated lab results, not proof of perfect accessibility or search rankings. No real-user data is available. Desktop report and full mobile/print visual review remain unverified. |
| 4 | Measure results | After indexing, review Search Console Pages, queries, impressions and clicks after 7–14 days; compare after 28 days. Low traffic may leave reports empty. No scheduled monitoring has been created. |
| 5 | Additional discovery channels | Bing site setup and sitemap reading confirmed on 16 October: Success, one URL discovered, zero sitemap errors/warnings. DONE: screenshot at 14:55 confirms Indexing requested and successful URL submission. Live URL at 14:56: URL can be indexed by Bing, no SEO/GEO issues found, JSON-LD and OpenGraph detected. Actual indexing remains pending; prior index status was Discovered but not crawled. |

## Remaining execution sequence

1. Bing setup and live validation COMPLETE: sitemap read successfully, indexing request accepted, Live URL eligible, no SEO/GEO issues detected. Wait for actual indexing; do not repeatedly submit.
2. Mobile automated audit COMPLETE with four 100/100 category scores. Review the Desktop tab and visually inspect mobile/desktop/print layout. No corrective change is justified by the supplied mobile category scores alone.
3. Professional identity: COMPLETE. Owner-confirmed name, email and LinkedIn are published. Do not add incidental phone/birthday data.
4. Processing follow-up: on or after 19 October check Google homepage index status and sitemap read status. Do not repeat ownership verification, the successful live test, completed profile links or the indexing request without a new reason. This is a suggested review date, not an automation.
5. Results: review queries, impressions and clicks after 7–14 days; compare after 28 days. Actual indexing and traffic are outcomes to verify, not completed setup steps.

## Completion criteria

Technical deployment and external profile links are complete. Google live eligibility and structured-data validation are complete. Professional identity and Bing sitemap setup are complete. Bing live URL/indexing request and mobile measured performance are complete. Remaining validation: desktop report, full rendered/print review, and a readable result of the new Google Rich Results Test. Google processing and later search measurement remain pending. The plan must not be described as fully complete until these distinctions are resolved.

## Evidence from 16 October, 14:55–14:57

- Owner screenshots confirm Bing indexing request accepted and successful live eligibility test.
- Mobile PageSpeed report: https://pagespeed.web.dev/analysis/https-stoqnist-github-io/9s4fblwujg?form_factor=mobile — four 100 scores visible in screenshot; detailed metrics and desktop results not yet inspected.
- New Google Rich Results Test link supplied: https://search.google.com/test/rich-results/result?id=Xzb6KoqGL5ea-MMNaDQvkQ — web retrieval failed; no result screenshot supplied, so this new test is not yet confirmed. Earlier Google ProfilePage validation remains confirmed.

## Maintenance

Keep Google's verification file unchanged and publicly reachable. Keep the sitemap limited to canonical pages intended for search. Do not add fabricated lastmod dates, keyword lists, rating/review schema, thin keyword pages or speculative personal facts. Keep accurate content over arbitrary SEO scores. A custom domain or llms.txt is not required to resolve the current indexing issue.

## References

- https://developers.google.com/search/docs/appearance/structured-data/profile-page
- https://developers.google.com/search/docs/appearance/snippet
- https://developers.google.com/search/docs/crawling-indexing/sitemaps/build-sitemap
- https://support.google.com/webmasters/answer/7451001?hl=en
- https://developers.openai.com/api/docs/bots

- https://www.bing.com/webmasters/help/add-and-verify-site-12184f8b
