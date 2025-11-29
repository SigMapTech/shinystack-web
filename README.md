# ShinyStack Website

Static website for the ShinyStack iOS app - a precious metals collection tracker.

## About ShinyStack

ShinyStack is an iPhone app that helps users track and manage their precious metals collection including gold, silver, platinum, and palladium.

## Website Structure

```
shinystack-web/
├── index.html      # Main landing page
├── privacy.html    # Privacy policy
├── terms.html      # Terms of service
├── .nojekyll       # Disables Jekyll processing
└── README.md       # This file
```

## GitHub Pages Setup

To deploy this website using GitHub Pages:

1. Go to your repository settings on GitHub
2. Navigate to **Settings** > **Pages**
3. Under "Source", select the branch you want to deploy (e.g., `main`)
4. Select the root folder (`/`)
5. Click **Save**

The site will be available at: `https://[username].github.io/shinystack-web/`

### Custom Domain (Optional)

To use a custom domain like `shinystack.app`:

1. Add a `CNAME` file to the repository root containing your domain:
   ```
   shinystack.app
   ```
2. Configure your domain's DNS:
   - For apex domain: Add A records pointing to GitHub's IPs
   - For subdomain: Add a CNAME record pointing to `[username].github.io`

See [GitHub's documentation](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site) for detailed instructions.

## Development

This is a static website with no build process required. Simply edit the HTML files directly.

To preview locally:
- Open `index.html` in a web browser, or
- Use a local server: `python -m http.server 8000`

## License

All rights reserved.
