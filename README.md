# Startpage

A simple browser start page that reads bookmarks from a YAML file or from a Raindrop.io collection and displays them grouped by tag.

## Usage

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Sources

### YAML (default)

Edit `bookmarks.yaml`:

```yaml
- name: GitHub
  url: https://github.com
  tags: [dev, tools]
```

### Raindrop.io

1. Get a test token at [app.raindrop.io/settings/integrations](https://app.raindrop.io/settings/integrations)
2. Create a collection named `startpage` and add bookmarks to it
3. Click the gear icon ⚙️ in the page header
4. Select **Raindrop.io**, paste your token, click **Test Connection**, then **Save & Close**

## Features

- Bookmarks grouped by tag into cards
- Click a tag pill to filter; click again to clear
- Search filters by name or URL in real time
- Dark/light toggle (persisted in localStorage)