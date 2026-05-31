# Insurance AI Learning Library Share

Shareable bilingual MkDocs Material site for insurance POS, sales journey AI, BRD reformatting, and AI use case prioritisation.

This is a sanitized Traditional Chinese + English learning and discussion library. It does not include raw notes, personal preparation details, or client-specific source material.

Traditional Chinese is the default language. English is available through the language switcher in the MkDocs Material header.

## Local Preview

From this folder:

```bash
python3 -m pip install -r requirements.txt
mkdocs serve
```

Then open:

```text
http://127.0.0.1:8000
```

Use the language selector in the top navigation to switch between:

- 繁體中文
- English

## Build Static Site

```bash
mkdocs build
```

The generated static site will be created in `site/`.

## Vercel Deployment

1. Push this folder to a Git repository.
2. In Vercel, create a new project from the repository.
3. Use the following settings:
   - Framework Preset: Other
   - Build Command: `pip install -r requirements.txt && mkdocs build`
   - Output Directory: `site`
4. Deploy.

## Notes

The site is intended for learning and discussion only. It is not client advice, legal advice, compliance advice, or an official project recommendation.
