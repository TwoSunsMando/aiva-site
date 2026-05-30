# aiva-site

Client site for **aivadealerteams.ai**.

- Single self-contained HTML file (`index.html`). All images are base64-embedded;
  the only external requests are to Google Fonts.
- **Content is read-only.** Do not modify, reformat, or "improve" the HTML.
  Treat the file as a delivered artifact from the client.
- Hosted on Coolify (`coolify.astridagent.ai`, droplet `159.203.174.128`),
  same git-push &rarr; redeploy workflow as `sde-tech.com`.
- DNS is managed in the **client's** GoDaddy account.
- Apex `aivadealerteams.ai` is canonical; `www.` redirects to apex.

## Local preview

```bash
docker build -t aiva-site .
docker run --rm -p 8083:80 aiva-site
# open http://localhost:8083/
```
