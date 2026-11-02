# Getting help

- **Docs:** [slidecold.com/docs](https://slidecold.com/docs) and the [OpenAPI spec](https://slidecold.com/openapi.yaml)
- **Your account, billing, or API behavior:** [support@slidecold.com](mailto:support@slidecold.com)
- **A bug in an SDK, the CLI or the MCP server:** open an issue in that repo, and include the package version and the full error message (remove your API key first)

Common errors:

| Status | Meaning |
|---|---|
| `401 Invalid API key` | The key is wrong or was deleted. Create a new one under Settings → API Keys. |
| `403 ... missing the <resource>:<action> scope` | The key works but wasn't given that scope. Create a key with the scope you need. |
| `403` (other) | A plan limit or a team permission. |
| `429` | Instagram or SlideCold rate limit. Wait and retry. |
