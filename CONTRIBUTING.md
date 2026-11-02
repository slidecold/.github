# Contributing

Thanks for helping improve SlideCold's developer tools.

## How the repos fit together

The SDKs ([Node](https://github.com/slidecold/slidecold-node), [Python](https://github.com/slidecold/slidecold-python), [Go](https://github.com/slidecold/slidecold-go)), the [CLI](https://github.com/slidecold/slidecold-cli) and the [MCP server](https://github.com/slidecold/slidecold-mcp) are all generated from the [OpenAPI spec](https://slidecold.com/openapi.yaml). Each SDK repo keeps a copy as `openapi.yaml`.

- **The API behaves differently from the spec?** That's an API bug, not an SDK bug. Open an issue and include the request and response.
- **Never edit generated files by hand.** Change the generator or the spec, then regenerate. CI fails if generated code is stale.

## Pull requests

1. Open an issue first for anything larger than a small fix, so we can agree on the approach.
2. Keep each PR focused, and add or update tests for the behavior you change.
3. Run the repo's checks locally (each README lists them) before you push.
4. Don't include real API keys, account data or customer information in code, tests, issues or logs.

By contributing, you agree that your contribution is licensed under the MIT license of the repo.
