# Goose Redirect

A simple GitHub Pages site that redirects to Goose protocol URLs.

## How to Use

This redirector supports three methods:

1. Path-based: `https://michaelneale.github.io/goose-redirect/your/path`
   - Redirects to `goose:///your/path`

2. Query parameter: `https://michaelneale.github.io/goose-redirect/?target=your/path`
   - Redirects to `goose:///your/path`

3. Extension format: `https://michaelneale.github.io/goose-redirect/?cmd=uvx&arg=extension-name&id=id&name=Name&description=Description`
   - Redirects to `goose://extension?cmd=uvx&arg=extension-name&id=id&name=Name&description=Description`

## Example

This URL:
```
https://michaelneale.github.io/goose-redirect/?cmd=uvx&arg=mcp-server-git&id=git&name=Git&description=Git%20version%20control%20system%20integration
```

Will redirect to:
```
goose://extension?cmd=uvx&arg=mcp-server-git&id=git&name=Git&description=Git%20version%20control%20system%20integration
```

## Why?

This allows creating links that work on platforms that don't support custom protocol handlers directly but do allow HTTP links.