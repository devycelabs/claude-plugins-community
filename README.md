# claude-plugins-community

A curated registry of community-built Claude Code plugins — vetted, maintained, and verified.

> **Not in the official marketplace?** This is the place.
> Plugins here are built by the community, reviewed by [Devyce Labs](https://github.com/devycelabs), and kept honest with a 6-month active verification cycle.

---

## Install a plugin

```bash
# Add this registry as a marketplace source
claude plugin marketplace add devycelabs/claude-plugins-community

# Then install any plugin from the list below
claude plugin install <plugin-name>
```

Or browse visually with [plugin-browser](https://github.com/devycelabs/claude-plugin-browser).

---

## Plugin registry

<!-- REGISTRY_TABLE_START -->
*No plugins listed yet. Be the first — see [CONTRIBUTING.md](CONTRIBUTING.md).*
<!-- REGISTRY_TABLE_END -->

---

## Status legend

| Badge | Meaning |
|-------|---------|
| ✅ Active | Verified within the last 6 months |
| ⏳ Pending | Verification due — awaiting contributor response |
| 🗄️ Archived | No longer actively maintained. Still installable. |

---

## Submit your plugin

See [CONTRIBUTING.md](CONTRIBUTING.md) for the full submission process and vetting criteria.

The short version:
1. Fork this repo
2. Add your entry to `registry.json`
3. Open a pull request

Submissions are reviewed within 7 days.

---

## Verification cycle

Every listed plugin is checked every **6 months**. Contributors are tagged in a GitHub issue and have 30 days to confirm the plugin is still active. No response = archived status. Archived plugins remain installable but are clearly flagged in the browser.

See [CONTRIBUTING.md](CONTRIBUTING.md) for full details.

---

## Maintainer setup

When forking or transferring this repo, create these GitHub labels before any submissions arrive — the automation depends on them:

| Label | Colour | Used by |
|-------|--------|---------|
| `verification` | `#e4e669` | `verification-check.yml` — weekly active-status issues |
| `submission` | `#0075ca` | Submission issue template |

Create them at `github.com/<org>/<repo>/labels`.

---

*Maintained by [Devyce Labs](https://github.com/devycelabs) · [claude-plugin-browser](https://github.com/devycelabs/claude-plugin-browser)*
