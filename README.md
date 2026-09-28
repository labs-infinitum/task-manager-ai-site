# task-manager-ai-site

Public pages for **task-manager-ai**, a private self-hosted tool by Infinitum Labs, served with GitHub Pages at
<https://labs-infinitum.github.io/task-manager-ai-site/>.

These exist because Google requires an app home page, privacy policy and terms of service before an
OAuth app that requests Gmail access can be published.

| Page | URL |
|---|---|
| Home | `https://labs-infinitum.github.io/task-manager-ai-site/` |
| Privacy policy | `https://labs-infinitum.github.io/task-manager-ai-site/privacy.html` |
| Terms of service | `https://labs-infinitum.github.io/task-manager-ai-site/terms.html` |
| Slack OAuth callback | `https://labs-infinitum.github.io/task-manager-ai-site/oauth/slack.html` |
| Notion OAuth callback | `https://labs-infinitum.github.io/task-manager-ai-site/oauth/notion.html` |

Plain static HTML and CSS, no build step. Edit a page and push to `main`; Pages redeploys automatically.
If the app's data handling changes (new scopes, new processors), update `privacy.html` and its effective date.

`oauth/slack.html` exists because Slack only redirects to HTTPS URLs: it forwards the one-time
authorization code to the sign-in helper on `127.0.0.1:8767`, reached through an SSH tunnel.
