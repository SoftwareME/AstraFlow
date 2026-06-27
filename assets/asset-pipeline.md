# Asset Pipeline

## Folder Structure

- `assets/references/`: user-provided reference screenshots, brand images, competitor screenshots.
- `assets/generated/`: AI-generated concepts, visual references, hero images, illustrations.
- `assets/cut/`: production-ready exported assets used by the app.
- `assets/icons/`: app icons and symbolic UI assets.

## Image Generation Flow

1. Read product and design context.
2. Generate 2-4 visual directions using `prompts/image-generation.md`.
3. Save outputs to `assets/generated/`.
4. Select one direction.
5. Extract reusable assets only when they are necessary for the product.
6. Export production assets to `assets/cut/`.
7. Use optimized formats:
   - SVG for icons when appropriate.
   - WebP or AVIF for raster images.
   - PNG only when transparency or tooling requires it.

## Cutting Rules

- Do not cut text as images.
- Do not cut buttons, tables, forms, or normal UI controls as images.
- Cut only illustrations, photos, textures, product mockups, or decorative assets that cannot be built cleanly in code.
- Keep UI layout, text, buttons, tables, and forms as real frontend components.

## Asset QA

- Check image dimensions.
- Check compression.
- Check retina quality.
- Check light and dark background compatibility when relevant.
- Check that assets do not cause layout shift.

