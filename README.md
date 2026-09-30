# SAT Prep

SAT flashcard trainer, hosted on GitHub Pages.

- `index.html` — the app
- `questions.json` — the question bank. Add or edit questions here; the app loads it on every visit.

Required fields per question: `id`, `section`, `category`, `difficulty`, `type`. If the JSON is invalid the app silently falls back to an older inline bank, so validate before pushing:

    python3 -m json.tool questions.json > /dev/null && echo OK
