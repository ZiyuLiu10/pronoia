# Pronoia

**Hakuna Matata 无忧无虑，梦想成真。**

[Open Pronoia / 打开网站](https://ziyuliu10.github.io/pronoia/)

A bilingual scent atlas and perfume recommendation website, with a mother-of-pearl interface and surreal artwork.

- 200 real perfumes across 16 brands, with downloaded product photographs and official note sources.
- Three recommendation levels: birth-chart symbolism and preferences, a longer-term intention, and a particular occasion.
- Up to three recommendations; layering never exceeds two fragrances.
- Private browser-local wardrobe, saved rituals and JSON backups.
- Automatic online lookup for missing perfumes through 12 supported brand catalogues. Confirmed official products and their photographs can be added to a shared public atlas.

Birth details and personal plans remain in the visitor's browser. The independent online catalogue service receives product search queries and confirmation tokens only. Astrology and historical symbolism are creative associations, not proven luck predictions.

## Source

`index.html` is the complete standalone website, including all code, data, artwork and 200 product images. GitHub Pages serves it from the root of `main`; `.nojekyll` disables Jekyll processing.

[`pronoia-source.zip`](pronoia-source.zip) contains modular HTML/CSS/JavaScript, research files, image credits, and recommendation tests. The frontend needs no build step or secret API key. The online service URL is configured in the modular `config.js`.

Code: MIT. Product photography, brand logos and trademarks retain their original rights and are not covered by the code license. Per-image sources are included in `data/image-credits.json` in the source archive.
