# Smash Up Data JSON

This repository contains a JSON file (`smashUpData.json`) that provides structured information about the various sets and factions from the popular card game, *Smash Up*. This README explains the structure and meaning of the data within this file.

## File Structure

The `smashUpData.json` file is a single JSON object with two main top-level keys:

* `version`: The version number of the data schema.

* `sets`: An array of objects, each representing a *Smash Up* game set (base game, expansion, promo, etc.).

* `factions`: An array of objects, each representing a specific faction available in *Smash Up*.

## Key Definitions

### Top-Level Keys

* **`version`** (Number):

  * Indicates the version of the `smashUpData.json` schema. This can be useful for tracking changes or ensuring compatibility with applications that consume this data.

* **`sets`** (Array of Objects):

  * Each object in this array describes a particular *Smash Up* set.

* **`factions`** (Array of Objects):

  * Each object in this array describes a specific faction.

### `sets` Array Object Keys

Each object within the `sets` array has the following keys:

* **`id`** (Number):

  * A unique numerical identifier for the set.

* **`name`** (String):

  * The official name of the *Smash Up* set (e.g., "Core Set", "Awesome Level 9000").

* **`type`** (String):

  * Categorizes the type of set. Possible values include:

    * `"base"`: The original core game.

    * `"expansion"`: A standard expansion adding new factions and bases.

    * `"standalone"`: A complete game that can be played on its own or combined with other *Smash Up* sets (e.g., "Smash Up: Munchkin").

    * `"promo"`: A promotional set, often containing a single faction or special cards.

    * `"storage"`: A box primarily for storing cards, sometimes including a new faction.

* **`status`** (String):

  * Indicates the current status of the set. Possible values:

    * `"active"`: The set is currently in production and widely available.

    * `"discontinued"`: The set is no longer actively produced.

* **`releaseDate`** (String):

  * The original release date of the set, in `YYYY-MM-DD` format.

* **`factionCount`** (Number):

  * The number of new factions introduced in this set. For sets like "TITANS" or "Dead Reckoning Promo", this might be 0 as they add other game components.

* **`description`** (String):

  * A brief summary or description of the set.

### `factions` Array Object Keys

Each object within the `factions` array has the following keys:

* **`id`** (Number):

  * A unique numerical identifier for the faction.

* **`name`** (String):

  * The official name of the faction (e.g., "Aliens", "Dinosaurs", "Robots").

* **`setId`** (Number):

  * The `id` of the set to which this faction originally belongs. This links the faction back to its release set in the `sets` array.

* **`theme`** (String):

  * A general theme or category for the faction (e.g., "Sci-Fi", "Horror", "Fantasy", "Japanese").

* **`description`** (String):

  * A brief overview of the faction's primary mechanics or playstyle.

## Usage

This JSON data can be used by applications, tools, or scripts that need to reference or display information about *Smash Up* sets and factions, such as:

* Collection trackers

* Random faction generators

* Fan-made apps or websites

* Data analysis of *Smash Up* content

Feel free to use and contribute to this data!
