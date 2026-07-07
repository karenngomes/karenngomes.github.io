# karenngomes.github.io

[![Deploy site](https://github.com/karenngomes/karenngomes.github.io/actions/workflows/deploy.yml/badge.svg)](https://github.com/karenngomes/karenngomes.github.io/actions/workflows/deploy.yml)

Personal academic homepage of **Karen Gomes** — Master's student in Computer Science at UFMG (LoCuS lab).

🔗 **Live site:** [karenngomes.github.io](https://karenngomes.github.io)

## What's here

- `/` — about, bio, and news
- `/publications/` — papers, generated from `_bibliography/papers.bib`
- `/cv/` — résumé, generated from `assets/json/resume.json`
- `/blog/` — posts

## Built with

This site is based on [al-folio](https://github.com/alshedivat/al-folio) (v0.16.3), a Jekyll theme for academics, hosted on GitHub Pages and deployed automatically via GitHub Actions on every push to `main`.

## Running locally

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`.

## License

Theme code is MIT-licensed, © [Maruan Al-Shedivat](https://github.com/alshedivat) and the al-folio contributors — see [LICENSE](LICENSE).
