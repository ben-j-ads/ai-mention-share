# AI Mention Share

Ask an AI assistant about your category. Count who shows up, in which situations, and how often. Paste the answers an assistant gave to a set of category prompts, list the brands you track, and get each brand's share of answers, share of mentions, how often it is named first, and how many buying situations it appears in.

Open `index.html` in any browser. No build step, no dependencies, and no API: you collect the answers yourself and nothing leaves your browser.

- **Prompt maker:** enter a category and a list of situations, get neutral prompts with no brand names in them. The situations are your category entry points.
- **Input:** answers pasted under `=== Assistant | prompt` header lines. The tool matches brands and their other spellings case-insensitively, whole words only.
- **Measures:** answers mentioning the brand (with a Wilson range), share of mentions, named first, and situations covered (the safer one, since repeat answers to one prompt are not independent).
- **Verdict:** `ahead`, `behind`, `level`, `invisible` or `too few answers`. It compares you with the best-mentioned rival using a paired difference over the same answers.
- **Also shows:** a brand by situation table, a brand by assistant table, and capitalised names that may be competitors you left off the list.
- **Share:** a paper-ground PNG card, and the URL hash carries your settings and brand list (not the pasted answers).

Answers change with the model version, the day, location, chat memory and whether the assistant searched the web, so date every result and re-run before calling anything a trend. A mention is not praise: the tool cannot read tone. Nothing found shows that being mentioned by an assistant moves sales. This borrows from mental availability (how many buying situations bring a brand to mind) as a proxy, and an assistant's answer is not a buyer's memory.

## License

Code is MIT licensed ([LICENSE](LICENSE)). The bundled fonts (Bricolage Grotesque, Archivo) are SIL OFL 1.1, with licenses in `fonts/`. The ben.j.ads wordmark and footnote mark in `logo/` are Ben Johnston's brand assets and are not covered by the MIT license.
