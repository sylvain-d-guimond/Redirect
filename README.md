# URL Redirect Script

A lightweight, elegant URL redirect utility that you can host on GitHub Pages.

## Features

- 🚀 Simple and fast redirects
- 🎨 Clean, modern UI with loading animation
- ✅ URL validation
- 🔒 Safe handling of invalid URLs
- 📱 Fully responsive
- 📦 Single HTML file (no dependencies)

## Usage

Simply add the `target` query parameter with your destination URL:

```
https://yourusername.github.io/redirect/?target=https://example.com
```

### Examples

```
# Redirect to GitHub
https://yourusername.github.io/redirect/?target=https://github.com

# Redirect to a shortened domain
https://yourusername.github.io/redirect/?target=example.com
```

The script will:
1. Validate the target URL
2. Show a brief loading animation
3. Redirect to your target URL after 1 second

## Setup on GitHub Pages

1. **Fork or clone this repository**

2. **Enable GitHub Pages:**
   - Go to Settings → Pages
   - Select "Deploy from a branch"
   - Choose `main` branch and `/root` directory (or your preferred branch)

3. **Access your redirect:**
   ```
   https://yourusername.github.io/redirect/?target=YOUR_URL_HERE
   ```

## Error Handling

If the target URL is:
- **Missing**: Shows a friendly error message asking for the `?target=` parameter
- **Invalid**: Displays the invalid URL with an error notification

## URL Format

The script accepts URLs with or without `https://`:
- ✅ `?target=https://example.com`
- ✅ `?target=example.com` (automatically adds `https://`)
- ❌ `?target=invalid url with spaces`

## Customization

You can modify the `index.html` file to:
- Change the gradient colors in the CSS
- Adjust the redirect delay (currently 1 second)
- Customize the loading message text
- Add your own branding

## Security Notes

- This script only performs redirects; it doesn't store or log URLs
- All URL validation happens in the browser
- No server-side processing required

## License

MIT - Feel free to use and modify as needed!

## Troubleshooting

**Redirect not working?**
- Ensure the URL starts with `http://` or `https://`, or let the script add it
- Check that the domain is reachable
- Clear your browser cache and try again

**GitHub Pages not working?**
- Make sure GitHub Pages is enabled in your repository settings
- Wait a few minutes for the site to deploy after pushing changes
