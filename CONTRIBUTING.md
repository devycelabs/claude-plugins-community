# Contributing to claude-plugins-community

A curated registry of community-built Claude Code plugins that aren't part of the official marketplace.

---

## Submitting a plugin

Open a pull request adding your plugin to `registry.json`. Your PR must include:

### Required fields

```json
{
  "name": "your-plugin-name",
  "displayName": "Your Plugin Name",
  "description": "One sentence. What it does, not what it is.",
  "author": "your-github-username",
  "repo": "your-github-username/your-repo-name",
  "marketplace": "your-github-username/your-repo-name",
  "addedAt": "YYYY-MM-DD",
  "lastVerified": "YYYY-MM-DD",
  "verificationDue": "YYYY-MM-DD",
  "status": "active",
  "tags": ["one", "or", "more"]
}
```

- `name` — must match the `name` field in your plugin's `.claude-plugin/plugin.json`
- `marketplace` — the value users pass to `claude plugin marketplace add`
- `tags` — pick from: `productivity`, `git`, `code-quality`, `testing`, `devops`, `ai`, `data`, `docs`, `ui`, `language-server`, `mcp`, `other`

### Vetting checklist

Before submitting, confirm your plugin meets these criteria:

- [ ] Public GitHub repository
- [ ] Contains a valid `.claude-plugin/plugin.json`
- [ ] Has a `README.md` explaining what it does and how to use it
- [ ] Has a `LICENSE` file
- [ ] Does not request unnecessary permissions
- [ ] Does not transmit user data to external services without disclosure
- [ ] No hardcoded secrets or credentials in the codebase
- [ ] Actively maintained (recent commit activity)

PRs that don't meet these criteria will be closed without merge.

---

## Review process

Submissions are reviewed by Devyce Labs maintainers. We check:

1. The plugin installs and runs without errors
2. The plugin does what it says it does
3. No obvious security concerns in the code
4. Description is accurate and useful

We aim to review PRs within **7 days**. We may request changes before merging.

---

## Active verification (6-month cycle)

All listed plugins undergo a verification check every **6 months** to confirm they are still actively maintained.

When your `verificationDue` date arrives:

- A GitHub issue will be opened in this repo, tagging you
- You have **30 days** to respond confirming the plugin is still active
- If you respond: `lastVerified` and `verificationDue` are updated (+6 months), status stays `active`
- If no response after 30 days: status is changed to `archived`

**Archived plugins** remain in the registry and are still installable — they just show an `archived` indicator in the plugin browser so users know maintenance may have lapsed.

To un-archive: open a PR updating `lastVerified`, `verificationDue`, and `status` back to `active`, with a note confirming the plugin is maintained again.

---

## Removing a plugin

Open a PR removing your entry from `registry.json`. We'll merge it promptly.
Alternatively, open an issue and we'll handle it.
