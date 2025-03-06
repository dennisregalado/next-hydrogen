# Next Hydrogen

Next Hydrogen is a fork of [Shopify's Hydrogen framework](https://github.com/Shopify/hydrogen) that provides custom modifications and enhancements for building Shopify storefronts.

## Overview

This package provides a modified version of Shopify's Hydrogen framework, maintaining compatibility with the core features while introducing custom improvements and modifications.

## Installation

```bash
npm install next-hydrogen
```

## Key Features

- All core Hydrogen features
- Compatible with Remix v2
- Built-in Shopify Storefront API integration
- Full TypeScript support
- Vite plugin support

## Usage

```tsx
import {
  createStorefrontClient,
  ShopifyProvider,
} from 'next-hydrogen';

// Initialize the Storefront client
const client = createStorefrontClient({
  storeDomain: 'your-store.myshopify.com',
  publicStorefrontToken: 'your-storefront-api-token',
});

// Wrap your app with the ShopifyProvider
function App() {
  return (
    <ShopifyProvider client={client}>
      {/* Your app components */}
    </ShopifyProvider>
  );
}
```

## Dependencies

- React ^18.2.0
- Remix ^2.10.0
- Vite ^5.1.0 (optional)

## Version

Current version: 2025.1.2

## License

MIT License - See LICENSE file for details

## Acknowledgments

This project is a fork of [Shopify's Hydrogen](https://github.com/Shopify/hydrogen), which is created and maintained by Shopify Inc. The original project is licensed under the MIT License.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Documentation

For detailed documentation about the original Hydrogen framework, please visit [Hydrogen's documentation](https://shopify.dev/custom-storefronts/hydrogen). Note that some features in this fork might differ from the original documentation.

## Support

For issues and feature requests specific to next-hydrogen, please use the [GitHub issues page](https://github.com/dennisregalado/next-hydrogen/issues).
