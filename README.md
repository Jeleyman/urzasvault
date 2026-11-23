# Urza's Vault

A personal browser for my Magic: The Gathering cards, built on Scryfall deck exports.

Import one Scryfall CSV export per deck and Urza's Vault shows everything you own as a card grid. Filter by deck, color, rarity, type, set, or the reserved list; search to check whether you already own a card; sort by name, value, set, mana value, or copies; draw a random card or pick a random deck to play.

## How it works

- Each CSV's file name becomes the deck's name. Importing a file with the same name again replaces that deck.
- Card images, colors, mana value, and current prices come from the [Scryfall API](https://scryfall.com/docs/api), looked up by each card's `scryfall_id` in batches of 75. Card data is saved in the browser and refreshed at most once a day.
- Everything stays in your browser's local storage. Nothing is uploaded anywhere.

## Hosting

It's a single `index.html` with no build step. Push it to a repo with GitHub Pages turned on.

Card data and images from Scryfall. Not affiliated with Scryfall or Wizards of the Coast. Magic: The Gathering is © Wizards of the Coast.
