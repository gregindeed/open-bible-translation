# Open Bible Translation

An open Bible translation made directly from the Hebrew and Greek, drafted with
AI, checked automatically, and reviewed by people — with the full history of
every verse in public. Free for anyone to use under
[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).

**Status: draft.** Nothing here has been reviewed by the committee yet. Every
verse carries its status (`draft`, `reviewed`, `approved`).

## Editions

- **Versión Testigo** (es): Rut (85 verses)
- **Open Bible Translation** (en): Ruth (85 verses)

Read them online at [witness-archive.org/bible/obt](https://witness-archive.org/bible/obt)
(English) and [witness-archive.org/bible/vt](https://witness-archive.org/bible/vt) (Spanish).

## Free JSON API

No key, no sign-up. Files are served from GitHub through jsDelivr:

```
https://cdn.jsdelivr.net/gh/gregindeed/open-bible-translation@main/v1/editions.json            all editions and books
https://cdn.jsdelivr.net/gh/gregindeed/open-bible-translation@main/v1/obt/mark.json            a whole book
https://cdn.jsdelivr.net/gh/gregindeed/open-bible-translation@main/v1/obt/mark/1.json          one chapter
https://cdn.jsdelivr.net/gh/gregindeed/open-bible-translation@main/v1/vt/ruth/1.json           Spanish (Versión Testigo)
https://cdn.jsdelivr.net/gh/gregindeed/open-bible-translation@main/v1/obt/mark/history.json    every revision, with who and why
```

Each verse: `{ "verse": 1, "text": "…", "notes": [{ "type": "meaning", "text": "…" }], "status": "draft" }`.
Book files use the OSIS book id in lowercase (`gen`, `ruth`, `mark`, `1cor`, …).

## How it is made

1. **Drafted from the original.** An AI translates each verse from the
   Hebrew/Greek words alone, with Strong's numbers, grammar tags and
   dictionary glosses, following the public style guide and glossary in
   `editions/<edition>/`. It is never shown a published translation.
2. **Checked.** Glossary and name rules, style rules, a scan for wording
   copied from other Bibles, and a back-translation compared with the Berean
   Standard Bible (public domain).
3. **Reviewed by people.** Every correction is recorded with the reviewer's
   name and reason (`history.json`).

## Sources

- Old Testament: Westminster Leningrad Codex (public domain)
- New Testament: SBL Greek New Testament, © Society of Biblical Literature and Logos Bible Software (CC BY 4.0)
- Comparison only: Berean Standard Bible (public domain)

## License and attribution

The translation text, notes, style guides and glossaries are licensed under
[Creative Commons Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/).
You may copy, share, adapt and build on them for any purpose, including
commercially, as long as you give credit and share changed versions under the
same license. Suggested credit:

> Open Bible Translation (OBT), github.com/gregindeed/open-bible-translation — CC BY-SA 4.0

## Contributing

Found a mistake, or want to help review? Open an issue on this repository —
please give the verse, the problem and, where you can, the Hebrew or Greek
behind it.

---

This repository is generated from the Witness Archive translation pipeline
(`scripts/vt/export.mjs`). Last export: 2026-11-02.
