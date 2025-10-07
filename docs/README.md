# My Tech Blog

A personal blog documenting my journey through algorithms and data structures.

## Project Structure

```
myblog/
├── config/                    # Configuration files
│   ├── _config.yml           # Main Hexo configuration
│   ├── _config.next.yml      # NexT theme configuration
│   └── _config.landscape.yml # Landscape theme configuration
├── docs/                     # Documentation
│   └── README.md            # This file
├── scripts/                  # Build and utility scripts
│   ├── build.bat            # Build script
│   └── deploy.bat           # Deploy script
├── source/                   # Source content
│   ├── _data/               # Theme customization files
│   ├── _posts/              # Blog posts (markdown files)
│   ├── pages/               # Static pages
│   │   ├── about/           # About page
│   │   ├── categories/      # Categories page
│   │   └── tags/            # Tags page
│   └── assets/              # All assets
│       ├── images/          # Images and media files
│       ├── css/             # Custom CSS files
│       └── js/              # Custom JavaScript files
└── public/                  # Generated static site (auto-generated)
```

## Content

This blog contains algorithm and data structure tutorials organized by topics:

- **Algorithm Complexity Analysis** - Time and space complexity
- **Data Structures** - Linked Lists, Arrays, Trees, Stacks, Queues, Heaps, Graphs
- **Algorithms** - String processing, Combinations, Dynamic Programming

## Development

### Prerequisites
- Node.js
- npm

### Setup
1. Install dependencies: `npm install`
2. Generate site: `npm run build`
3. Run server: `npm run server`

### Commands
- `npm run build` - Generate static files
- `npm run clean` - Clean generated files
- `npm run server` - Start local server
- `npm run deploy` - Deploy to GitHub Pages

## Deployment

The blog is automatically deployed to GitHub Pages at: https://danieldzy7.github.io/myblog/

## License

This project is for educational purposes.
