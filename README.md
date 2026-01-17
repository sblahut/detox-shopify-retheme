# Detox Nation - Warehouse Theme Fresh

A custom Shopify theme for the Detox Nation website, based on the Warehouse theme framework. This theme provides a modern, responsive shopping experience with custom features and optimizations.

## 🚀 Features

- Responsive design optimized for all devices
- Custom sections and templates for flexible page building
- Enhanced product display with image galleries and quick view
- Advanced collection filtering and sorting
- Newsletter integration
- Adobe Fonts (Mozaic Variable, Marlide Display Variable) - served via Typekit
- Optimized performance with WebP images
- Multi-language support (EN, DE, ES, FR, IT, JA, NB, PT-BR, TR)

## 📁 Project Structure

```
warehouse-theme-fresh/
├── assets/         # Static assets (JS, CSS, images, fonts)
├── config/         # Theme settings and configuration
├── layout/         # Main theme layouts
├── locales/        # Translation files
├── sections/       # Theme sections
├── snippets/       # Reusable liquid snippets
└── templates/      # Page templates
```

## 🛠️ Development

### Prerequisites

- [Node.js](https://nodejs.org/) (Latest LTS version recommended)
- [Shopify CLI](https://shopify.dev/themes/tools/cli)
- [Ruby](https://www.ruby-lang.org/) (Required for Shopify CLI)
- A Shopify Partner account
- Store access with "Manage themes" permission

### Shopify CLI Setup

1. Install Ruby (if not already installed):
   ```bash
   # macOS (using Homebrew)
   brew install ruby

   # Windows (using Chocolatey)
   choco install ruby
   ```

2. Install the Shopify CLI:
   ```bash
   gem install shopify-cli
   ```

3. Authenticate with Shopify:
   ```bash
   shopify login --store your-store.myshopify.com
   ```

### Theme Development

1. Clone this repository:
   ```bash
   git clone https://github.com/your-org/warehouse-theme-fresh.git
   cd warehouse-theme-fresh
   ```

2. Start the development server:
   ```bash
   shopify theme serve
   ```
   This will:
   - Create a development theme in your store
   - Start a local server
   - Watch for changes and hot-reload

3. Common theme commands:
   ```bash
   # Pull theme files from Shopify
   shopify theme pull

   # Push theme files to Shopify
   shopify theme push

   # List all themes in your store
   shopify theme list

   # Get information about the current theme
   shopify theme info
   ```

4. Working with theme variations:
   ```bash
   # Create a new theme variation
   shopify theme push --theme-id=[theme_id] --name="Theme Name"

   # Publish a theme
   shopify theme publish --theme-id=[theme_id]
   ```

### Theme Customization

The theme can be customized through:
- `config/settings_schema.json` - Theme settings structure
- `config/settings_data.json` - Theme settings values
- `assets/theme.css` - Custom CSS styles
- `assets/theme.js` - Custom JavaScript functionality

### Best Practices

1. Always work on a development theme, never the live theme
2. Use version control for all changes
3. Test across multiple devices and browsers
4. Optimize images before uploading
5. Keep the theme up to date with Shopify's latest features

## 🌐 Deployment

1. Test your changes thoroughly in a development theme
2. Push your changes to the theme:
   ```bash
   shopify theme push
   ```
3. Preview in the theme editor
4. When ready, publish through Shopify admin or CLI:
   ```bash
   shopify theme publish --theme-id=[theme_id]
   ```

## 📝 License

This is a private theme developed for Detox Nation by Steven Blahut and Zero Tech, LLC. All rights reserved. 
