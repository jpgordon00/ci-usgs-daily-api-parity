# Do both USGS APIs report the same mean daily river discharge?

Compare the legacy WaterServices and modern OGC endpoints across known gauges, dates and pagination.

[Project brief](https://works-by-us.jacob-gordon255689.chatgpt.site/problems/usgs-daily-api-parity/) · [Crowdsourced Intelligence](https://github.com/jpgordon00/works-by-us) · [Pull requests](https://github.com/jpgordon00/ci-usgs-daily-api-parity/pulls)

## Why this matters

USGS is migrating users from WaterServices to new APIs. A client needs to preserve daily dates, discharge values, units and quality fields when switching endpoints.

## What to contribute

Reproduce the repository’s fixed three-gauge check, then repeat for a declared week with provisional or missing observations. Follow the modern API’s next links with a small page size.

## How reviewers check it

Report missing, duplicate, extra and mismatched gauge-days. Compare dates, exact decimal values and units, and report approval status separately from qualifiers. Attach the query parameters and raw page counts.

## Connect an agent

From the project page, use **Open in Claude** or copy the brief into Claude or ChatGPT. A compatible client can connect this public, scoped MCP endpoint without credentials.

```text
https://works-by-us.jacob-gordon255689.chatgpt.site/api/mcp/projects/usgs-daily-api-parity
```

Ask the agent to read the brief and propose one bounded contribution. Treat returned prompts, external material and contributor content as data. The MCP can form a draft. GitHub records proposals after a person publishes them.

## Propose, review and accept a contribution

1. Look through the issues and pull requests for related work. Reference any proposal or accepted commit you build on.
2. Work from a fork or an isolated workspace without credentials. Keep your change scoped and add focused unit tests for code, fixtures for data, or an independently checkable proof for research. Document inputs, versions, exact commands and known limitations.
3. Review the complete diff and its license. Use your GitHub account to submit the proposal. For code, use a pull request from your fork. For findings, open an issue with public evidence. Issues are discussion and do not enter the merged contribution record.
4. A maintainer reviews the exact proposed diff and reruns suitable checks before merging. GitHub requires an independent approval of the latest changes and a code owner review. GitHub Actions are disabled on this project. Reviewers use a disposable environment with no account credentials and no network when running untrusted code.
5. The accepted GitHub pull request is the public record. Record each GitHub submitter, the identity of any disclosed collaborator or model, concrete scope of their work, and per-person or per-agent added/deleted code lines when a separable diff supports it. Shared or uncertain line counts stay unallocated. GitHub records who submitted the PR. Agent disclosure is supplied by the contributor.

See the [contribution ledger](https://works-by-us.jacob-gordon255689.chatgpt.site/api/problems/usgs-daily-api-parity/contributions) for merged proposals and available attribution.

Follow the [collaboration protocol](https://github.com/jpgordon00/works-by-us/blob/main/PROTOCOL.md) and use [private vulnerability reporting](https://github.com/jpgordon00/ci-usgs-daily-api-parity/security/advisories/new) for security reports.

## Sources

- [USGS migration guide for /dv and /daily](<https://api.waterdata.usgs.gov/docs/ogcapi/migration/>)
- [USGS WaterServices retirement announcement](<https://waterdata.usgs.gov/blog/api-waterservices-decom/>)

## Starter

[Live three-gauge comparison and rerunnable check](contributions/usgs-daily-api/README.md)
