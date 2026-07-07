# Pablo Moreno Lasa Business Card

Static digital business card for Pablo Moreno Lasa at Evercore, ready to publish with GitHub Pages.

## Files

- `index.html`: page markup and Open Graph metadata.
- `styles/style-1.css`: current visual direction.
- `styles/style-2.css`: alternate visual direction for client review.
- `scripts/style-switcher.js`: swaps the active stylesheet and stores the preference in `localStorage`.
- `scripts/card.js`: editable profile configuration, 3D/touch movement and Web Share API.
- `assets/pablo-moreno.vcf`: downloadable contact card.
- `assets/evercore-seeklogo-2.svg`: Evercore logo. Add this file before publishing.

## Edit Contact Data

Update the profile data in `scripts/card.js`. The visible card, links and share text are controlled from this block:

```js
const profile = {
  name: "Pablo Moreno Lasa",
  role: "Investment Banking Analyst",
  company: "Evercore",
  tagline: "Utilities, Infrastructure & Transport M&A",
  location: "London, United Kingdom",
  linkedin: "https://www.linkedin.com/in/pablo-moreno-lasa-924890254/",
};
```

`assets/pablo-moreno.vcf` is included as the static contact download.

## Choosing A Final Style

The site is set up so the client can compare two styles without changing the HTML:

- `index.html` stays shared.
- The selector swaps between `styles/style-1.css` and `styles/style-2.css`.
- The selected style is saved in `localStorage`.

When the client chooses one direction, remove the switcher block in `index.html`, remove `scripts/style-switcher.js`, and keep only the chosen stylesheet in the `<head>`.

After publishing, replace the Open Graph image URL in `index.html` with the final absolute GitHub Pages URL for the strongest WhatsApp and LinkedIn previews.

## Publish With GitHub Pages

1. Push these files to the repository.
2. In GitHub, open Settings > Pages.
3. Choose the branch and root folder.
4. Save and wait for GitHub Pages to publish the site.
