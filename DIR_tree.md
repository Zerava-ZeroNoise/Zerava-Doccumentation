```markdown
# Zerava MVP – Full Project Tree Structure

Below is the **clean, full tree-style folder structure** exactly how it would appear using the `tree` command. No abstractions, no fluff, just reality.

```

zerava-mvp/
├── README.md
├── .gitignore
│
├── frontend/
│   ├── package.json
│   ├── public/
│   │   ├── index.html
│   │   └── favicon.ico
│   │
│   └── src/
│       ├── components/
│       │   ├── Button.jsx
│       │   ├── Card.jsx
│       │   └── ProgressBar.jsx
│       │
│       ├── pages/
│       │   ├── LandingPage.jsx
│       │   ├── ScanPage.jsx
│       │   └── ResultsPage.jsx
│       │
│       ├── services/
│       │   └── api.js
│       │
│       ├── styles/
│       │   ├── main.css
│       │   └── theme.css
│       │
│       ├── App.jsx
│       └── index.jsx
│
└── backend/
├── run.py
├── config.py
├── requirements.txt
│
└── app/
├── **init**.py
│
├── routes/
│   ├── **init**.py
│   ├── scan_routes.py
│   └── status_routes.py
│
├── scanners/
│   ├── **init**.py
│   ├── https_checker.py
│   ├── ssl_tls_checker.py
│   ├── security_headers.py
│   ├── open_ports.py
│   └── owasp_top10.py
│
├── scoring/
│   ├── **init**.py
│   └── score_calculator.py
│
├── models/
│   ├── **init**.py
│   ├── scan.py
│   ├── finding.py
│   └── report.py
│
└── utils/
├── **init**.py
└── job_queue.py

```

### Why this works
- Matches your **API-first, async, MVP-only** philosophy
- Keeps hacking tools isolated and auditable
- Frontend stays dumb, backend stays smart
- No premature scaling nonsense

This is something you can build in days, not months, and still not regret later.
```
