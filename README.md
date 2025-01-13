# A4 in Svelte

A simple template for previewing and printing A4 pages in Svelte. Perfect for creating documents, reports, or any content that needs to match A4 paper size exactly.

## Features

- Live preview of A4 pages in browser
- Accurate representation of printed output
- Customizable page margins
- Simple component-based structure

## Usage

1. Clone this template using one of these methods:

```bash
# Using degit
npx degit NotCoffee418/a4-in-svelte my-a4-project

# Or use GitHub's template feature
# Visit https://github.com/NotCoffee418/a4-in-svelte
# Click "Use this template" > "Create a new repository"

cd my-a4-project
npm install
```

2. Define your content in `routes/+page.svelte`:
```svelte
<script>
  import PagesContainer from '$lib/base/PagesContainer.svelte';
  import Page from '$lib/base/Page.svelte';
</script>

<PagesContainer>
  <Page margin="15mm">
    <h1>Page 1</h1>
    <p>Content for Page 1</p>
  </Page>
  <Page>
    <h1>Page 2</h1>
    <p>Content for Page 2</p>
  </Page>
</PagesContainer>
```

## Components

### Page
Represents a single A4 page.

Props:
- `margin` (optional): Sets the page margins. Default is `20mm`

### PagesContainer
Wrapper component that handles page layout and printing behavior.

## Printing

To print your pages:
1. Use your browser's print function (Ctrl+P / Cmd+P)
2. Set margins to "None" in the print dialog (the component handles margins)
3. Ensure "Background Graphics" is enabled if you're using background colors

## Development

```bash
npm run dev
```

Visit [localhost:5173](http://localhost:5173) to see your pages.

## License

MIT

