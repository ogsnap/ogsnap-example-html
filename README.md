# OgSnap HTML Example

> Simple example of creating dynamic social media preview images with OgSnap

This repository demonstrates how to use [OgSnap](https://ogsnap.com) to generate dynamic Open Graph images for social media. It provides a basic implementation that you can deploy, customize, and integrate into your own projects to create engaging social previews without design skills.

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/yourusername/ogsnap-example-html)
[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/yourusername/ogsnap-example-html)

## What is OgSnap?

OgSnap is a service that renders your webpages as images for social media sharing. Instead of creating static images for each page, you can:

1. Design a dynamic HTML template with customizable parameters
2. Host it anywhere (Vercel, Netlify, etc.)
3. Use OgSnap to capture the rendered page as an image

## How It Works

When you send a URL to OgSnap via `https://ogsnap.com/i/your-webpage.com`, it:
1. Visits your webpage
2. Renders it
3. Takes a screenshot
4. Returns the image

## Getting Started

### Local Development

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/ogsnap-example-html.git
   cd ogsnap-example-html
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

4. Visit http://localhost:1234 to see the example

5. Test with dynamic parameters:
   ```
   http://localhost:1234/?title=This%20is%20title%21&description=This%20is%20description%21%20You%20can%20write%20a%20message%20here.
   ```

### Deployment

1. Deploy this repository to your favorite hosting platform (Netlify, Vercel, etc.)
2. Note your deployed URL (e.g., `https://my-og-example.netlify.app`)

### Using with OgSnap

Once deployed, use your example with OgSnap:

```
https://ogsnap.com/i/my-og-example.netlify.app?title=My%20Awesome%20Page&description=Check%20out%20this%20content!
```

Add this URL to your website's meta tags:

```html
<meta property="og:image" content="https://ogsnap.com/i/my-og-example.netlify.app?title=My%20Awesome%20Page&description=Check%20out%20this%20content!" />
<meta name="twitter:image" content="https://ogsnap.com/i/my-og-example.netlify.app?title=My%20Awesome%20Page&description=Check%20out%20this%20content!" />
```

## Customization

This example accepts query parameters to customize the OG image:

- `title`: The main heading for your OG image
- `description`: The descriptive text below the title

You can extend the example to accept more parameters like:
- Background color
- Logo image
- Author name
- Publication date

## Examples

Here are some example OG images created with this implementation:

1. Basic Example:
   ```
   https://ogsnap.com/i/my-og-example.netlify.app?title=Hello%20World&description=Welcome%20to%20my%20website!
   ```

2. Blog Post:
   ```
   https://ogsnap.com/i/my-og-example.netlify.app?title=10%20Tips%20for%20Better%20Code&description=Improve%20your%20coding%20skills%20with%20these%20expert%20tips
   ```

## Resources

- [OgSnap Documentation](https://ogsnap.com/docs)
- [Open Graph Protocol](https://ogp.me/)

## License

MIT