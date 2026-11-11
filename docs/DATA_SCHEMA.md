# Data schema

Mỗi file import có dạng:
```json
{"book": {...}, "units": [...], "items": [...], "relations": [...]}
```

## Book
`id`, `title`, `subtitle`, `level`, `publisher`, `edition`, `language`, `description`.

## Unit
`id`, `bookId`, `number`, `title`, `category`, `summary`.

## Item
Bắt buộc: `id`, `bookId`, `unitId`, `type`, `headword`, `meaningVi`.
Khuyến nghị: `partOfSpeech`, `ipa`, `meaningEn`, `examples`, `collocations`, `synonyms`, `antonyms`, `tags`, `level`, `sourceRef`.

`type`: vocabulary, phrase, collocation, phrasal_verb, grammar, idiom.

## Relation
`sourceId`, `type`, `targetId`; type gồm synonym, antonym, family, collocation, topic, related.
