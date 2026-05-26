# Yorùbá Alphabet System

Àkọsílẹ̀ yí ṣe àfihan kíkọ ọ̀rọ̀ Yorùbá ní ìlana for Natural Language Processing (NLP), including letters, digraphs, and tonal markings.

---

## 1. Vowels

Yorùbá has 7 basic vowels:

a, e, ẹ, i, o, ọ, u

### Notes:
- Vowels may carry tone marks.
- ẹ and e are distinct sounds.
- ọ and o are distinct sounds.
- ṣ and s are distinct sounds.

---

## 2. Consonants

b, d, f, g, gb, j, k, l, m, n, p, r, s, ṣ, t, w, y

### Notes:
- gb is a single consonant sound (labio-velar stop)
- ṣ is different from s (sh-like sound)

---

## 3. Digraphs (Single Sound Units)

- gb
- kp (used in some dialectal contexts)
- ny (nasal sound in some usage contexts)

---

## 4. Tone System

Yorùbá is a tonal language with 3 main tones:

| Tone | Mark | Example |
|------|------|--------|
| High | ´ | á, é, ẹ́, í, ó, ọ́, ú |
| Low  | ` | à, è, ẹ̀, ì, ò, ọ̀, ù |
| Mid  | (no mark) | a, e, ẹ, i, o, ọ, u |

---

## 5. Tone Importance

Tone changes meaning completely:

- ọkọ́ (vehicle)
- ọkọ̀ (husband)
- ọkọ (context-dependent/neutral usage)

---

## 6. Writing Rules

- Words are written left to right.
- Tone marks must be preserved in NLP datasets.
- e ≠ ẹ and o ≠ ọ must never be merged.
- gb is treated as a single phoneme, not two letters.

---

## 7. NLP Guidelines

For machine learning systems:

- Preserve diacritics during preprocessing
- Do not strip tone marks
- Tokenizers must recognize digraphs (gb, ṣ)
- Tone is a semantic feature, not decoration

---

## 8. Purpose

This alphabet specification is designed to support:
- NLP preprocessing
- Tokenization
- POS tagging
- Machine translation
- Future LLM training for Yorùbá language
