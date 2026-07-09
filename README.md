# Microsoft 365 Copilot Prompt Builder

A standalone HTML prompt-building app for creating structured, role-aware prompts for Microsoft 365 Copilot. Designed primarily for user training on how to create prompts in Microsoft 365 Copilot, using the Microsoft GCSE methodology, Goal, Context, Source, Expectation.

The app guides users through prompt construction by combining intent, role context, industry and sub-vertical targeting, expectations, disclaimers, editable placeholders, and a GCSE-style progress flow. It is packaged as a static single-page app, so it can run from GitHub Pages, SharePoint, any static web server, or directly from a local browser.

## Features

- Guided prompt-building flow for Microsoft 365 Copilot
- Industry and sub-vertical targeting
- Role-aware context and expectation suggestions
- Editable prompt placeholders
- Built-in disclaimer and guidance text
- Copy-ready final prompt output
- Link-out support for launching Microsoft 365 Copilot
- Self-contained HTML with JavaScript and CSS inlined

## Run the app

### GitHub Pages

If this repository has GitHub Pages enabled, open:

```text
https://drowe_microsoft.github.io/copilot-prompt-builder/
```

### Local browser

Download or clone the repository, then open `index.html` in a modern browser.

```powershell
git clone https://github.com/drowe_microsoft/copilot-prompt-builder.git
cd copilot-prompt-builder
Start-Process .\index.html
```

### Local web server

Some browsers and security policies behave more consistently when the app is served over HTTP instead of opened from `file://`.

```powershell
cd copilot-prompt-builder
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Deploy elsewhere

Because this is a static app, deployment only requires hosting these files:

- `index.html`
- `favicon.ico`

Upload both files to a static web host, SharePoint document library, Azure Static Web Apps, or another static hosting provider.

## Notes

- The app runs entirely in the browser.
- No build step is required for the packaged version in this repository.
- Microsoft 365 Copilot links require access to Microsoft 365 Copilot in the signed-in tenant.

## License

No open-source license is included in this package. Add a `LICENSE` file before granting reuse, modification, or redistribution rights.
