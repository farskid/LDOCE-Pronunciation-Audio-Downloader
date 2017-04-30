# LDOCE Pronunciation Audio Downloader
> A Node.js tool to download both British and American pronunciation of vocabularies from Longman Dictionary of Contemporary English (http://www.ldoceonline.com)

## Heads UP!
This was initialy a fork of [jmosawy Fork](https://github.com/jmosawy/LDOCE-Pronunciation-Audio-Downloader) project, but has been provided an API and an online website for better usage experience.
The website can be found at [Longman API](https://longman-api.herokuapp.com/).

## API
It also adds an API on top of the crawling service with a single endpoint:
```
const getWordPronounciation = (word) => {
  return fetch('https://https://longman-api.herokuapp.com/pronounce?word')
    .then(res => res.json())
    .then(res => res)
    .catch(e => alert(e))

const fantastic = getWordPronounciation('fantastic')
console.log(fantastic); // prints {american: 'Some_URL.mp3', british: 'Some_other_url.mp3'} to console
}
```

## Description

This tool is built for educational purposes, plus it'd be useful for anyone who's looking for getting the most correct word pronunciations.

## How to Use
You may clone this project, and then run the following command to get all dependencies:

`npm install`

After that, you may use the following command to get both American and British pronunciation of a :WORD:

`node index.js ':word:'`

**Please Note:** include your word in a single quote.
