# words

A copy of `/usr/share/dict/words` from macOS 26.6.2.

The file is the classic `web2` word list derived from Webster's Second
International Dictionary (1934), which is in the public domain. It is the
list used by `look`, `spell`, and similar Unix tools.

## Format

- One word per line, plain ASCII, newline-terminated.
- 235,976 entries.
- Sorted case-insensitively, so `A`, `a`, `aa`, `aal` appear together.
- About 25,000 entries are capitalized proper nouns (`Aani`, `Zyzzogeton`).

## Usage

```sh
# Look up words with a prefix
look zyz words

# Pick a random word
shuf -n 1 words

# Find 7-letter words ending in "ing"
grep -E '^.{4}ing$' words
```
