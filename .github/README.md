# GitHub Actions Setup

## Workflows

### deploy.yml
Builds and deploys the Quartz site to GitHub Pages on push to `v4` branch.

### social-post.yml
Posts new blog articles to social media when markdown files are added to `content/`.

## Required Secrets

Go to **Settings > Secrets and variables > Actions** to add these:

### Bluesky

| Secret | Description |
|--------|-------------|
| `BLUESKY_IDENTIFIER` | Your Bluesky handle (e.g., `yourname.bsky.social`) |
| `BLUESKY_PASSWORD` | App password from Bluesky Settings > App Passwords (not your main password) |

### Twitter/X

Get these from [developer.twitter.com](https://developer.twitter.com):

| Secret | Description |
|--------|-------------|
| `TWITTER_API_KEY` | Consumer API key |
| `TWITTER_API_SECRET` | Consumer API secret |
| `TWITTER_ACCESS_TOKEN` | Access token |
| `TWITTER_ACCESS_SECRET` | Access token secret |

Note: Twitter's free API tier allows 1,500 posts/month.
