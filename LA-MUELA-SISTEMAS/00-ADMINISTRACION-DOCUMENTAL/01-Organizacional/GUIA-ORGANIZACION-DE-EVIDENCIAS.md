# Guía de organización de evidencias

- [Índice general](../../INDICE.md)
- [Inicio](../../README.md)
- [Convenciones](../02-CONVENCIONES/CONVENCIONES.md)
- [Evidencias y adjuntos](../../08-EVIDENCIAS-Y-ADJUNTOS/README.md)

## Principio

El documento Markdown describe el hecho. El adjunto (imagen, PDF, Excel u otro) se guarda **una sola vez** en `08-EVIDENCIAS-Y-ADJUNTOS/` y se enlaza con una ruta relativa.

No duplique el mismo archivo en varias carpetas.

## Clasificación por tipo

| Extensión o tipo | Carpeta |
| --- | --- |
| `.png`, `.jpg`, `.webp` de pantalla | `08-EVIDENCIAS-Y-ADJUNTOS/01-CAPTURAS-PANTALLA/` |
| Fotografías de equipos o instalaciones | `08-EVIDENCIAS-Y-ADJUNTOS/02-FOTOGRAFIAS/` |
| Otras imágenes (logos, recortes, mocks) | `08-EVIDENCIAS-Y-ADJUNTOS/03-IMAGENES/` |
| `.pdf` | `08-EVIDENCIAS-Y-ADJUNTOS/04-DOCUMENTOS-PDF/` |
| `.doc`, `.docx` | `08-EVIDENCIAS-Y-ADJUNTOS/05-DOCUMENTOS-WORD/` |
| `.xls`, `.xlsx` | `08-EVIDENCIAS-Y-ADJUNTOS/06-ARCHIVOS-EXCEL/` |
| `.csv` | `08-EVIDENCIAS-Y-ADJUNTOS/07-ARCHIVOS-CSV/` |
| `.xml` | `08-EVIDENCIAS-Y-ADJUNTOS/08-ARCHIVOS-XML/` |
| Diagramas (`.drawio`, `.svg`, exports) | `08-EVIDENCIAS-Y-ADJUNTOS/09-DIAGRAMAS/` |
| Exportaciones de herramientas | `08-EVIDENCIAS-Y-ADJUNTOS/10-EXPORTACIONES/` |
| Comparativos antes / después | `08-EVIDENCIAS-Y-ADJUNTOS/11-ANTES-Y-DESPUES/` |
| Cualquier otro adjunto | `08-EVIDENCIAS-Y-ADJUNTOS/12-OTROS-ARCHIVOS/` |

## Subcarpetas por actividad

Cuando una actividad genera **varios** archivos, cree una subcarpeta identificada por fecha y actividad **solo en ese momento**:

```text
08-EVIDENCIAS-Y-ADJUNTOS/
└── 01-CAPTURAS-PANTALLA/
    └── 2026/
        └── 2026-11-04_AUDITORIA-WORDPRESS/
            ├── 01-SALUD-DEL-SITIO.png
            ├── 02-PLUGINS-ACTIVOS.png
            └── 03-ERROR-INSTAGRAM.png
```

No cree subcarpetas de actividades futuras.

## Enlaces relativos desde un documento

Ejemplo desde `02-WORDPRESS-Y-PAGINA-WEB/01-AUDITORIAS/SEO/`:

```markdown
![Salud del sitio](../../../08-EVIDENCIAS-Y-ADJUNTOS/01-CAPTURAS-PANTALLA/2026/2026-11-04_AUDITORIA-WORDPRESS/01-SALUD-DEL-SITIO.png)
```

Ejemplo de documento PDF:

```markdown
[Reporte SEO](../../08-EVIDENCIAS-Y-ADJUNTOS/04-DOCUMENTOS-PDF/2026-11-04_REPORTE-SEO.pdf)
```

## Seguridad

No almacene contraseñas, tokens, claves API ni datos personales sensibles en evidencias ni en Markdown. Si una captura las muestra, enmascárelas antes de guardarla.
