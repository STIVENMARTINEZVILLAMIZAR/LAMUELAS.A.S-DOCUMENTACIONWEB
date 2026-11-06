
# Informe diario de actividades — Analista de Sistemas / Gestión Web

**Empresa:** LA MUELA S.A.S.  
**Fecha:** 5 de noviembre de 2026  
**Área:** Sistemas / Administración de página web y comercio electrónico  
**Sitio:** https://lamuela.com.co/  
**Estado del informe:** Registro de actividades y seguimiento (no equivale a acta de cierre técnico)

## 1. Objetivo de la jornada

Realizar actividades de análisis y mantenimiento del sitio web de LA MUELA S.A.S., revisar datos de adquisición de tráfico y gestionar el cargue de un artículo odontológico en WooCommerce, procurando conservar trazabilidad de los cambios y evidencia de los asuntos pendientes.

## 2. Actividades realizadas

### 2.1. Análisis de Google Analytics 4 y Google Ads

- Se revisaron informes de adquisición de tráfico de GA4 para el período comprendido entre el **1 de enero y el 5 de noviembre de 2026**.
- Se examinaron los medios de adquisición y nombres de campañas, incluidos registros `paid`, `cpc` y `ppc`.
- Se identificaron diferencias de etiquetado y registros incompletos de atribución, pendientes de comprobación por plataforma.
- Se revisó la cuenta de Google Ads mostrada en pantalla, en la que figuraban anuncios sin publicación activa para el período consultado.
- Se preparó un informe de adquisición y publicidad digital en Excel y **se remitió a la coordinadora**.

**Resultado:** Informe remitido. Queda pendiente la validación del origen de campañas, inversión publicitaria y conversiones comerciales.

### 2.2. Gestión del producto «Eyector de conductos» en WooCommerce

- Se revisó la ficha técnica del fabricante **Specialized Ltda.**, correspondiente al **Eyector de conductos #1 (1,60 mm)**, código del fabricante **EA-E-001**.
- Se identificó en SAP Business One el artículo **SPEC-8 — EYECTOR DE CONDUCTO**, perteneciente al grupo Odontología, con indicador tributario `IVAG-V19`.
- Se prepararon nombre comercial, descripción corta, descripción larga en HTML básico y etiquetas para la ficha web.
- Se cargó una imagen del producto en la biblioteca de medios de WordPress:  
  https://lamuela.com.co/wp-content/uploads/2026/11/EYECTOR-DE-CONDUCTOS.png
- Se preparó una versión de la ficha técnica en imagen PNG para usarla como recurso de consulta en la ficha del producto.
- Se identificaron los códigos de clasificación comunicados para la plantilla:
  - **4147 — Odontología**
  - **1791 — Instrumental Dental**
- Se realizaron mediciones físicas del instrumento:
  - **Longitud:** 9 cm.
  - **Peso:** 13 g (0,013 kg).
- Se diligenciaron o revisaron los campos visibles de la ficha de WooCommerce: nombre, contenido, imagen, categorías, marca, datos del producto y precio.
- Se comprobó la visualización del artículo en la tienda.
- Se seleccionó **SPECIALIZED LTDA** en los controles de marca disponibles en el editor.

**Resultado:** Artículo cargado y visible en la tienda. Requiere control de calidad de los datos finales y validación de la sincronización con SAP.

### 2.3. Verificación de precios e impuestos

- Se confirmó que el precio comercial informado para el eyector es **$51.000 COP, IVA incluido**.
- Se verificó que WooCommerce agrega el IVA del 19 % al precio base.
- Con $51.000 antes de impuestos, la página mostraba **$60.690**.
- Se calculó como referencia un precio base de **$42.857,14** para obtener $51.000 con IVA, sujeto al tratamiento de redondeo y la integración con SAP.
- En una captura posterior, el precio normal aparecía como **$42.900 sin impuestos**.
- Ese valor daría **$51.051** con IVA del 19 %, por lo que queda pendiente confirmar el precio final publicado y corregir la diferencia si aplica.

**Resultado:** Identificada una diferencia de criterio entre precio base y precio final; verificación final pendiente.

### 2.4. Revisión de presentación, marca y medidas del producto

