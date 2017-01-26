## nrc-sentiment
#### NRC Word-Emotion Lexicon based sentiment analysis for Node.js

NRC Sentiment is a Node.js module that uses the [NRC Word-Emotion Lexicon](http://saifmohammad.com/WebPages/NRC-Emotion-Lexicon.htm) wordlist to perform [sentiment analysis](http://en.wikipedia.org/wiki/Sentiment_analysis) on arbitrary blocks of input text. NRC Sentiment provides:

- A build process that makes updating sentiment to future versions of the word list trivial

### Installation
```bash
npm install git://github.com/jeremylind/nrc-sentiment
```

### Usage
```javascript
var sentiment = require('nrc-sentiment');

var r1 = sentiment('Cats are stupid.');
console.dir(r1);        // Score: -2, Comparative: -0.666

var r2 = sentiment('Cats are totally amazing!');
console.dir(r2);        // Score: 4, Comparative: 1
```
