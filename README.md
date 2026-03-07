# @tclohm/car-colors

A comprehensive ESM module of car colors, organized by category with utility functions.

## Install

```bash
npm install @tclohm/car-colors
```

## Usage

```js
import carColors, { blues, findByName, randomColor } from '@tclohm/car-colors';

// Get all colors
console.log(carColors.allColors);

// Get all blues
console.log(blues);

// Search by name
console.log(findByName('midnight'));     // { name: 'Midnight Black', hex: '#1C1C1C' }

// Get a random color
console.log(randomColor());             // { name: 'Soul Red', hex: '#B22222' }
```

## Categories

| Category    | Description                            |
|-------------|----------------------------------------|
| `whites`    | White tones (polar, pearl, ivory…)     |
| `silvers`   | Silver tones (lunar, platinum, sonic…) |
| `blacks`    | Black tones (jet, obsidian, carbon…)   |
| `grays`     | Grays (graphite, nardo, gunmetal…)     |
| `blues`     | Blues (navy, cobalt, portimao…)        |
| `reds`      | Reds (rosso corsa, crimson, candy…)    |
| `greens`    | Greens (british racing, lime…)         |
| `yellows`   | Yellows (racing, sunburst, dakar…)     |
| `golds`     | Golds (metallic, champagne, amber…)    |
| `oranges`   | Oranges (blaze, volcanic, copper…)     |
| `browns`    | Browns (mocha, chestnut, walnut…)      |
| `purples`   | Purples (ultraviolet, midnight…)       |
| `pinks`     | Pinks (hot pink, sakura, rose…)        |
| `specialty` | Special finishes (matte, chrome, candy…) |

## API

### `allColors`
Flat array of every color object `{ name, hex }`.

### `categories`
Object containing all category arrays.

### `findByName(name)`
Returns the first color whose name contains the search string (case-insensitive).

### `searchByName(name)`
Returns all colors whose name contains the search string.

### `findByHex(hex)`
Returns the color matching the given hex code exactly.

### `getCategory(category)`
Returns the array of colors for a given category name string.

### `getCategoryNames()`
Returns an array of all category name strings.

### `randomColor()`
Returns a random color from the full list.

## License
MIT
