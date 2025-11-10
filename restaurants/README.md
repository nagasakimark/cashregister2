# Restaurant Structure

Each restaurant has its own folder with the following structure:

```
restaurants/
├── horizon/
│   ├── menu.json          # Restaurant configuration and menu items
│   └── products/          # Product images for this restaurant
│       ├── rice.png
│       ├── sushi.png
│       └── ...
├── fastfood/
│   ├── menu.json
│   └── products/
├── japanese/
│   ├── menu.json
│   └── products/
└── cafe/
    ├── menu.json
    └── products/
```

## Menu.json Structure

Each `menu.json` file contains:

```json
{
  "name": "Restaurant Name",
  "icon": "🍔",
  "description": "Short description",
  "theme": {
    "primary": "#color",
    "secondary": "#color",
    "gradient": "linear-gradient(...)",
    "productsPanel": "#color",
    "registerPanel": "#color",
    "cartPanel": "#color"
  },
  "categories": {
    "set": [],
    "main": [
      {
        "id": "main1",
        "name": "Item Name",
        "price": 100,
        "image": "products/item.png"
      }
    ],
    "dessert": [...],
    "drink": [...]
  }
}
```

## Adding a New Restaurant

1. Create a new folder in `restaurants/` (e.g., `restaurants/italian/`)
2. Create a `menu.json` file with the structure above
3. Create a `products/` subfolder
4. Add product images to the `products/` folder
5. Update `index.html` to include the new restaurant key in `restaurantKeys` array

## Image Paths

All image paths in `menu.json` are relative to the restaurant folder.
Example: `"image": "products/pizza.png"` will load from `restaurants/italian/products/pizza.png`
