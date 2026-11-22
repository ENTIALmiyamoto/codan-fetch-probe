# Public rental page comparison

Manual, read-only browser check of three public rental pages. Uses a standard public-repository Ubuntu runner, a six-minute job limit, and a pinned Playwright release. No schedule, credentials, LINE integration, artifacts, or caches. Results contain only public page paths, titles, HTTP status, HTML length and readiness timings.

Based on Microsoft's official Playwright GitHub Actions guide. Run manually from Actions; compare the run timestamp and page results against the production collector diagnostics. A single successful run is not proof of long-term stability.

## Result: 2026-11-22

[Manual run #2](https://github.com/ENTIALmiyamoto/codan-fetch-probe/actions/runs/44978421137) ran on the standard Ubuntu 24.04 runner with Playwright 1.56.1. All three public URLs returned HTTP 403 with title `Just a moment...`; none contained the expected listing/detail selector. This does not establish a reliable collection path. No challenge bypass or repeated automated retries were attempted. The workflow remains manual-only.

The first run stopped before fetching any pages because Ubuntu latest (26.04) was incompatible with the pinned Playwright release; this was corrected by pinning Ubuntu 24.04.
