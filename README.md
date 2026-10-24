# Pronoia

**Hakuna Matata 无忧无虑，梦想成真。**

[Open Pronoia / 打开网站](https://ziyuliu10.github.io/pronoia/)

A bilingual astrology-based fragrance website with a mother-of-pearl interface and surreal artwork.

- 200 real perfumes across 16 brands, with product photographs and official note sources; verified online additions extend the atlas.
- Three modes: a natal signature scent, a longer-term intention, or a particular occasion.
- 24 selectable feelings plus a custom description, with Chinese/English keyword matching.
- Actual tropical planetary positions, seven traditional planets, chart ruler, whole-sign houses, major aspects and reference-time transits participate in scent ranking.
- Natal temperament and contextual support needs are evaluated separately, including dignity, retrograde motion, solar distance, angular houses, domicile reception and hard versus flowing aspects. Support resources must have an actual natal connection; a missing element is not automatically prescribed.
- Documented material correspondences from Agrippa, with traditional house themes and explicit Pronoia scoring weights. Each recommendation explains the route from chart to published scent notes.
- Up to three recommendations; layering never exceeds two fragrances.
- Browser-local wardrobe, saved rituals and JSON backups; online lookup for missing perfumes through 12 supported brand catalogues.

Provide birth date, time, location and the UTC offset at birth for a full natal calculation. Date-only mode uses the Sun alone. Goal/occasion transits use the entered local reference time and its UTC offset. The method applies a documented astrological interpretation to perfume selection; it does not claim scientifically established changes in luck or event-success probabilities.

Birth details, feelings and personal plans are processed in the visitor’s browser. The online catalogue service receives product lookup and confirmation requests only.

## Source

`index.html` is the complete standalone website, including code, data, artwork and 200 product images. GitHub Pages serves it from `main` / root.

[`pronoia-source.zip`](pronoia-source.zip) contains modular HTML/CSS/JavaScript, research, image credits and 42 tests. No frontend build step or secret API key is needed. Run `node --test tests/*.test.cjs` in the extracted source directory.

Code: MIT. Product photography, brand logos and trademarks retain their original rights and are excluded from the code license. Per-image sources are in `data/image-credits.json`.
