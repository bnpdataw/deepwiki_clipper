# DeepWiki Clipper Chrome Extension

A Chrome Extension that automatically detects DeepWiki pages and downloads wiki content as formatted markdown files. This extension replicates the functionality of the Python script within a browser environment.

## Features

- **Automatic Detection**: Detects DeepWiki pages (`https://deepwiki.com/*/*`)
- **One-Click Download**: Download content as formatted markdown with a single click
- **Smart Parsing**: Handles RSC (React Server Components) format from DeepWiki API
- **Organized Output**: Creates markdown with table of contents and proper formatting
- **Caching**: Optional content caching to reduce API calls
- **Download History**: Track all your downloads with timestamps
- **Configurable Settings**: Customize filename patterns, auto-download, and more

### Chrome Web Store

The extension will be available on the Chrome Web Store once published.

### Microsoft Edge Store

The extension will be available on the Microsoft Edge Store once published.

## Usage

### Basic Usage

1. **Navigate** to any DeepWiki page (e.g., `https://deepwiki.com/microsoft/vscode`)
2. **Click** the extension icon in the toolbar
3. **Download** - Click "Download as Markdown" button
4. **Save** - The file will be automatically downloaded to your default downloads folder

### Popup Interface

The extension popup shows:
- **Current page status** (DeepWiki detected or not)
- **Download button** (enabled for DeepWiki pages)
- **Progress indicator** during download
- **Settings** and **History** access

### Content Script Features

- **Auto-detection** of DeepWiki pages
- **Download trigger** button on the page itself
- **Real-time status** updates

## Configuration

### Settings Panel

Access via the popup → ⚙️ Settings:

- **Auto-download**: Automatically download when a DeepWiki page loads
- **Download Format**: Choose between Markdown (.md) or HTML (.html)
- **Filename Pattern**: Customize output filename using variables:
  - `{namespace}` - First part of URL path
  - `{page}` - Second part of URL path  
  - `{title}` - Extracted page title
  - `{timestamp}` - Current timestamp
- **Notifications**: Enable/disable download notifications
- **Content Caching**: Cache downloaded content to reduce API calls
- **Cache Expiry**: Set cache expiration time (1-168 hours)
