# Break Things Safely

Source for breakthingssafely.com — a free cyber security learning pathway.

## Local preview

```bash
pip install mkdocs mkdocs-material
mkdocs serve
```

Then open http://127.0.0.1:8000

## Deploying

This is set up to deploy on Cloudflare Pages:

1. Push this repo to GitHub.
2. In Cloudflare Pages, create a project connected to the repo.
3. Build command: `pip install mkdocs-material && mkdocs build`
4. Build output directory: `site`
5. Add `breakthingssafely.com` as the custom domain in the Pages project settings.
