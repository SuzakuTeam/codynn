<div align="center">
  <img src="https://files.catbox.moe/5idb5o.png" alt="SuzakuTeam Scraper Modules" style="border-radius: 15px; box-shadow: 0 8px 32px rgba(0,0,0,0.2); max-width: 400px; width: 100%; height: auto; margin-bottom: 20px;">
  
  <h1>@SuzakuTeam/scraper-node</h1>
  
  <p><strong>Professional Scraper Modules by SuzakuTeam</strong></p>
  
  <p>
    <a href="https://www.npmjs.com/package/@suzakuteam/scraper-node">
      <img src="https://badge.fury.io/js/@suzakuteam%2Fscraper-node.svg" alt="npm version">
    </a>
    <a href="https://opensource.org/licenses/MIT">
      <img src="https://img.shields.io/badge/License-ISC-yellow.svg" alt="License: ISC">
    </a>
    <a href="https://nodejs.org/">
      <img src="https://img.shields.io/badge/node-%3E%3D%2016.0.0-brightgreen" alt="Node.js Version">
    </a>
  </p>
  
</div>

- [!IMPORTANT]  
- **Sxyz** is back and brings several significant updates to this module. Please use it and apologize for any inconvenience. 🚀

A powerful and efficient web scraping library for modern Node.js applications. Designed with a focus on high performance, reliability, and ease of use.

## Key Features

- **Dual Module Support** - Full compatibility with both ESM and CommonJS
- **High Performance** - Optimized for speed and memory efficiency
- **Type-Safe** - Complete TypeScript support with comprehensive type definitions
- **Modern API** - Promise-based interface with async/await support
- **Lightweight** - Minimal dependencies for maximum performance
- **Comprehensive** - Wide range of scraping capabilities across multiple platforms

## Technology Stack

- **Language**: JavaScript (ES2022+)
- **Module System**: ESM & CommonJS
- **Runtime**: Node.js 16+
- **Architecture**: Modern async/await patterns
- **Type Support**: Full TypeScript definitions

## Installation

```bash
# Using npm
npm install @suzakuteam/scraper-node

# Using yarn
yarn add @suzakuteam/scraper-node

# Using pnpm
pnpm add @suzakuteam/scraper-node
```

## Table of Contents

- [Quick Start](#quick-start)
- [Basic Usage](#basic-usage)
- [Function Parameters](#function-parameters)
- [API Integration](#api-integration)
- [Available Categories](#available-categories)
- [System Requirements](#system-requirements)
- [Documentation](#documentation)
- [Community & Support](#community--support)

## Quick Start

```javascript
// ESM
import { SuzakuTeam } from "@suzakuteam/scraper-node";

// CommonJS
const { SuzakuTeam } = require("@suzakuteam/scraper-node");

(async () => {
  const availableScrapers = await SuzakuTeam.list();
  console.log(availableScrapers);
})();
```

## Basic Usage

### Standard Scraping

```javascript
// ESM
import { SuzakuTeam } from "@suzakuteam/scraper-node";

// CommonJS
const { SuzakuTeam } = require("@suzakuteam/scraper-node");

(async () => {
  // Pattern: const result = await SuzakuTeam.<category>.<scraper>(parameters)
  const aiResponse = await SuzakuTeam.ai.phindChat("What is JavaScript?");
  console.log(aiResponse);

  const instagramData = await SuzakuTeam.stalker.instagram("username");
  console.log(instagramData);
})();
```

### Function Parameters

Check required parameters for any scraper function:

```javascript
// ESM
import { SuzakuTeam } from "@suzakuteam/scraper-node";

// CommonJS
const { SuzakuTeam } = require("@suzakuteam/scraper-node");

/**
 * Get function parameter information
 * @returns {Promise<{lengths: number, params: Array}>}
 */
async function checkParameters() {
  const functionInfo = await SuzakuTeam.getFunctionParams(
    SuzakuTeam.ai.phindChat,
  );
  console.log(functionInfo);
  // Output: { lengths: 1, params: ['query'] }
}

checkParameters();
```

## API Integration

Access external APIs through the integrated API system:

```javascript
// ESM
import { SuzakuTeam } from "@suzakuteam/scraper-node";

// CommonJS
const { SuzakuTeam } = require("@suzakuteam/scraper-node");

(async () => {
  const apiList = await SuzakuTeam.api;
  console.log(apiList);

  // Example API usage:
  // const result = await SuzakuTeam.apis.VelynAPI.velynAI("Hello");
})();
```

## Available Categories

### Tools

Utility functions including NSFW detection, translation, text-to-speech, and various converters.

### AI

AI-powered features with chatbots, code assistants, and intelligent image processing capabilities.

### Downloader

Content download support for major platforms including Facebook, Twitter, Instagram, Spotify, and more.

### Game

Gaming-related scrapers supporting Mobile Legends, Free Fire character information, and game statistics.

### Anime

Comprehensive anime information, quotes, character details, and search functionality.

### Stalker

User information lookup and profile data retrieval for various gaming and social platforms.

### Info

Information services including TV schedules, prayer times, and regional data.

### News

Indonesian news aggregation from multiple categories and reliable sources.

### Search

Advanced search capabilities for NASA data, Spotify content, and specialized databases.

## System Requirements

- Node.js 16.0.0 or higher
- ESM or CommonJS compatible environment
- Modern JavaScript runtime support
- Stable internet connection for web scraping operations

## Documentation

Complete API documentation and detailed usage examples are available in our comprehensive guide. Each scraper function includes parameter specifications, return value descriptions, and practical implementation examples.

## Community & Support

**Official Channels:**

- [WhatsApp Community](https://whatsapp.com/channel/0029VbB0oUvBlHpYbmFDsb3E)
- [Discord Server](https://discord.gg/GxqptZZg)
- [Email Support](mailto:sxyzz.dev@gmail.com)

**Contributing:**
We currently maintain internal development standards. Community contributions will be accepted in future releases with proper guidelines.

## License

This project is licensed under the ISC License. See the [LICENSE](LICENSE) file for complete details.

## Development Team

**Suzaku Team** - Professional development team dedicated to creating high-quality, reliable scraping solutions for the Node.js ecosystem.

---

## Additional Information

This package provides comprehensive dual-module support for both ESM and CommonJS environments, ensuring maximum compatibility across different Node.js project configurations. All functions implement modern asynchronous patterns with promise-based returns, making integration seamless with contemporary JavaScript applications.

**Performance Optimizations:**

- Efficient memory management
- Optimized request handling
- Minimal dependency footprint
- Advanced error handling and recovery
