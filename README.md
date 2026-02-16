# Growth Marketer Toolkit

A collection of 8 browser-based tools built for growth marketers. Single HTML file, no dependencies, no backend required.

## Tools

### 1. JSON to CSV Converter
Convert JSON data to CSV with one-click export. Handles nested objects (flattens with dot notation), arrays of objects, and wrapper objects with embedded arrays.

### 2. Delimiter / Text Converter
Full-featured delimiter tool inspired by [delim.co](https://delim.co). Convert between delimited formats with options for:
- 5 output delimiters (comma, semicolon, pipe, space, newline)
- 4 input split modes
- Quote wrapping (none, double, single)
- Trim whitespace & remove duplicates
- Interval grouping with custom wrap tags
- Custom open/close tags per item

### 3. Word Count & Readability Analyzer
Real-time text analysis with:
- Word count, characters, characters (no spaces), sentences, paragraphs, total lines
- Hemingway-style readability grading using the Automated Readability Index (ARI)
- Color-coded difficulty badges (Easy / Moderate / Difficult)
- No API or LLM required

### 4. URL Encode / Decode
Live bidirectional URL encoding/decoding with support for both `encodeURIComponent` and `encodeURI` modes.

### 5. Mailto Link Generator
Generate mailto: links with:
- To, Subject, CC, BCC fields
- Body with line break support
- Copy as raw link or HTML anchor tag
- Test directly in email client

### 6. URL to QR Code Generator
Generate QR codes from URLs with:
- Single or bulk URL input (one per line)
- Individual PNG download per QR code
- Batch export all QR codes

### 7. Meta Data Extractor
Extract meta tags from any URL including:
- Title, description, canonical URL
- Open Graph tags (title, description, image, type, URL, site name)
- Twitter Card data
- Robots, viewport, charset, favicon
- Bulk import and CSV export
- Uses CORS proxies for cross-origin fetching

### 8. UTM Builder & Parser
**Build mode:** Generate campaign URLs with all 6 standard UTM parameters (source, medium, campaign, term, content, id). UTM params highlighted in output.

**Parse & Validate mode:** Paste any URL to parse and validate UTM tags with:
- Status per parameter (Valid, Warning, Missing, Not set)
- Best-practice checks (lowercase, no spaces, no special characters)
- Overall grade badge
- Summary cards for params found, required present, and warnings

## Usage

Open `index.html` in any modern browser. No build step, no server, no install.

```
open index.html
```

## Tech

- Single HTML file (~1,470 lines)
- Vanilla JS, no frameworks
- Dark/light theme toggle
- JetBrains Mono + Space Mono fonts (Google Fonts)
- QR code generation via [qrcodejs](https://github.com/davidshimjs/qrcodejs)
- Meta extraction uses public CORS proxies (allorigins, corsproxy.io)

## License

MIT
