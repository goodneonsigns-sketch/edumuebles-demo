# Edumuebles Industrial, SRL — edumuebles.do

Sitio web **de producción** de Edumuebles Industrial, SRL, fabricante dominicano de
mobiliario escolar, preescolar y de oficina, con taller propio en República
Dominicana: soldadura de estructuras de acero, corte de tableros, pintura
electrostática y tapicería. El sitio está en vivo en **https://edumuebles.do** y
este repositorio contiene su exportación estática, servida por GitHub Pages.

Los 48 modelos publicados son productos reales del Catálogo 2026 de la empresa: se
fabrican en su taller, y las estructuras, medidas y acabados corresponden a lo que
se entrega. Las imágenes de producto se reconstruyeron con edición asistida por IA
a partir de las fotos de ese mismo catálogo, porque las del PDF impreso son
demasiado pequeñas para web; conservan el modelo, la geometría y los colores de
fábrica. Las escenas de aula y biblioteca son composiciones ilustrativas.

Todo dato que la empresa no confirmó se retiró del sitio en vez de publicarse: lo
que falta está en `/por-confirmar/`, fuera del índice.

## Mantenimiento

No editar a mano: se regenera desde el código fuente (repo `edumuebles`) con

    PAGES_DOMAIN=edumuebles.do bash scripts/deploy-pages.sh

Indexación activa. `app/robots.ts` y `app/sitemap.ts` generan robots.txt y
sitemap.xml; la hoja de trabajo interna `/por-confirmar/` queda excluida.
