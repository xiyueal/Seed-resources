# Seed 思得 downloadable resources

Versioned vocabulary, lexical relation and audio resources for Seed 思得.
This repository contains data and recordings only; the app source is separate.

Files are fetched on demand and validated against the app's SHA-256 catalog.
The vocabulary supports 5,558 exam headwords. The lexical corpus contains
30,000 word/component nodes and 740,895 typed relation records.

Sources, versions, attributions, modification notes and full license text are
included in the downloaded network header and LICENSES.md. Etymological links,
modern word formation, synonyms, antonyms and spelling similarities remain
separate types; limited coverage does not imply a relation does not exist.

The generated audio manifest is retained in the private source project; these
MP3 recordings are downloadable assets for the same app, not an online TTS API.

The downloadable relation format is tuple-v2. It retains the original relation fields and includes explicitly sourced target-definition/POS evidence; absent reverse evidence stays empty.
