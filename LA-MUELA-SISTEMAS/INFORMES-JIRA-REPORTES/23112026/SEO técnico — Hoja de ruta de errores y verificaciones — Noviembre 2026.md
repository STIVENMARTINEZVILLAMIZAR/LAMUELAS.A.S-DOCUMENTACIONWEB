# SEO técnico — Hoja de ruta de errores y verificaciones — Noviembre 2026

**Corte del 23 de noviembre de 2026.** La primera intervención corresponde a la plantilla de producto, a las reglas de rastreo y a la tienda. Las fechas y las áreas que figuran a continuación son propuestas de seguimiento.

## Qué se revisó

Lectura del HTML público de [portada](https://lamuela.com.co/), [tienda](https://lamuela.com.co/tienda/), [Black Days](https://lamuela.com.co/blackdays/) y tres fichas enlazadas desde la portada: [Tijeras Castro Viejo Rectas](https://lamuela.com.co/producto/tijeras-castro-viejo-rectas-cirene/) · [Portagrapas](https://lamuela.com.co/producto/portagrapas-cirene/) · [Forcep #150](https://lamuela.com.co/producto/forcep-150-cirene/). Se inspeccionaron títulos, metadescripciones, H1, canonical, directivas robots, imágenes y marcado JSON-LD. También se consultaron [robots.txt](https://lamuela.com.co/robots.txt) y el [índice de sitemaps](https://lamuela.com.co/sitemaps.xml). Las seis páginas respondieron HTTP 200, con canonical propia e index, follow. /sitemap\_index.xml condujo a /sitemaps.xml. La muestra cubre tres fichas de una misma marca y no determina el estado de todo el catálogo ni la indexación efectiva.

## Plan de corrección

### Datos de producto y valoraciones

**Alta · 24–25 nov**

Las tres fichas CIRENE declaran brand.name = Essentia. Repiten 4,5/5, 23 valoraciones y una reseña idéntica del mismo autor y fecha. La procedencia de estas valoraciones requiere comprobación.

**Acción y área sugerida.** Sistemas y Catálogo. Localizar la plantilla JSON-LD, alimentar marca y valoraciones desde datos comprobados por SKU y retirar los valores fijos sin soporte.

**Prueba de cierre.** Comparar el marcado con la ficha y reseñas de cada SKU. Probar las tres URLs y una ficha adicional de otra marca. Conservar el resultado de la prueba de resultados enriquecidos.

### Rastreo de recursos y paginación

**Alta · 24–25 nov**

La respuesta de robots.txt incluye reglas para /wp-content/themes/, /wp-includes/, /wp-content/plugins/ y /\*page/\*. Dos lecturas devolvieron envoltorio HTML aunque la cabecera indica text/plain. El efecto en Googlebot está por verificar.

**Acción y área sugerida.** Sistemas y SEO. Contrastar la respuesta de origen y la recibida por Search Console. Revisar una categoría paginada y recursos CSS/JS necesarios para renderizarla.

**Prueba de cierre.** Guardar la respuesta en texto plano y la inspección en vivo de categoría, página 2 y producto. Verificar carga de recursos y mantener las exclusiones intencionales.

### Metadescripción de la tienda

**Alta · 24 nov**

En /tienda/ el campo description contiene literalmente %%post\_description%%. El título termina en un guion suelto.

**Acción y área sugerida.** Gestión Web. Corregir la plantilla del archivo de tienda. Usar una descripción propia, por ejemplo «Explore equipos, instrumental e insumos odontológicos en La Muela. Consulte referencias, disponibilidad y opciones de compra en Colombia».

**Prueba de cierre.** Comprobar en el HTML público la descripción aprobada, un título sin guion residual y ausencia de variables sin resolver. Revisar también dos categorías.

### Jerarquía de Black Days

**Media · 25–27 nov**

La landing entrega tres H1: «BlackDays», «¡Black Friday La muela!» y «👇Tus marcas favoritas con precios de Black Friday👇». Compiten como encabezado principal.

**Acción y área sugerida.** Gestión Web. Elegir un H1 descriptivo de la campaña y pasar los títulos de sección a H2 conservando el diseño.

**Prueba de cierre.** Un H1 principal en el HTML. Comprobar jerarquía y apariencia en móvil y escritorio.

### Alternativas de imágenes y experiencia móvil

**Media · 25–27 nov**

Portada: 18 de 242 etiquetas img sin texto alternativo útil en el atributo. Black Days: 4 de 74. El conteo incluye elementos que pueden ser decorativos.

**Acción y área sugerida.** Web y Publicidad. Clasificar banners, logos y controles. Describir imágenes informativas y comprobar el nombre accesible de enlaces que solo contienen imágenes. Mantener alt vacío en decoración.

**Prueba de cierre.** Registrar los casos revisados. Probar a 360, 390 y 768 px que header, cierre del pop-up, carrusel, precios y botón quedan visibles y sin desplazamiento horizontal.

### Conciliación de Semrush y rendimiento real

**Seguimiento · 27 nov–4 dic**

La captura informa 14 errores y 3.288 advertencias sin desglose por URL. Core Web Vitals figura como «No implementado».

**Acción y área sugerida.** SEO. Exportar incidencias y URLs, agrupar por plantilla, asignar responsable y repetir el rastreo con el mismo alcance. Medir portada, campaña y ficha con PageSpeed Insights móvil y consultar datos de campo disponibles.

**Prueba de cierre.** Comparativa fechada por incidencia y URL. Registrar LCP, INP y CLS de campo cuando existan, y separar pruebas de laboratorio. Documentar pendientes con fecha y responsable.

## Referencia para el próximo corte

Captura de Semrush aportada por Gestión Web: salud del sitio 76 %, salud de búsqueda con IA 82 %, rastreabilidad 96 %, HTTPS 98 %, rendimiento del sitio 85 %, enlazado interno 89 % y marcados 95 %. La mejora del 6 % desde el inicio de la gestión es reportada por el responsable. Para calcular la variación, recuperar la auditoría inicial fechada y comparar el mismo indicador y alcance. El porcentaje de rendimiento de Semrush y las métricas de experiencia de usuarios se registran por separado.

Registrar por incidencia la URL, la fecha, el responsable confirmado, evidencia antes y después y el resultado de la prueba. Vincular la exportación de Semrush al mismo registro para evitar contabilizar dos veces una misma incidencia.
