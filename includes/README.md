# Includes Folder

This folder contains reusable HTML components that are dynamically loaded into all pages.

## Files

- **navbar.html** - Navigation bar component
- **footer.html** - Footer component

## How It Works

The `js/main.js` file automatically loads these components when each page loads:

1. When a page loads, the `loadIncludes()` function runs
2. It fetches `navbar.html` and inserts it into `<div id="navbar-placeholder"></div>`
3. It fetches `footer.html` and inserts it into `<div id="footer-placeholder"></div>`
4. After loading, it sets up navbar functionality (scroll effects, active links)

## Benefits

- **Easy Maintenance**: Update navbar or footer once, changes apply to all pages
- **Consistency**: Ensures all pages have identical navigation and footer
- **Clean Code**: Reduces duplication across HTML files

## Editing

To update the navigation or footer:

1. Edit `navbar.html` or `footer.html`
2. Save the file
3. Refresh any page to see the changes

**Note**: You need to run the site through a web server (not just opening files directly) for the includes to work properly, as the `fetch()` API requires HTTP/HTTPS protocol.
