# authorwebsite

Content for www.theworldsgreatestwriter.com. The site itself is hosted on SiteGround. Its pages read these files straight from GitHub, so editing a file here updates the live site without touching SiteGround.

| File | What it controls |
|---|---|
| `data/events.json` | "Upcoming" on the home page. Past events drop off by themselves. |
| `data/stories.json` | The list on the Stories page, newest first. |

## Adding an event or story

1. Open the file above on github.com and click the pencil icon.
2. Copy an existing entry from `{` to `}`, paste it after a comma, and change the details. Set `"hidden": false`, or delete that line.
3. Click **Commit changes**. The live site picks it up within about five minutes.

Dates use `YYYY-MM-DD`. Event fields: `date`, `time`, `title`, `place`, `url`, `note`. Story fields: `title`, `venue`, `year`, `url`, `note`. Only `title` is required.

If a list on the site says it couldn't load, the file usually has a missing comma or quote mark. Paste it into jsonlint.com to find the problem.

This repo must stay **public** for the site to read it.
