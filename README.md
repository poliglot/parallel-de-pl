# Bilingual German-Polish corpora
This is a collection of parallel corpora for German -> Polish.

## Sentence corpus
The sentence corpus contains aligned sentences taken from the OpenSubtitles dump ``de-pl.tmx`` (15th November 2013).

The majority of the sentences were selected with the bias of containing at least one of these German adpositions:

> an, auf, in, mit, nach, um, zu, über

Each sentence was given a flag indicating its viability, however a more permissive metric was used in the beginning of the annotation process.

As of January 2015 it contains 481 sentences (261 bad, 220 good).

## Semantic entities
It contains all sentences from the sentence corpus equipped with morphological tags (RFTagger was used for German and concraft-pl for Polish sentences).

Then, all sentences were annotated with regards to:

a) semantic entities; represented as a hierarchy
b) dependencies between entities
c) alignment of source into target entities
d) semantic tags for German adpositions (see below)

Statistics (January 2015):

- Sentences: 220
- Aligned sentences: 220
- Total entities: 2892
- Aligned entities: 1187
- Dependencies: 196
- German tokens (total): 2220
- Polish tokens (total): 1911

## Lemma corpus
This contains manually aligned lemmas which appear in the sentence corpus. Its purpose is to improve statistic models by providing an additional information source. As of now, the entries do not contain morphological tags or reflexive markers (sich/się).

## Classes
This is the tagset that was used for annotating the adpositions.

## Language resources
Additional language resources used by other components of Poliglot must be obtained manually, these are:

- ``de-pl.tmx``: OpenSubtitles dump
- ``dictcc-de-pl.txt``: dict.cc dump for German-Polish translations

## See also
* [Poliglot corpus editor](https://github.com/poliglot/poliglot-ui)
* [OpenSubtitles website](http://www.opensubtitles.org/)
* [OpenSubtitles dumps](http://opus.lingfil.uu.se/OpenSubtitles.php)
* [dict.cc dumps](http://www1.dict.cc/translation_file_request.php)

## License
Poliglot is licensed under the terms of the Apache v2.0 license.

## Authors
- Tim Nieradzik
