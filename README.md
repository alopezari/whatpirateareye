# What Pirate Are Ye?

Answer a few questions and get your own pirate trading card: a name, a portrait, attacks and a bounty, ready to share.

Live at **https://whatpirateareye.view.fast**

## How it works

Everything is one static file, `index.html`, and runs in the browser. There is no server and no AI model:

- Your answers seed a random generator, so the same answers plus the same roll always give the same card. That is how share links work: the answers are encoded in the URL hash.
- Names, attacks, abilities and flavour text are built from word banks combined at random, so cards rarely repeat.
- The portrait is drawn on a canvas in code: shapes, ink lines, paper grain.

## Run it locally

```sh
python3 -m http.server 8765
```

Then open http://localhost:8765.

## Deploy

Hosted on [Spacefast](https://spacefast.com):

```sh
sf publish .
```

`.spacefast/space.json` links this folder to the space.
