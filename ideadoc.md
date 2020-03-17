# Untranslatable

Untranslatable is a knowledge base of untranslatable terms from different languages. Browse them for your edutainment!

## Interface



## Data models

The central entity in untranslatable is the `term`.

A term has

    - one original_latin The term in its original language but written in latin script

    - one original_term The term in its original language and its original script

    - one language Reference to the original language

    - one script Reference to the original script

    - one phonetic The term's pronunciation in the International Phonetic Alphabet

    - many descriptions

A Description has

    - one body The actual description

    - one language the description is written in

A Language has

    - one name of the language in English

    - one own_name The name of the language in that language

A script has

    - one name


**Example**

```
Term
.original_latin: cafuné
.original_term: cafuné
.language: Portuguese
.script: latin
.phonetic: /ˌka.fu.ˈnɛ/
.descriptions:
   - .body: The act of tenderly running one’s fingers through someone’s hair.
     .language: English
   - .body: Acto de acariciar el cabello de alguien
     .language: Spanish
```
