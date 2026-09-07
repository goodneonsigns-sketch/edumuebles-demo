# Media provenance

Every raster under `public/media/` is **generated demonstration imagery** derived
from Edumuebles' own *Catálogo 2026 · Mobiliarios escolares* (PDF supplied by the
client on 2026-09-06), except the `catalogo/` folder, which holds the catalogue's
own page images kept for their published measurements.

## Products (`products/<slug>/`)

- `base.webp` — a clean studio packshot regenerated from the catalogue photo of
  that model with Higgsfield `nano_banana_2` (2k), the catalogue view passed as
  `image_references` and a prompt that fixes the design, proportions, frame,
  fixings and viewpoint. Wood/laminate surfaces rendered in natural birch.
- `naranja / amarillo / verde / rojo / azul.webp` — the same packshot recoloured
  by referencing the base job id and changing only the laminate colour. The
  plastic *silla inicial* uses `naranja / verde / rojo / azul / blanco`.
- extra views (`lateral`, `frontal`, `superior`, `config-1…`, `agrupadas`,
  `con-sillas`, `estructura`, `posterior`, `perspectiva`, `vista-2`,
  `tres-mesas`, `conjunto`, `alineadas`) — regenerated from the matching
  catalogue view.
- `_comparaciones/*.webp` — the catalogue's "Diferencia: altura y anchura"
  lineups regenerated from the base packshots plus the catalogue comparison photo.

## Scenes (`scenes/`)

- `aula-butacas`, `aula-inicial`, `biblioteca` — interiors furnished with the
  regenerated models (base job ids as references). `taller` — the workshop
  documentary scene from the first build.

## Catalogue pages (`catalogo/`)

Native page images from the PDF, enlarged 4x (Lanczos) by the client's
extraction, converted to webp. Not generated; they carry the printed cotas.

Prompts and provenance are embedded per file as `.webp.json` sidecars by
`scripts/embed-catalog-prompts.py`; the generation plan lives in
`media-src/catalog/plan-*.json` and `jobs.json` (gitignored source folder).
