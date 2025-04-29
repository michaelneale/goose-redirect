# Goose Redirect

A simple GitHub Pages site that redirects to Goose protocol URLs.

## How to Use

This redirector supports two methods:

1. Path-based: `https://michaelneale.github.io/goose-redirect/your/path`
2. Query parameter: `https://michaelneale.github.io/goose-redirect/?target=your/path`

Both will redirect to `goose:///your/path`

## Why?

This allows creating links that work on platforms that don't support custom protocol handlers directly but do allow HTTP links.