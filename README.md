# flashcards
A simple JavaScript web app for learning Latin vocabulary

## FlashCardView:
This is both the view and controller. It draws everything inside a fixed-size Canvas.
There’s no CSS or DOM interaction. To change the layout or look, you have to change the code.
It contains an array of model class instances. Each model instance implements these functions:
* *getWordCount* — returns the number of words it contains
* *getWordRendering* — returns a string that contains a specific rendering of a word
* *getWordDefinition* — returns a string that contains the English translation of a word
* *getGender* — returns the gender of the words it contains
* *getDeclension* — returns the declension of the words it contains
* *getDescription* — returns a string containing the name of model (for use in a menu)

## Models:
* *Nouns1stDeclension* — 1st declension nouns
* *Nouns2ndDeclensionMasc* — 2nd declension masculine nouns
* *Nouns2ndDeclensionNeut* — 2nd declension neuter nouns

## Utils:
A class containing some handy static functions.
* *getRandomInt* — returns a random integer value that’s between two integer values
* *getElementFromID* — returns a DOM element that has a unique ID string
* *setButtonText* — replaces the label text of an HTML "button" element
* *showElement* — makes an HTML element visible
* *hideElement* — makes an HTML element invisible

## Number:
A class that describes a Latin noun’s "number" case, whether singular or plural.

## Case:
A class that describes the Latin noun cases, from *Nominative* through *Ablative*.

## Gender:
A class that describes a Latin noun’s gender, whether *masculine*, *feminine* or *neuter*.

## Declension:
A class that describes a Latin noun’s declension, from *1st* through *4th*.
