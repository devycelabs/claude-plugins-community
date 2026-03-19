---
name: Plugin verification (reference only)
about: "Reference template showing the format of automated verification issues. Do not open manually — these are created by the verification-check workflow. Placeholders like {plugin-name} will not be substituted by GitHub."
title: "[VERIFY] {plugin-name} — active status check"
labels: verification
assignees: ''
---

Hi @{author} 👋

Your plugin **{plugin-name}** (`{repo}`) is listed in the claude-plugins-community registry and is due for its 6-month verification check.

Please confirm one of the following by **{deadline}** (30 days from now):

- [ ] ✅ **Still active** — the plugin is maintained and working with the current version of Claude Code
- [ ] 🗄️ **Archive it** — the plugin is no longer maintained; please archive the GitHub repo too if applicable
- [ ] 🔀 **Transferred** — the plugin has moved to a new repo (provide the new URL)

**No response by {deadline}** will result in the plugin being marked as `archived` in the registry by a maintainer. It will remain installable but show an archived indicator in the plugin browser.

To respond, simply leave a comment on this issue.

---
*This check is part of the [claude-plugins-community verification process](../blob/main/CONTRIBUTING.md#active-verification-6-month-cycle).*
