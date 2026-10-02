# YT Ad Skipper - Remote Rules Configuration

This repository hosts the `rules.json` file used by the **YT Ad Skipper** browser extension. 

By hosting this file externally on GitHub, the extension can dynamically fetch the latest DOM selectors on startup. This allows you to update the ad-blocking logic to counter YouTube's frequent layout changes without needing to republish or reinstall the extension.

## JSON Structure

The `rules.json` file must follow this exact structure:

```json
{
  "version": 1.0,
  "skipSelectors": [
    ".ytp-skip-ad-button",
    ".ytp-ad-skip-button"
  ],
  "adPlayerClasses": [
    ".ad-showing",
    ".ad-interrupting"
  ]
}
