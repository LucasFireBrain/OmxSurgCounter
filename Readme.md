# OmxSurgCounter

## Overview
OmxSurgCounter is a lightweight web tool that helps surgical teams record the consumables used during a procedure. The single-page app lets you choose a surgery, search the appropriate price list, and compile the final count for export. It was designed as a quick prototype, so everything runs entirely in the browser without a backend.

## Features
- **Surgery selection:** pick a procedure code to automatically load the corresponding price list.
- **Guided product search:** type to filter items by internal code, global code, or description before adding them to the count.
- **Editable register:** adjust product codes, replace products, or change quantities directly in the table.
- **JSON export:** copy the compiled count to the clipboard or download it as a structured JSON file for record keeping.
- **Easy reset:** clear the form to start documenting a new surgery.

## Project structure
- `index.html` – the main interface and all client-side logic for managing surgeries, products, and exports.
- `products.json` – reference catalog that maps global product identifiers to list-specific codes.
- `listC.txt` – raw reference list that can be imported to extend the in-browser catalog.

## Getting started
1. Open `index.html` in your browser. No build step or server is required.
2. Choose a surgery from the dropdown to enable search and entry fields.
3. Search for products, add them to the register, edit as needed, then export or reset the session.

To customize the catalog, update the `surgeries` or `products` arrays inside `index.html`, or replace them with data loaded from `products.json` or other sources.
