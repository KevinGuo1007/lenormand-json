# Lenormand JSON

A JSON dataset of the 36 Lenormand cards, inspired by
[metabismuth/tarot-json](https://github.com/metabismuth/tarot-json).

This repository includes:

- `lenormand.json`: card data without image paths
- `lenormand-images.json`: the same card data with image paths
- `lenormand-card/`: public-domain card images from *Das Spiel der Hofnung*

## Source

The card images are derived from
[*Das Spiel der Hofnung (The Game of Hope)*](https://commons.wikimedia.org/wiki/File:Das_Spiel_der_Hofnung_(The_Game_of_Hope).png),
created by Johann Kaspar Hechtel and dated 1799. Wikimedia Commons marks the
source file as public domain.

## Data Shape

Each card entry follows this structure:

```json
{
  "name": "Rider",
  "number": "1",
  "name_zh": "骑士",
  "playing_card": "9 of Hearts",
  "suit": "Hearts"
}
```

`lenormand-images.json` adds an `img` field:

```json
{
  "name": "Rider",
  "number": "1",
  "name_zh": "骑士",
  "playing_card": "9 of Hearts",
  "suit": "Hearts",
  "img": "lenormand-card/Slice 1.png"
}
```

## Usage

```js
const cards = require("./lenormand.json");

console.log(cards.cards[0]);
```

## License

The JSON dataset and repository documentation are available under the MIT
License.

The original card artwork is public domain. See the Wikimedia Commons source
page for the image provenance and public-domain notice.
