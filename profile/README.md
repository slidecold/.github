<p align="center">
  <a href="https://slidecold.com">
    <img src="https://cdn.slidecold.com/static/logo-transparent.png" alt="SlideCold" width="96">
  </a>
</p>

<h3 align="center">SlideCold</h3>

<p align="center">
  Instagram cold-DM outreach: scrape targeted audiences, warm up accounts safely, and send personalized DMs at scale.
  <br>
  <a href="https://slidecold.com"><strong>slidecold.com</strong></a> ·
  <a href="https://slidecold.com/docs">Docs</a> ·
  <a href="https://slidecold.com/openapi.yaml">OpenAPI spec</a>
</p>

---

### Build on SlideCold

Everything in the dashboard is available over the REST API: accounts, proxies, audiences, campaigns and conversations. Create an API key under **Settings → API Keys** and pick only the scopes you need.

| | Repo | Install |
|---|---|---|
| **CLI** | [slidecold-cli](https://github.com/slidecold/slidecold-cli) | [Release binaries](https://github.com/slidecold/slidecold-cli/releases) · `go install github.com/slidecold/slidecold-cli/cmd/slidecold@latest` |
| **MCP server** | [slidecold-mcp](https://github.com/slidecold/slidecold-mcp) | `npx -y slidecold-mcp` |
| **Node.js / TypeScript** | [slidecold-node](https://github.com/slidecold/slidecold-node) | `npm install slidecold` |
| **Python** | [slidecold-python](https://github.com/slidecold/slidecold-python) | `pip install slidecold` |
| **Go** | [slidecold-go](https://github.com/slidecold/slidecold-go) | `go get github.com/slidecold/slidecold-go` |

[![npm](https://img.shields.io/npm/v/slidecold?label=npm%20slidecold)](https://www.npmjs.com/package/slidecold)
[![npm](https://img.shields.io/npm/v/slidecold-mcp?label=npm%20slidecold-mcp)](https://www.npmjs.com/package/slidecold-mcp)
[![PyPI](https://img.shields.io/pypi/v/slidecold?label=pypi%20slidecold)](https://pypi.org/project/slidecold/)
[![Go Reference](https://pkg.go.dev/badge/github.com/slidecold/slidecold-go.svg)](https://pkg.go.dev/github.com/slidecold/slidecold-go)

### Quick start

```bash
# CLI
slidecold login                  # saves your key to ~/.config/slidecold/config.json
slidecold campaigns list

# Use SlideCold from Claude Code
claude mcp add slidecold -e SLIDECOLD_API_KEY=cs_... -- npx -y slidecold-mcp
```

```ts
import { SlideCold } from "slidecold";

const sc = new SlideCold(); // reads SLIDECOLD_API_KEY or ~/.config/slidecold/config.json
const campaigns = await sc.campaigns.list();
```

Every SDK, the CLI and the MCP server are generated from the same [OpenAPI spec](https://slidecold.com/openapi.yaml), so they always cover the same operations. Releases are built and published by GitHub Actions with signed provenance: verify a download with `gh attestation verify <file> --owner slidecold`.

### Help

- Questions about the API or your account: [support@slidecold.com](mailto:support@slidecold.com)
- Bugs in an SDK, the CLI or the MCP server: open an issue in that repo
- Security issues: see our [security policy](https://github.com/slidecold/.github/blob/main/SECURITY.md)
