# MenstruAI — Menstrual Health & Cycle Tracker

MenstruAI is a browser-based menstrual health companion that combines period logging, cycle estimates, educational material, and an AI chat interface in a single-page web app.

## Features

- **Cycle tracking:** Record period start dates and daily notes, symptoms, flow, and mood where supported by the app.
- **Calendar and estimates:** View historical entries and estimates for upcoming periods and fertile windows.
- **Cycle insights:** Review average cycle metrics and trends from recorded history.
- **Health education:** Browse material about menstrual hygiene, symptoms, common myths, and self-care.
- **AI chat:** Ask menstrual-health questions through the configured external AI endpoint.
- **Data export:** Export local records for personal backup where supported.

## Technology

- HTML5, CSS, and vanilla JavaScript
- Browser `localStorage`
- External AI API integration
- Static single-page application

## Run locally

No package installation is required for the static page itself.

```bash
git clone https://github.com/nksdev/privacy-first-cycle-tracker.git
cd privacy-first-cycle-tracker
python -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000) in a browser.

You can also open `index.html` directly, although browser restrictions may affect external API requests. The Android download link in older documentation should be verified before use; this repository does not itself prove that an app-store build is current or maintained.

## Privacy and data handling

- Cycle records stored in `localStorage` remain in that browser profile and are not automatically synchronized across devices.
- Anyone with access to the unlocked browser profile may be able to view stored records.
- Clearing site data can erase records; export a backup if the application provides that feature.
- The AI chat sends prompts to an external API endpoint. **Do not assume that all data remains on-device**; avoid sending personally identifying or sensitive health information unless you have reviewed the provider's privacy terms.
- Cycle and fertile-window predictions are estimates and may be inaccurate, especially with irregular cycles. This application is not a diagnostic tool or a substitute for a qualified healthcare professional.

## Project structure

```text
privacy-first-cycle-tracker/
├── index.html   # Main web application
├── icon.png     # App icon
├── README.md    # Project documentation
└── LICENSE      # License
```

## Responsible use

Use the tracker as an informational aid, keep backups of records you need, and consult a healthcare professional for medical concerns or decisions.

## Maintainer

[Naman Kumar Sonker](https://github.com/nksdev)

## License

See [LICENSE](LICENSE).
