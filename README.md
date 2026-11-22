# Public rental page comparison

Manual, read-only browser check of three public rental pages. Uses a standard public-repository Ubuntu runner, a six-minute job limit, and a pinned Playwright release. No schedule, credentials, LINE integration, artifacts, or caches. Results contain only public page paths, titles, HTTP status, HTML length and readiness timings.

Based on Microsoft's official Playwright GitHub Actions guide. Run manually from Actions; compare the run timestamp and page results against the production collector diagnostics. A single successful run is not proof of long-term stability.
