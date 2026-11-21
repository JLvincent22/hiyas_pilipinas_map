# HIYAS PILIPINAS — Heritage Explorer

A responsive, static HTML/CSS/JavaScript website featuring 18 Philippine regions and one featured heritage destination per region. The destination information is based on the supplied `Info each region (1).pdf`.

## Preview locally
Open `index.html` in a browser. Internet access is needed for the Google Maps embeds.

## Google Maps
Each region loads a Google Maps embed using its featured destination address. To use your own exact Google Maps embed for any destination, add a `mapEmbed` property to that destination object in the `REGIONS` array, for example:

```js
mapEmbed: 'https://www.google.com/maps/embed?pb=YOUR_EMBED_CODE'
```

The website will use that exact embed URL when present and will otherwise fall back to the address-based Google Maps embed.

## Deploy to Vercel
1. Create a GitHub repository.
2. Upload `index.html` (and this README).
3. Import the repository in Vercel.
4. Framework Preset: **Other**. Build Command: leave blank. Output Directory: `.`.
5. Deploy.

No build step or API key is required for this basic Google Maps search embed. For a production Maps Embed API integration, you can replace the map URL with your Google Maps Embed API URL and API key.

## Customize
- Search regions in the header.
- Select a region to change the pinned Google Maps destination and details.
- Update the `REGIONS` array in the script to edit content and coordinates.