- Se observó que la marca estaba seleccionada en WordPress, pero no aparecía en el bloque de información adicional de la ficha pública.
- Se abrió la plantilla de producto individual en Elementor y se ubicó el widget **«Información adicional»**.
- Se identificó que la marca seleccionada en las taxonomías de marcas no necesariamente se presenta en ese widget, que muestra atributos e información del producto.
- Se detectó un **error de peso** en la vista pública:
  - Peso mostrado: 13 kg.
  - Peso real: 0,013 kg.
- Se recomendó corregir el peso en el origen de datos autorizado y comprobar la visualización posterior.

**Resultado:** Problemas identificados. No consta en la evidencia revisada que el peso y la visualización de marca hayan quedado corregidos.

### 2.5. Localización de una imagen de medios de pago

- Se investigó la ubicación del recurso `medios-de-pago-bold.png` dentro del sitio.
- Se identificó mediante el inspector del navegador que la imagen estaba asociada a un **widget de imagen de Elementor**.
- Se localizó la plantilla de producto individual que contiene dicho recurso.

**Resultado:** Ubicación del recurso identificada. No se da por confirmada la sustitución definitiva de la imagen sin evidencia de publicación.

### 2.6. Organización de documentación técnica

- Se organizó el seguimiento de auditorías, tareas e incidencias en el repositorio de documentación Markdown administrado desde Cursor.
- Se definió el uso de archivos `.md` y carpetas de evidencias para conservar historial de las actividades.

**Resultado:** Proceso documental en uso; continuar registrando evidencias y estados de cierre.

## 3. Hallazgos y pendientes de seguimiento

| ID | Hallazgo / pendiente | Prioridad | Estado | Próxima acción |
|---|---|---|---|---|
| WEB-001 | Precio final del SPEC-8 debe ser $51.000 IVA incluido; se observó base de $42.900 | Alta | Pendiente de verificación | Comprobar importe en la tienda y ajustar por el procedimiento autorizado |
| WEB-002 | Peso público del SPEC-8 mostrado como 13 kg en vez de 0,013 kg | Alta | Pendiente de corrección/validación | Revisar datos de envío y confirmar sincronización desde SAP |
| WEB-003 | La marca SPECIALIZED LTDA no se muestra en el widget de información adicional | Media | En análisis | Revisar taxonomía/atributo y el alcance de la plantilla global |
| WEB-004 | Correspondencia exacta entre el código SAP SPEC-8 y el modelo #1 de la ficha del fabricante | Alta | Pendiente de validación | Confirmar con responsable de catálogo o ingeniero |
| WEB-005 | Imagen de medios de pago Bold: confirmar sustitución en plantilla | Baja | Por verificar | Comprobar archivo corregido y resultado publicado |
| MKT-001 | Campañas `paid`, `cpc`, `ppc` con atribución incompleta | Media | En análisis | Identificar origen, gasto y conversiones reales |
| INT-001 | Confirmar responsabilidad y reglas del cargue SAP–WooCommerce | Alta | Pendiente | Verificar con ingeniero para evitar sobrescrituras o duplicados |

## 4. Recomendaciones

1. Validar **precio, impuestos, peso e inventario** del artículo SPEC-8 contra SAP y contra la ficha pública antes de dar por finalizado el cargue.
2. Evitar modificaciones de código, plugins o plantillas globales sin autorización del ingeniero.
3. Registrar capturas «antes/después» y enlaces de evidencia para cada incidencia resuelta.
4. Continuar con el cruce de precios y referencias de SAP–WooCommerce y, posteriormente, preparar Black Friday con precios y productos aprobados.

## 5. Estado de cierre de la jornada

**Actividades completadas:**

- Revisión del tráfico y campañas de adquisición.
- Elaboración y envío del informe a coordinación.
- Preparación documental y comercial del producto.
- Carga y revisión inicial de su ficha web.
- Identificación de hallazgos técnicos.
- Organización del seguimiento documental.

**Pendientes de validación:**

- Precio final con IVA.
- Peso correcto del artículo.
- Visualización de la marca.
- Correspondencia de referencia.
- Confirmación de sincronización SAP–WooCommerce.
- Cierre de cambios globales.

**Observación:** Este documento describe las acciones respaldadas por las capturas y datos compartidos. No da por ejecutadas correcciones cuya publicación o verificación no quedó confirmada.
