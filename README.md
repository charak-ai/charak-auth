# Charak OAuth Redirect

This is a simple redirect page for the Charak medical AI assistant app.

It receives OAuth callbacks from healthcare providers (Epic/MyChart) and redirects them to the Charak desktop app using a custom URL scheme.

## How it works

1. User authenticates with their healthcare provider (Epic)
2. Epic redirects to `https://hbatmit.github.io/charak-auth/?code=...&state=...`
3. This page redirects to `charak://callback?code=...&state=...`
4. The Charak desktop app receives the OAuth tokens

## Setup

1. Fork or clone this repo
2. Enable GitHub Pages in Settings → Pages
3. Set source to "Deploy from a branch" → main → / (root)
4. Your redirect URL will be: `https://hbatmit.github.io/charak-auth/`
