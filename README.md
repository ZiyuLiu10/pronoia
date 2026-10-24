# Pronoia

**Hakuna Matata 无忧无虑，梦想成真。**

[Open Pronoia / 打开网站](https://ziyuliu10.github.io/pronoia/)

A bilingual astrology-based fragrance website with a mother-of-pearl interface and surreal artwork.

- 200 real perfumes across 16 brands, with product photographs and official note sources; verified online additions extend the atlas.
- Three modes: a natal signature scent, a longer-term intention, or a particular occasion.
- Male, female and unisex scent-direction choices, with bilingual labels and brand-source positioning. This lightly adjusts ranking while preserving chart calculations and individual preferences.
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

[`pronoia-source.zip`](pronoia-source.zip) contains modular HTML/CSS/JavaScript, research, image credits and 50 tests. No frontend build step or secret API key is needed. Run `node --test tests/*.test.cjs` in the extracted source directory.

Code: MIT. Product photography, brand logos and trademarks retain their original rights and are excluded from the code license. Per-image sources are in `data/image-credits.json`.

## Birth city search

Search cities worldwide in Chinese or English, distinguish places by region and country, and open the chosen city on Google Maps. Coordinates are handled internally; there are no coordinate input fields. In-page search uses Open-Meteo / GeoNames, not Google Places. Only the city query is sent to the search service. Birth date and time stay in the browser. Check the historical UTC offset and daylight saving time for the birth date. Editing the city text invalidates the previous selection. A full chart requires choosing a result.

The free geocoding endpoint is for non-commercial use. Before commercial use, arrange the provider's commercial plan or substitute a licensed service. Google Maps links require no API key.

## Scent introductions

The atlas now includes 201 individually written bilingual scent sketches: one for each of the 200 base fragrances and the verified Dear Polly addition. Each Chinese paragraph is about 57–84 characters, paired with an English paragraph of about 27–36 words. The original editorial text draws on published brand notes and available brand descriptions; product-page references appear in each detail view. Cards display the complete paragraph. Different concentrations have separate copy.

The source text and references are in `data/stories.json`, with the browser copy in `data/stories.js`. `node scripts/sync-data.cjs` regenerates browser data files. Newly imported products without a curated sketch receive a short description based only on their available notes. These descriptions do not affect recommendation scoring.
