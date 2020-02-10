# English Thesaurus in JSON

I looked *everywhere* for an english thesaurus in JSON format (for spinning/bots/experiments) and had a hard time finding a decent one. This one was a pretty good attempt.

I managed to create it by scraping and cleaning an english thesaurus in plain text

## Usage
```js

const thesaurus = require('thesaurus.json');

// just as an example
const word = 'exit';

// the thesarus is keyed by noun, verb, adjective, then by word
const replacements = thesarus.n[word]

// choose a random term
const index = Math.floor(Math.random() * replacements.length);

console.log(replacements[index]);

```

The structure of the thesaurus was chosen so that lookup can be performed in O(1) time
