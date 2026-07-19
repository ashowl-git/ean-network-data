# EAN Network Data Visualization

Interactive network visualization of EAN Technology contract data using D3.js force-directed layout with Obsidian-style design.

## Live Demo

**https://ashowl-git.github.io/ean-network-data/**

## Features

- **Interactive Network Graph**: D3.js-based force-directed layout
- **503 Contract Records**: Data from 2003-2025
- **Real-time Search & Filtering**: Search by contractor, project name, or service type
- **Obsidian-style Theme**: Dark theme with smooth animations
- **Responsive Design**: Optimized for mobile, tablet, and desktop

## Data Structure

- **Services**: 24 types of certification and evaluation services
- **Contractors**: 248 partner organizations
- **Regions**: 16 geographical areas
- **Time Range**: 2003-2025

## Technology Stack

- **HTML5** + **CSS3** (Grid, Flexbox)
- **JavaScript (ES6+)**: Vanilla JS, no framework dependencies
- **D3.js v7**: Force-directed graph layout
- **JSON Data**: Structured contract information

## Usage

### Navigation
- **Zoom**: Mouse wheel or zoom buttons (+/-)
- **Pan**: Click and drag the graph
- **Node Focus**: Click on any node to zoom in
- **Highlight**: Hover over nodes to see connections

### Search & Filter
- **Text Search**: Search contractors, projects, or services
- **Year Filter**: Filter by specific year or view all
- **Node Type Filter**: Filter by contractor, project, or service type

## Performance

- **Load Time**: ~1-2 seconds (JSON data loading)
- **Rendering**: ~100-300ms (503 nodes)
- **Interaction**: <50ms response time
- **Memory**: ~10-20MB browser usage

## Browser Support

- Chrome/Edge (Recommended)
- Firefox
- Safari
- Modern browsers with ES6+ support

## Project Structure

```
ean-network-data/
├── index.html          # Main visualization page
├── styles.css          # Obsidian-style CSS
├── data.json           # Contract data (503 records)
└── README.md           # This file
```

## License

© 2025 EAN Technology. All rights reserved.

## Contact

For inquiries about the data or visualization, please contact EAN Technology.

---

**Powered by D3.js** | **Designed with Obsidian-inspired aesthetics**
