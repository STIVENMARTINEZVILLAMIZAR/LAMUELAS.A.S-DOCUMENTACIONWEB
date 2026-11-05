# Repositorio documental — Sistemas LA MUELA S.A.S.

Repositorio de **documentación técnica** del Analista de Sistemas de LA MUELA S.A.S. Sirve para clasificar, consultar y conservar evidencias de las actividades del área, empezando por WordPress y extendiéndose a toda la infraestructura y el software de la empresa.

Este directorio **no es una aplicación**. No contiene frontend, backend, dashboards ni código ejecutable.

## Navegación

- [Índice general](INDICE.md)
- [Guías](00-ADMINISTRACION-DOCUMENTAL/01-GUIAS/GUIA-ORGANIZACION-DE-EVIDENCIAS.md)
- [Convenciones](00-ADMINISTRACION-DOCUMENTAL/02-CONVENCIONES/CONVENCIONES.md)
- [Plantillas Markdown](00-ADMINISTRACION-DOCUMENTAL/03-PLANTILLAS-MARKDOWN/)
- [Historial de cambios de la estructura](00-ADMINISTRACION-DOCUMENTAL/05-HISTORIAL-DE-CAMBIOS/HISTORIAL.md)

## Cómo usar este repositorio

1. Copiar la plantilla que corresponda en `00-ADMINISTRACION-DOCUMENTAL/03-PLANTILLAS-MARKDOWN/`.
2. Guardar el documento en la sección temática adecuada, con el formato de nombre `AAAA-MM-DD_TIPO_DESCRIPCION`.
3. Depositar adjuntos en `08-EVIDENCIAS-Y-ADJUNTOS/` según el tipo de archivo.
4. Enlazar evidencias desde el Markdown con **rutas relativas**.
5. Registrar la actividad en la bitácora del mes correspondiente.

## Dónde guardar cada tipo de archivo

| Tipo | Ubicación |
| --- | --- |
| Documentos técnicos `.md` | Sección temática (`02` a `12`) |
| Bitácoras | `01-BITACORA-DE-ACTIVIDADES/AAAA/MM-MES/` |
| Capturas de pantalla | `08-EVIDENCIAS-Y-ADJUNTOS/01-CAPTURAS-PANTALLA/` |
| Fotografías | `08-EVIDENCIAS-Y-ADJUNTOS/02-FOTOGRAFIAS/` |
| Otras imágenes | `08-EVIDENCIAS-Y-ADJUNTOS/03-IMAGENES/` |
| PDF | `08-EVIDENCIAS-Y-ADJUNTOS/04-DOCUMENTOS-PDF/` |
| Word | `08-EVIDENCIAS-Y-ADJUNTOS/05-DOCUMENTOS-WORD/` |
| Excel | `08-EVIDENCIAS-Y-ADJUNTOS/06-ARCHIVOS-EXCEL/` |
| CSV | `08-EVIDENCIAS-Y-ADJUNTOS/07-ARCHIVOS-CSV/` |
| XML | `08-EVIDENCIAS-Y-ADJUNTOS/08-ARCHIVOS-XML/` |
| Diagramas | `08-EVIDENCIAS-Y-ADJUNTOS/09-DIAGRAMAS/` |
| Documentación de proyectos | `06-PROYECTOS/` (estado actual) |
| Informes | `09-INFORMES-Y-REPORTES/` |
| Procedimientos y manuales | `12-PROCEDIMIENTOS-Y-MANUALES/` |

## Principios

- Nombres descriptivos, sin espacios ni caracteres especiales.
- Prefijos numéricos para mantener el orden.
- No duplicar evidencias: referenciarlas una sola vez.
- No registrar contraseñas, tokens ni datos sensibles.
- No crear subcarpetas de actividades futuras hasta que existan archivos reales.

## Conservación

Los archivos que ya existían fuera de `LA-MUELA-SISTEMAS/` no se movieron ni se modificaron. Si se versiona este repositorio con Git, las carpetas vacías se conservan con `.gitkeep`.
