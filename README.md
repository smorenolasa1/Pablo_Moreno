# Pablo Moreno Lasa Business Card

Static digital business card for Pablo Moreno Lasa at Evercore, ready to publish with GitHub Pages.

## Files

- `index.html`: page markup and Open Graph metadata.
- `styles.css`: mobile-first visual design, responsive layout, glassmorphism and animations.
- `script.js`: editable profile configuration, 3D/touch movement and Web Share API.
- `assets/pablo-moreno.vcf`: downloadable contact card.
- `assets/evercore-seeklogo-2.svg`: Evercore logo. Add this file before publishing.

## Edit Contact Data

Update the profile data in `script.js`. The visible card, links and share text are controlled from this block:

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

After publishing, replace the Open Graph image URL in `index.html` with the final absolute GitHub Pages URL for the strongest WhatsApp and LinkedIn previews.

## Publish With GitHub Pages

1. Push these files to the repository.
2. In GitHub, open Settings > Pages.
3. Choose the branch and root folder.
4. Save and wait for GitHub Pages to publish the site.
