Look at the screenshot the user has provided (from Maya's French-German textbook).

Extract every French–German vocabulary pair you can find. Also extract example sentences if they are present next to a word.

Output ONLY a plain text block in this exact format — one word pair per line, nothing else before or after the block:

```
FRENCH_WORD = GERMAN_WORD | FRENCH_EXAMPLE_SENTENCE | GERMAN_EXAMPLE_SENTENCE
```

Rules:
- If there is no example sentence, omit everything after the first `=`: just `FRENCH_WORD = GERMAN_WORD`
- If there is an example sentence in French but not German (or vice versa), still include what you have and leave the other side empty: `la gare = der Bahnhof | Où est la gare ? |`
- Keep articles with the noun: `la gare`, `der Bahnhof`, `un CDI`
- Do not include page numbers, phonetic transcriptions, section headers, or grammar tables
- Do not include the clock/time phrases (those are handled by the L'heure tab)
- Preserve accents exactly: é, è, ê, ë, à, â, ù, û, ô, î, ï, ç, œ, æ

After the block, add a short line saying how many pairs were found and remind the user to paste them into the app's **Words → Bulk Import** field (they can use the `=` and `|` separators).
