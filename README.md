# Stoyan — CV website

A lightweight, English-language CV for applications in the Netherlands. Static HTML and CSS, ready for GitHub Pages; no build step, dependencies, analytics or external fonts.

Live CV: [https://stoqnist.github.io/](https://stoqnist.github.io/)

## Pages

- `index.html`: CV, with responsive layout and a Print / save PDF button using the browser print dialog.
- `style.css`: screen, mobile and A4 print styles.
- `reader.html`: the previous text-reader functionality, preserved separately.

## Content

Derived from the career record reviewed on 15 October 2026. Publish only professional CV content here; do not commit the private source record. ScavaSoft is the employer; Docebo projects and StoryShell are responsibilities within that employment. The licensing platform reached beta; StoryShell experiments were not production ML work.

Before using this as an application CV, confirm and add the preferred full professional name and contact email, plus a LinkedIn URL if desired. The supplied source does not provide verified current contact details. No placeholders or guessed details are shown to visitors. Review dates and current-employment status when updating.

## Preview and print

Open `index.html` in a browser, or serve this directory with a static web server. Use Print / save PDF, select A4 and disable browser headers and footers. Print pagination depends on the browser; review the result before sending.

## Hosting

Merge the CV branch into the branch configured for GitHub Pages (normally `main`, repository root). Existing Pages settings are not changed by this source update. The expected address is https://stoqnist.github.io/ when Pages is enabled and deployment succeeds.

## Search discovery

The CV text and headings are in the initial HTML; JavaScript is only used for printing. Keep the title and description accurate when changing the CV. The canonical URL and sitemap identify `https://stoqnist.github.io/` as the CV URL. `robots.txt` allows crawling, including OAI-SearchBot. Permission to crawl does not guarantee indexing or successful retrieval by any particular tool.

### Google Search Console (account owner)

1. Open https://search.google.com/search-console/ and sign in.
2. Add a **URL prefix** property for `https://stoqnist.github.io/`. Do not choose a Domain property: GitHub controls the `github.io` DNS.
3. Choose **HTML tag** verification. Copy the exact `google-site-verification` meta tag Google provides and add it inside `<head>` in `index.html`. Publish, check that the live page contains it, then click **Verify**. Keep the tag after verification. Alternatively, commit Google's supplied HTML verification file unchanged at the repository root.
4. Inspect `https://stoqnist.github.io/`, choose **Test live URL**, review crawl/indexing status, then **Request indexing** if eligible.
5. Under **Sitemaps**, submit `https://stoqnist.github.io/sitemap.xml`.

Verification requires Google's actual account-specific token; do not commit a placeholder. Indexing is not guaranteed and may take time.

### Profile discovery links (account owner)

- GitHub: open https://github.com/settings/profile and set the website URL to `https://stoqnist.github.io/`. If a profile README is used, add `[My CV](https://stoqnist.github.io/)` there too.
- LinkedIn: add `https://stoqnist.github.io/` as a website in Contact info and/or a Featured link titled “Stoyan — Backend & Cloud Engineer CV”.

Official references: [Google ownership verification](https://support.google.com/webmasters/answer/9008080?hl=en), [URL inspection](https://support.google.com/webmasters/answer/9012289?hl=en), [OpenAI crawlers](https://developers.openai.com/api/docs/bots).
