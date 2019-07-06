# HTML-To-PHP-Helpers
Docs and tools for converting static HTML pages to production PHP pages

# CSS

## Asset loading and cache busting for CSS files using `asset()` helper
regex: <link(.+)href="(.+)" +(.*?)>
replace with: <link $1 href="<\?php asset($2); \?\> "$3>
