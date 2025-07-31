# Web Crawler

A TypeScript-based web crawler that maps internal links on websites. This tool helps analyze website structure and SEO by tracking internal link counts.

## Features

- Crawls websites and maps internal links
- Concurrent crawling with configurable limits
- Reports link counts for each page
- Handles both relative and absolute URLs
- Respects same-domain boundaries

## Prerequisites

- Node.js (version 22.15.0)
- npm (comes with Node.js)

## Installation

1. Clone the repository:

```sh
git clone https://github.com/fatkungfu/crawler-ts.git
cd crawler-ts
```

2. Install dependencies:

```sh
npm install
```

## Usage

Run the crawler with:

```sh
npm start https://example.com
```

Replace `https://example.com` with the website you want to crawl.

The crawler will output a report showing how many times each page was linked to within the site.

## Running Tests

Execute the test suite with:

```sh
npm test
```

## Project Structure

- `src/index.ts` - Entry point
- `src/crawl.ts` - Core crawler implementation
- `src/report.ts` - Report generation functionality
- `src/*.test.ts` - Test files

## Development

The project uses:

- TypeScript for type safety
- JSDOM for HTML parsing
- p-limit for concurrent request management
- Vitest for testing
