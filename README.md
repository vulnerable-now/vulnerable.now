# vulnerable.now

[vulnerable.now](https://vulnerable.now/) is a public catalog of software vulnerabilities. **It’s free to use, private, and requires no account.** Look up a CVE, see whether a version you run is affected, and find the fix and the advisory that published it.


## Search the catalog

[Explore](https://vulnerable.now/explore) searches by CVE or advisory ID, vendor, product, package, or description. You can filter by severity, exploitation status, ecosystem, and publication date, then sort by relevance, recency, CVSS, EPSS, or priority.

Each entry combines records from its sources on one page. When available, it shows affected and fixed versions, CVSS severity, the EPSS estimate of exploitation likelihood, and evidence of known exploitation. Entries link to their original advisories. CVE pages can also include an AI-written overview alongside the source records.

- [Exploited](https://vulnerable.now/exploited) tracks entries in CISA's Known Exploited Vulnerabilities catalog.
- [Rankings](https://vulnerable.now/rankings) orders vulnerabilities by patching priority. The [scoring method](https://vulnerable.now/about#priority) explains how the site weighs severity and exploitation signals.
- [Daily](https://vulnerable.now/daily) groups newly published CVEs by UTC date.

You can also [install vulnerable.now as a web app](https://vulnerable.now/#install-app) on a supported browser or phone.

## Find what affects your software

Browse [Packages](https://vulnerable.now/packages) by ecosystem or look up a vendor and product in [Technologies](https://vulnerable.now/tech). Enter the version you run to see which advisories apply and, where the published version ranges allow it, the earliest upgrade that addresses all matching entries. The [WordPress index](https://vulnerable.now/wordpress) covers core, plugins, and themes.

[Check dependencies](https://vulnerable.now/check) accepts supported lockfiles, CycloneDX and SPDX SBOMs, and Wappalyzer exports. Results include affected components, available fixes, and a SARIF download. If you create a share link, the saved report can update as new advisories appear, and it comes with its own RSS feed.

To check a WordPress installation, use [WordPress site check](https://vulnerable.now/check?mode=wordpress). Enter the core version and the plugin and theme versions, or paste the lists from WP-CLI.

## API, MCP, and feeds

The public API, MCP server, and feeds require no API key.

- [JSON API documentation](https://vulnerable.now/agents#api) and [OpenAPI definition](https://vulnerable.now/api/v1/openapi.json) cover catalog search, advisory lookups, and dependency checks.
- [MCP setup](https://vulnerable.now/agents#mcp) explains how to connect to `https://vulnerable.now/mcp` over Streamable HTTP for read-only catalog lookups and checks.
- Subscribe to new entries via [RSS](https://vulnerable.now/feed), [Atom](https://vulnerable.now/feed.atom), or [JSON Feed](https://vulnerable.now/feed.json). Use the [daily recap feed](https://vulnerable.now/daily/feed) for one roundup per UTC day.
- Add `.md` to supported catalog URLs or send `Accept: text/markdown` to get the page as Markdown. See the [machine-readable formats](https://vulnerable.now/agents#llms).

## Data sources

The catalog draws on the CVE List, NVD, GitHub Advisory Database, OSV, and ENISA EUVD, among other sources. CISA KEV and FIRST EPSS supply exploitation status and likelihood data. See the [full source list](https://vulnerable.now/about#sources) and [how records are merged](https://vulnerable.now/about#merge).

## Privacy

The site runs without ads or tracking cookies, and our server keeps no request logs. Cloudflare handles traffic and provides aggregate analytics.

[Read the full privacy policy](https://vulnerable.now/privacy).

## Report a bug or request a feature

[Open a GitHub issue](https://github.com/vulnerable-now/vulnerable.now/issues/new) for site bugs, feature requests, or errors in how vulnerable.now shows or merges an advisory. For a bug, include the page URL, what you expected, and what happened. For a catalog correction, include the CVE or advisory ID and a link to the source record. If the source record itself is wrong, report it to the publisher.

For a security issue in vulnerable.now itself, use the private reporting instructions on the [security page](https://vulnerable.now/security).
