# Convenciones del repositorio

- [Índice general](../../INDICE.md)
- [Inicio](../../README.md)
- [Guía de evidencias](../01-GUIAS/GUIA-ORGANIZACION-DE-EVIDENCIAS.md)
- [Plantillas](../03-PLANTILLAS-MARKDOWN/)

## Idioma

Nombres de carpetas y documentos en **español**, salvo extensiones y términos técnicos de uso universal (`WordPress`, `SKU`, `SEO`, `CSV`, `XML`, `PDF`, `SQL`).

## Nombres de archivos nuevos

Formato:

```text
AAAA-MM-DD_TIPO_DESCRIPCION.ext
```

Ejemplos:

- `2026-11-04_AUDITORIA-WORDPRESS.md`
- `2026-11-04_ERROR-AUTOLOAD.png`
- `2026-11-04_REVISION-WOOCOMMERCE.xlsx`
- `2026-11-04_REPORTE-SEO.pdf`

Reglas:

- Usar guiones para separar palabras.
- Evitar espacios y caracteres especiales (`á é í ó ú ñ ? ! / \ : *`).
- El `TIPO` en mayúsculas y breve: `AUDITORIA`, `INCIDENCIA`, `BITACORA`, `INFORME`, `PROCEDIMIENTO`.
- La descripción en mayúsculas, concreta y sin ambigüedades (`documento1`, `final2`, `varios`, `nuevo`).

## Carpetas

- Prefijo numérico de dos dígitos para el orden (`01-`, `02-`, … `99-`).
- Nombres descriptivos en mayúsculas y guiones.
- Para una herramienta o sistema nuevo, crear una subcarpeta en `04-SOFTWARE-Y-SISTEMAS/` o en la sección que corresponda, con el siguiente número disponible.

## Markdown

- Copiar una plantilla; no editar el archivo original de `03-PLANTILLAS-MARKDOWN/`.
- Enlazar solo archivos que existan.
- Usar rutas relativas.
- Un hecho, un documento; las evidencias van aparte.

## Bitácora

- Un archivo por día de trabajo real, no por cada fecha del calendario.
- Ruta: `01-BITACORA-DE-ACTIVIDADES/AAAA/MM-MES/AAAA-MM-DD_BITACORA.md`.

## Proyectos e incidencias

- Proyecto: carpeta con nombre descriptivo dentro del estado actual (`01-EN-PLANIFICACION`, `02-EN-EJECUCION`, etc.).
- Incidencia: un Markdown por caso, movido de carpeta según el estado (abierta, análisis, escalada, corrección, validación, cerrada).

## Archivo histórico

Mover a `99-ARCHIVO-HISTORICO/` solo documentación que ya no esté activa y deba conservarse.
