# Verse-final Words in the Middle English Alliterative *Joseph of Arimathea*

This repository supplies supporting data for the article 'Endings of Half-Lines in the Middle English Alliterative *Joseph of Arimathea*', henceforth abbreviated 'Endings'.

Data are presented in the CSV file `joseph-of-arimathea-scansions.csv`.
Excluding column labels, the file has 709 lines, one for each metrical line of the poem.
Column labels are as follows.

The file `bibliography.yaml` provides bibliographical details (in Better CSL YAML format) for works referenced in this README.

## `line`

Line numbers.

## `text_a`, `text_b`

Text of *Joseph of Arimathea* (a-verse and b-verse).
For reasons of copyright, the text given in these columns is derived from Skeat's 1871 edition, as re-edited within the [*Corpus of Middle English Prose and Verse*](https://quod.lib.umich.edu/c/cme/AHA2700.0001.001).
The division of half-lines agrees with Skeat in every case: see 'Endings' n16.

## `item_a`, `item_b`

The final lexical item in the half-line.
The text is from Scase's 2011 diplomatic transcription of the Vernon manuscript, except

1. prefixes and compounds written separately by the scribe are joined with a hyphen;
2. scribal abbreviations are expanded silently;
3. transcription errors are corrected in lines 68 and 158 of the poem: see 'Endings' n14.

## `prosodel_a`, `prosodel_b`

Tags for the prosodic contour of (the coda of) the verse-final lexical item.
Options are: `trochaic`, `dative_e`, `short_i`, `nonschwa`, and `nontrochaic`.
Tags have the following meanings:

- `trochaic` designates a disyllabic sequence terminated by a word boundary, in which the penult is stressed or stressable and the ultima contains the vowel schwa: see 'Endings', text at nn9--11.
- `dative_e` designates a noun with monosyllabic stem, trochaic on account of dative *-e* as the object of a preposition: see 'Endings', within the section 'Nouns and their Inflections'.
- `short_i` designates an item with a trochaic contour, in which the ultima has short /i/ without consonantal coda: see 'Endings' n36.
- `nonschwa` designates an item that may be stressed on the penult, hence 'trochaic' in the broader sense, but has a full vowel in the ultima.
- `nontrochaic` designates other nontrochaic contours: monosyllables, other oxytones, and proparoxytones.

Several proper nouns of doubtful pronunciation are left untagged.

## `lexel_a`, `lexel_b`

Unique identifiers for lexical items.
Where possible, these are derived from *MED Online* and correspond to the final segment of the URI path for the relevant entry.
Accordingly, *MED* entries may be retrieved by appending the given identifiers to the base path <https://quod.lib.umich.edu/m/middle-english-dictionary/dictionary/>.
For proper nouns not in *MED Online*, identifiers are derived from the Wikidata URI for the corresponding entity.
(This involves a slip from onomastics into ontology.)
For proper nouns recorded in neither authority, the identifier is the prefix `NO_AUTH_` followed by the initial or usual spelling of the item in *Joseph*.

## `grammel_a`, `grammel_b`

Tags for grammatical class and function.
These are a simplified subset of grammel tags employed in *A Linguistic Atlas of Early Middle English*.
See 'Endings' n18.

## `notes`

This column may hold notes on any of the preceding values in the row.
