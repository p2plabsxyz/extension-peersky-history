# extension-peersky-history

Peersky's history tracking web extension (Manifest V3). History is stored locally in IndexedDB.

## Features

- Automatic tracking of all web navigation
- Fast fuzzy search through history
- Protocol-aware (works with peersky://, IPFS, Hypercore, etc.)
- Duplicate filtering in search results
- Individual entry deletion
- Real-time search with debouncing
- Chronological ordering (newest first)

## Installation

1. Load the extension in your Peersky Browser
2. The extension will automatically start tracking your browsing history
3. Access the history viewer through the extension's options page

## Privacy

- All history is stored locally in IndexedDB
- No data is sent to external servers
- You have full control to delete individual entries

## Search

Use fuzzy matching to search - just type words from the URL or title, separated by spaces. For example:
- "peersky docs" will match "Peersky Documentation"
- "github repo" will match any GitHub repository URLs

## Technical Details

- **Manifest Version**: 3
- **Storage**: IndexedDB
- **Permissions**: webNavigation, tabs
- **Background**: Service Worker 
