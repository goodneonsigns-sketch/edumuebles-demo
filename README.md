# Edumuebles Industrial — edumuebles.do

Exportación estática del sitio, servida por GitHub Pages en
**https://edumuebles.do**. No editar a mano: se regenera desde el código
fuente (repo `edumuebles`) con

    PAGES_DOMAIN=edumuebles.do bash scripts/deploy-pages.sh

Los 48 modelos provienen del Catálogo 2026 de la empresa. Las fotografías de
producto son renders generados a partir de las fotos de ese catálogo, porque
las del PDF impreso son demasiado pequeñas para web; las escenas de aula son
ilustrativas. Todo dato que la empresa no confirmó se retiró del sitio en vez
de publicarse: lo que falta está en `/por-confirmar/`, fuera del índice.

Indexación activa. `app/robots.ts` y `app/sitemap.ts` generan robots.txt y
sitemap.xml; la hoja de trabajo interna `/por-confirmar/` queda excluida.
