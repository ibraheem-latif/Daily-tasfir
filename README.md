# Daily Tafsir

Generates a daily summary + full tafsir (Ibn Kathir) for one juz of the Quran, cycling through all 30 juzs.

## Setup

1. Create a GitHub repo and push this code
2. Add your `ANTHROPIC_API_KEY` as a repository secret (Settings → Secrets → Actions)
3. Enable GitHub Pages (Settings → Pages → Source: "GitHub Actions")
4. The workflow runs daily at 5 AM UTC, or trigger manually from the Actions tab

## Local usage

```bash
export ANTHROPIC_API_KEY=sk-...
pip install -r requirements.txt
python generate.py              # auto-selects today's juz
JUZ_NUMBER=1 python generate.py # override specific juz
```

Output goes to `site/index.html` and `site/juz-{n}.html`.

## Share

Send the GitHub Pages URL to your WhatsApp group. The page has a built-in WhatsApp share button.
