# @nattui/tailwind-colors

Centralized CSS and Tailwind color definitions for consistent styling across projects.

## Installation

```bash
npm install @nattui/tailwind-colors
# or
pnpm add @nattui/tailwind-colors
# or
bun add @nattui/tailwind-colors
```

## Usage

### Import in your CSS

```css
@import "@nattui/tailwind-colors";
```

Or import directly in your main CSS file:

```css
@import "@nattui/tailwind-colors/src/index.css";
```

### Using CSS Variables

All colors are available as CSS custom properties:

```css
.my-element {
  background-color: var(--color-gray-1);
  color: var(--color-primary-9);
  border-color: var(--color-gray-a3);
}
```

### Using with Tailwind CSS

The package includes Tailwind CSS theme definitions. After importing, you can use colors in your Tailwind classes:

```html
<div class="bg-gray-1 text-primary-9 border-gray-a3">
  Content
</div>
```

### Theme Classes

Apply theme classes to switch between color variants:

```html
<!-- Gray theme -->
<div class="color-gray-gray">
  <!-- Uses gray color palette -->
</div>

<!-- Primary theme (gold) -->
<div class="color-primary-gold">
  <!-- Uses gold color palette -->
</div>
```

## Color System

### Color Scales

Each color palette includes:

- **Base colors**: `--color-{name}-1` through `--color-{name}-12`
- **Alpha variants**: `--color-{name}-a1` through `--color-{name}-a12`
- **Light variants**: `--color-{name}-light-1` through `--color-{name}-light-12`
- **Dark variants**: `--color-{name}-dark-1` through `--color-{name}-dark-12`

### Available Color Palettes

- **Gray**: Neutral grayscale palette with light and dark variants
- **Primary**: Brand color palette with multiple color options (e.g., gold) and light/dark variants
- **Black & White**: Base colors with alpha variants
