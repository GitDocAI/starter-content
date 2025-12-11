# GitDocAI Starter Content

This is the official starter content template for [GitDocAI](https://gitdoc.ai). It provides a complete example of how to structure and write documentation using GitDocAI's MDX-based format.

## What is this?

This repository serves as a reference implementation showing:

- How to structure your documentation files
- How to configure `gitdocai.config.json`
- How to use all available MDX components
- Best practices for organizing content

## Project Structure

```
starter-content/
├── gitdocai.config.json      # Main configuration file
├── assets/                   # Logo and favicon assets
│   ├── dark.svg              # Dark mode logo
│   ├── light.svg             # Light mode logo
│   └── favicon.svg           # Site favicon
└── documentation/            # Documentation pages
    ├── getting_started/
    │   ├── introduction.mdx
    │   ├── installation.mdx
    │   ├── quick_start.mdx
    │   └── all_components.mdx
    └── core_features/
        ├── cloud_services.mdx
        ├── security_configuration.mdx
        └── monitoring_analytics.mdx
```

## Configuration

The `gitdocai.config.json` file controls your documentation site:

```json
{
  "name": "Your Documentation",
  "description": "Your site description",
  "theme": "crystal",
  "colors": {
    "dark": "#8b5cf6",
    "light": "#3b82f6"
  },
  "logo": {
    "light": "/assets/light.svg",
    "dark": "/assets/dark.svg"
  },
  "navigation": {
    "tabs": [...]
  }
}
```

## Available Components

GitDocAI supports 31 MDX components organized in categories:

### Text & Formatting
- Headings (H1-H3)
- Bold, Italic, Strikethrough, Underline
- Blockquotes
- Inline code

### Lists
- Bullet lists
- Numbered lists
- Task lists (checkboxes)

### Code
- Fenced code blocks with syntax highlighting
- `<CodeGroup>` for multi-language examples

### Info Blocks
```mdx
> [!TIP]
> Helpful tips for users

> [!INFO]
> General information

> [!NOTE]
> Important notes

> [!WARNING]
> Warning messages

> [!DANGER]
> Critical warnings
```

Or use component syntax:
```mdx
<Tip>Helpful tip</Tip>
<Info>Information</Info>
<Warning>Warning message</Warning>
<Danger>Critical warning</Danger>
```

### Layout Components
- `<Card>` - Clickable cards with icons
- `<Columns>` - Multi-column layouts
- `<RightPanel>` - Side panel content
- `<Tabs>` - Tabbed content
- `<Accordion>` - Collapsible sections

### Technical Components
- `<Endpoint>` - API endpoint badges
- `<Label>` - Status labels/badges
- `<Table>` - Advanced tables with sorting/filtering
- `<CheckList>` - Do's and don'ts lists

## Getting Started

1. **Clone this repository** as a starting point
2. **Modify** `gitdocai.config.json` with your project details
3. **Replace** the content in `/documentation` with your own
4. **Update** the assets in `/assets` with your branding
5. **Connect** your repository to GitDocAI

## Example Usage

### Cards
```mdx
<Card title="Getting Started" icon="pi pi-rocket" href="/docs/intro">
  Learn the basics and get started quickly.
</Card>
```

### Code Groups
```mdx
<CodeGroup>
  <Code lang="javascript">
    console.log('Hello');
  </Code>
  <Code lang="python">
    print('Hello')
  </Code>
</CodeGroup>
```

### Tabs
```mdx
<Tabs>
  <Tab title="npm">
    npm install package-name
  </Tab>
  <Tab title="yarn">
    yarn add package-name
  </Tab>
</Tabs>
```

### API Endpoints
```mdx
<Endpoint method="GET" path="/api/users" />
<Endpoint method="POST" path="/api/users" />
```

## Learn More

- Visit [gitdoc.ai](https://gitdoc.ai) to get started
- Check `/documentation/getting_started/all_components.mdx` for a complete component showcase
- Explore the example pages to see components in action

## License

This starter content is provided as a template for GitDocAI users.
