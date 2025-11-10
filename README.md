# Multi-Restaurant POS System

A touch-friendly point-of-sale system designed for themed restaurants with a guided ordering flow.

## Features

- **Multi-Restaurant Support**: Switch between different themed restaurants
- **Guided Ordering Flow**: Automatic progression through Main → Dessert → Drink
- **Touch-Optimized**: 3D pushable buttons with touch animations
- **Menu Mode**: Digital menu view for customers to browse
- **Custom Sets**: Create custom meal combinations
- **Themed UI**: Each restaurant has its own color scheme and styling

## Live Demo

Visit: [https://nagasakimark.github.io/cashregister2/](https://nagasakimark.github.io/cashregister2/)

## Restaurants

- **New Horizon Restaurant** - Japanese & International Cuisine
- **Kirby Café** - Cute & Delicious Kirby-themed Dishes
- **Pokemon Cafe** - Gotta Eat 'Em All!
- **Rilakkuma Tea House** - Relax and Enjoy Cute Bear-themed Treats

## Usage

1. Select a restaurant from the main screen
2. Follow the guided flow: Select Main → Dessert → Drink
3. Items are automatically added to cart (1 of each)
4. After completing the flow, add more items or checkout
5. Enter payment amount and press ENTER to complete transaction

## Technical Details

- Pure HTML/CSS/JavaScript (no frameworks)
- Optimized for 1366x598 touch screen resolution
- Responsive design with fallbacks for smaller screens
- JSON-based menu configuration for easy updates

## Adding a New Restaurant

1. Create a folder in `restaurants/[restaurant-name]/`
2. Add `menu.json` with restaurant configuration
3. Add `logo.png` (or .jpg)
4. Create `products/` subfolders: `main/`, `dessert/`, `drink/`, `set/`
5. Add product images to appropriate folders
6. Update `restaurantKeys` array in `index.html`

## License

MIT License - Feel free to use and modify for your projects!
