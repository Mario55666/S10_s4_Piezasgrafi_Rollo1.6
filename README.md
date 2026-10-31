# Simulador 3D · Gran formato Epson SureColor S60600L

Página web autocontenida para la Unidad didáctica **Producción y publicación de piezas gráficas** del IES Público Diseño y Comunicación (IDC). Reúne:

- un simulador 3D de una impresora eco-solvente rollo a rollo de 1,6 m;
- un tutorial por fases y un glosario de términos técnicos;
- una guía de procedimientos de operación y seguridad;
- un ejercicio resuelto de verificación previa de una lona;
- un verificador de archivos TIFF, PNG, JPEG y PDF;
- los anexos de control de calidad;
- un generador de reporte PDF por estudiante;
- un mecanismo para importar los valores de referencia del cuaderno NotebookLM del curso.

- Autor: Mg. Mario Quiroz Martínez, 2026
- Publicación: https://claude.ai/artifact/L6oG5zz26sE2GxgqSJwpej
- Formato: un archivo HTML (`dist/index.html`, ≈ 3,1 MB). Lleva incrustados los estilos, los scripts, las imágenes, dos TIFF y un PDF de prueba, y el script de extracción de NotebookLM.
- Fuente principal: página de producto de Epson Perú (SCS60600L), consultada el 30/10/2026.

---

## 1. Equipo modelado

| Parámetro | Valor | Fuente |
|---|---|---|
| Cabezales | 2 × PrecisionCore TFP de 8 canales, gota a demanda | Ficha |
| Configuración | 360 boquillas × 2 canales × 2 cabezales × 4 colores | Ficha |
| Resolución máxima | 1440 × 1440 dpi; gota mínima 4,2 pl, 3 tamaños | Ficha |
| Velocidad borrador | 94 m²/h | Ficha |
| Velocidad producción | Lona 51 m²/h · vinil 28,7 m²/h | Ficha |
| Velocidad calidad | Lona 28,7 m²/h · vinil 17 m²/h | Ficha |
| Tinta | UltraChrome GS3, C M Y K (T45L120 / 220 / 320 / 420) | Ficha |
| Suministro | 8 bolsas de 1500 ml (C M Y K × 2) | Ficha |
| RIP | Onyx Thrive | Ficha |
| Ancho de sustrato | 305–1626 mm; área máxima de impresión 1610 mm; márgenes 5 mm | Ficha |
| Espesor de sustrato | ≤ 1 mm | Ficha |
| Rollo | Núcleo 2" o 3" · Ø ≤ 250 mm · entrada ≤ 45 kg · salida ≤ 43 kg | Ficha |
| Calentadores | Pre 30–50 °C · platina 30–50 °C · post 30–55 °C | Hoja de especificaciones SC-S60600 |
| Entorno | 10–35 °C · 20–80 % HR (recomendado 40–60 %) | Ficha |
| Desgasificación antes de laminar | ≥ 6 h | Ficha |
| Dimensiones / peso | 2616 × 609 × 1346 mm · 336 kg | Ficha |
| Alimentación | 100–120 V (10 A) o 200–240 V (5 A), 50/60 Hz; 2 × 110 V + 1 × 110 V para la secadora | Ficha |
| Consumo | Operación ≈ 650 W · calentadores en reserva ≈ 520 W · reposo ≤ 3,5 W | Ficha |
| Ruido | ≈ 59 dB (ISO 7779) | Ficha |

La ficha peruana no incluye las temperaturas de los calentadores. Se tomaron de la hoja de especificaciones de la SureColor S60600, la versión anterior con cartuchos.

Discrepancias anotadas en la página:

1. El campo «Diámetro máximo del rollo» mezcla medidas. Se usa 250 mm.
2. La corriente de la secadora («20 A a 110–120 VCA o 0,5 A a 200–240 VCA») no es coherente entre sí. Debe confirmarse con el manual.
3. La descripción general asigna 51 y 28,7 m²/h a exteriores e interiores. La tabla los asigna a lona y vinil en modo producción.
4. La S60600 con cartuchos de 700 ml figura como descontinuada en Epson EE. UU. La S60600L usa bolsas de 1,5 L.

---

## 2. Secciones de la página

| N.° | Sección | Contenido |
|---|---|---|
| — | Portada | Título, canales C M Y K × 2, seis indicadores de ficha |
| 01 | Simulador | Escena 3D con seis vistas (operación, explosionada, circuito de tinta, recorrido del sustrato, rótulos, vista general), pantalla LCD, mandos, parámetros, bolsas de tinta, advertencias y registro de eventos |
| 02 | Estructura y mecanismos | Tarjetas de componentes; cada una enfoca la pieza en 3D |
| 03 | Sistema de tinta | Esquema bolsas → cabezales → estación de tapado → botella residual |
| 04 | Sustratos | 8 sustratos con gramaje, espesor, rollo, peso y diámetro calculados, consignas de calentadores, laminado, resolución mínima y estado de carga |
| 05 | Diagrama de procesos | 10 etapas, de Archivo a Acabado, sincronizadas con el simulador |
| 06 | Protocolos de seguridad | Ítems marcables por grupo de riesgo con etiqueta Ficha / Práctica general |
| 07 | Especificaciones | Tablas de ficha y discrepancias |
| 08 | Costos y tamaños | Límites de formato, panelado, calculadora de costo de material, tinta, acabado y energía |
| 09 | Guía GP-GF-01 | Objetivo, alcance, marco normativo, responsabilidades, EPP, POE, matriz IPERC 3 × 3, registro por sesión |
| 10 | Arte final | Ejercicio resuelto (lona 1500 × 900 mm), montaje con ojales, zonas, imagen con errores, verificador |
| A | Anexo A | Ficha técnica de verificación |
| B | Anexo B | Checklist por bloques con firmas |
| — | Reporte PDF | Formulario del estudiante y generación del PDF |

Herramientas presentes en toda la página:

- en la barra superior, los botones **Tutorial** y **Glosario** y el indicador **Cuaderno** («sin vincular» / «vinculado»);
- abajo a la izquierda, los lanzadores flotantes del tutorial y del glosario.

---

## 3. Simulador 3D

- **Escala:** 1 unidad = 10 cm. Geometría esquemática construida con primitivas a partir de las medidas exteriores de la ficha.
- **Tiempo simulado:** ×20 por defecto; el tutorial lo lleva a ×3600 en las esperas largas. El factor vigente se muestra en la escena.
- **Avance del sustrato:** (m²/h del modo y clase de sustrato ÷ ancho imprimible) ÷ 3600. Los sustratos sin clase en la ficha (papel, canvas) usan la velocidad de vinil y se rotulan como estimación.
- **Calentadores:** respuesta de primer orden con τ = 90 s simulados. Al cargar un sustrato, la consigna toma sus valores. Mientras alguna zona no está a ±2 °C de su consigna, la pantalla indica PRECALENTANDO y el carro no se mueve.
- **Estados de pantalla:** APAGADO, INICIALIZANDO, SIN SUSTRATO, EN ESPERA, LISTO, PRECALENTANDO, IMPRIMIENDO, LIMPIEZA, FALLO: TAPA, PARO EMERG.

**Interbloqueos que impiden la acción:**

- paro de emergencia, que corta movimiento y calentadores y exige rearme manual;
- tapa frontal abierta;
- rollo fuera de ficha: espesor > 1 mm, peso > 45 kg, Ø > 250 mm o ancho fuera de 305–1626 mm;
- trabajo más ancho que el área imprimible del sustrato, que obliga a panelar.

**Advertencias, que permiten seguir:**

- local o humedad fuera de rango;
- consigna sobre la temperatura máxima del sustrato;
- post-calentador bajo sin secadora;
- extracción apagada durante la impresión;
- bobinador desactivado;
- rollo de salida > 43 kg;
- bolsa con menos del 15 %;
- laminado antes del tiempo de desgasificación.

**Consumo de tinta:** 15 ml/m² a TAC 300 %, escalado por el TAC medio del trabajo (práctica general, estimación).

---

## 4. Tutorial por fases

Es un panel flotante que guía la operación sobre el simulador real y lee su estado cada 400 ms. Tiene 9 fases y 22 pasos:

| Fase | Pasos |
|---|---|
| 1. Preparación del puesto | EPP y HDS · condiciones del local |
| 2. Control previo del arte | Cargar el arte en el verificador · registrar el Anexo A |
| 3. Encendido | Encender · extracción de vapores |
| 4. Carga del sustrato | Sustrato apto · cargar el rollo · tapa cerrada y bobinador activo |
| 5. Mantenimiento previo | Patrón de inyectores · limpieza (opcional) |
| 6. Calentadores y RIP | Consigna de calentadores · modo de impresión · envío del trabajo |
| 7. Impresión | Iniciar · supervisar hasta el final |
| 8. Desgasificación y acabado | Espera ≥ 6 h · laminado (opcional según sustrato) · corte y ojales |
| 9. Cierre y registro | Descargar · apagar · reporte PDF |

Funcionamiento:

- **Avance:** los pasos se completan solos cuando el simulador cumple la condición. Los que el simulador no puede detectar se cierran con «Hecho», y los opcionales con «Omitir».
- **Resaltado:** el control de cada paso se resalta y se desplaza a la vista. Con `prefers-reduced-motion` el contorno no se anima.
- **Estado en vivo:** temperaturas, avance de la impresión y horas de desgasificación transcurridas.
- **Acelerador:** en impresión y desgasificación lleva el reloj a ×3600. Vuelve a ×20 al salir del paso o cerrar el panel.
- **Enlaces:** los términos subrayados abren el glosario.

---

## 5. Glosario

Es un diálogo emergente con 79 términos en 8 categorías: archivo y color, calidad, equipo, proceso, seguridad, sistema de tinta, software y sustrato.

- **Contenido de cada entrada:** definición, fuente, alias y acceso a la sección de la página. Si el término corresponde a una pieza del modelo, también trae el botón «Ver en 3D».
- **Búsqueda:** por nombre, alias o definición, sin distinguir acentos. Hay filtro por categoría e índice alfabético.
- **Apertura:** desde la barra, el lanzador, cualquier término enlazado (`data-term`) o el atajo **Alt+G**.

---

## 6. Verificador de archivo

El análisis se ejecuta en el navegador; el archivo no se envía a ningún servidor. Al cargar un archivo se actualizan:

- el montaje con ojales y las zonas;
- la imagen con errores;
- el film del modelo 3D y el trabajo del RIP;
- la calculadora de costos.

Los botones de resultado pasan la medición al Anexo A como control previo o como valor final.

| Formato | Lectura | Controles |
|---|---|---|
| TIFF | UTIF.js + pako; etiquetas 262, 277, 258, 282/296, 34675 | Modo y perfil ICC, resolución declarada, tamaño frente a final + sangrado, sangrado deducido, panelado, peso; en CMYK de 8 bits, TAC máximo y medio con mapa de píxeles > límite |
| PNG | Chunks `IHDR`, `pHYs`, `iCCP` | Los mismos; TAC solo estimado (RGB) |
| JPEG | `APP0 JFIF`, `APP2 ICC_PROFILE`, componentes del `SOF` | Los mismos; TAC estimado si es RGB |
| PDF | pdf-lib 1.17.1 (estructura) + pdf.js 4.10.38 (render y operadores) | Ver abajo |

Controles específicos de PDF (página 1):

- **Formato, modo de color y perfil:**
  - versión del PDF y OutputIntent (identificador y perfil ICC);
  - espacios de color de las imágenes;
  - operadores de color de los flujos de contenido: `k/K` CMYK, `rg/RG` RGB, `g/G` gris. El resultado se clasifica como CMYK, RGB o mixto.
- **Tamaño de página:** BleedBox o, si no existe, MediaBox, frente a final + sangrado ± tolerancia.
- **TrimBox y sangrado:** formato final frente al objetivo; sangrado = distancia mínima entre TrimBox y BleedBox.
- **Resolución efectiva:** se recorre la lista de operadores acumulando la matriz de transformación. En cada imagen, ppi = píxeles ÷ (ancho colocado en pt ÷ 72); se informa el mínimo y el número de imágenes. Sin imágenes, el contenido figura como vectorial.
- **Fuentes:** diccionarios `/Font` con `FontFile`, `FontFile2` o `FontFile3`; lista de las no incrustadas.
- **Cobertura total de tinta:** máximo exacto de los vectores CMYK (suma de los operandos de `k/K` × 100) y media estimada del render.
- **Páginas:** observación si hay más de una.
- **Zona segura de ojales:** no es medible; queda como observación con la referencia.

**Archivos de prueba incrustados:**

| Archivo | Descripción | Resultado |
|---|---|---|
| `arte_v1_lona_control_previo.tif` | 1500 × 900 mm, 72 ppi, CMYK sin perfil, sin sangrado, negro 400 % | Desviaciones en perfil, resolución, tamaño, sangrado y TAC |
| `IDC_GF_lona_1500x900_sangrado10_100ppi_CMYK.tif` | 1520 × 920 mm, 100 ppi, CMYK FOGRA39, TAC ≤ 300 % | Conforme |
| `IDC_GF_lona_1500x900_sangrado10_PDF.pdf` | Vectorial CMYK, 2 fuentes incrustadas, logo CMYK a 119 ppi efectivos, TrimBox 1500 × 900 mm, BleedBox 1520 × 920 mm, OutputIntent FOGRA39 | Conforme; TAC máximo de vectores 240 % |

---

## 7. Valores de referencia del curso (NotebookLM)

El cuaderno del curso (ID `cd735b07-b253-41af-b16f-2f2a03b0e705`) no permite lectura externa desde la página. Mientras no se importe, los valores salen del PDF de Epson Perú y las temperaturas, de la hoja de la S60600.

La primera vez que se carga un arte final se abre el diálogo «Cuaderno del curso en NotebookLM». El diálogo muestra ese estado, los enlaces al cuaderno y al repositorio [notebooklm-py](https://github.com/teng-lin/notebooklm-py), y dos vías de importación.

**Vía A · script local** (`notebook/extraer_parametros_notebooklm.py`)

```bash
pip install "notebooklm-py[browser]"
playwright install chromium
notebooklm login                 # cuenta de Google con acceso al cuaderno
python extraer_parametros_notebooklm.py [--notebook ID] [--salida parametros_curso_gf.json] [--perfil PERFIL]
```

- **Funcionamiento:** el script envía al cuaderno una consulta que pide solo JSON con datos de sus fuentes, con `null` donde falte el dato. Extrae el bloque JSON, quita las marcas de cita `[n]` y valida rangos.
- **Archivos que genera:** `parametros_curso_gf.json` y `respuesta_notebooklm.md`, con la respuesta completa para revisión docente.
- **Limitación:** notebooklm-py es un cliente no oficial que usa interfaces internas de Google, sujetas a cambios.
- **Descarga desde la página:** se entrega como `.py.txt`, porque el entorno de descargas no admite `.py`. Hay que renombrarlo antes de ejecutarlo.

**Vía B · chat del cuaderno.** Se copia la consulta desde la página, se pega en el chat de NotebookLM y la respuesta se pega en el área de texto.

**Esquema JSON**

```json
{
  "sustratos": { "lona13": { "pre": null, "platina": null, "post": null, "ppi_min": null } },
  "tac_max_pct": null, "sangrado_mm": null, "zona_segura_mm": null, "tolerancia_mm": null,
  "desgasificacion_h": null, "temp_local_c": [null, null], "hr_recomendada_pct": [null, null],
  "notas": "",
  "_meta": { "fuente": "NotebookLM", "cuaderno_id": "", "cuaderno": "", "fecha": "" }
}
```

Claves de sustrato: `lona13`, `lona18`, `malla`, `vinil`, `micro`, `papel`, `canvas`.

**Efecto de la importación**

- Actualiza:
  - las consignas y la resolución mínima de cada sustrato;
  - el límite de TAC del verificador y el mapa de defectos;
  - el sangrado y la tolerancia del formato objetivo;
  - la zona segura y las horas de desgasificación;
  - los rangos de temperatura y humedad del simulador.
- Muestra la tabla «parámetro | antes | cuaderno».
- Cambia la etiqueta de fuente a **Curso (NotebookLM)** en las filas modificadas del Anexo A.
- Agrega al reporte PDF el origen y la fecha de los valores.
- Se guarda en `localStorage` de ese navegador. «Volver a los valores de la ficha» restablece la línea base.

---

## 8. Anexos y reporte

- **Anexo A · Ficha técnica de verificación:**
  - cabecera con institución, unidad, docente, estudiante, pieza, técnica, archivo, origen y fecha;
  - 16 filas: formato y perfil, ancho, alto, sangrado, ancho imprimible, resolución, TAC, peso, zona segura, espesor, peso de rollo, post-calentador, temperatura del local, desgasificación, patrón de inyectores y medida final;
  - columnas: referencia, fuente, medido, desviación, corrección, final y conforme;
  - cálculo por tipo: mínimo, máximo, rango, tolerancia o selección.
- **Anexo B · Checklist:** bloques de archivo, equipo y seguridad, sustrato, impresión, y desgasificación y acabado. Cada ítem remite al Anexo A o a la etapa del proceso.
- **Reporte PDF** (jsPDF 2.5.1 + AutoTable 3.8.2):
  - nombre y apellidos obligatorios;
  - el dictamen combina Anexo A y verificador: no declara APTO si el verificador encontró desviaciones;
  - advierte si el archivo del Anexo A no coincide con el analizado;
  - incluye arte y montaje, resultado del verificador, Anexo A, Anexo B, firmas y pie institucional;
  - se descarga con la capacidad `downloads` del entorno de artefactos.

---

## 9. Etiquetas de fuente

| Etiqueta | Uso |
|---|---|
| Ficha | Página de producto de Epson Perú u hoja de especificaciones de la S60600 |
| Curso (NotebookLM) | Valores importados del cuaderno del curso |
| Taller | Criterio fijado para el ejercicio (sangrado 10 mm, zona segura 30 mm, ojales a 15 mm, tolerancia ± 2 mm) |
| Práctica general | Valor habitual de la técnica eco-solvente; confirmar con la ficha del consumible |
| Estimación / reemplazar | Cálculo propio o precio sin cotización local |

---

## 10. Estructura del proyecto

```
gf/
├── base.css, extra.css        estilos
├── body.html, body2.html      marcado de las secciones
├── data.js                    sustratos, velocidades, límites (window.GF)
├── app.js                     tablas, costos, guía, Anexo A, verificador (TIFF/PNG/JPEG/PDF), Anexo B, reporte, importación del curso
├── sim.js                     módulo 3D: escena, rótulos, vistas, estado (window.__sim), bucle
├── glossary.js                glosario emergente
├── tutorial.js                tutorial por fases
├── notebook.js                diálogo de vínculo con NotebookLM
├── notebook/
│   └── extraer_parametros_notebooklm.py
├── arte/
│   ├── make_svg.py, render.js, build.py   generación de los TIFF del ejercicio (FOGRA39, límite de TAC)
│   ├── make_pdf.py                        generación del PDF de prueba (reportlab + pikepdf)
│   └── *.tif, *.pdf, *.jpg, *.png
├── build.py                   ensambla dist/index.html e incrusta imágenes, TIFF, PDF y script
└── dist/index.html            entregable
```

Construcción:

```bash
python3 build.py                                   # genera dist/index.html
for f in /tmp/g*.mjs; do node --check "$f"; done   # comprueba la sintaxis de cada bloque de script
```

Bibliotecas (versiones fijas, CDN jsDelivr): Three.js 0.186.1, Anime.js 4.5.0 (adaptador Three), UTIF.js 3.1.0, pako 1.0.11, pdf-lib 1.17.1, pdfjs-dist 4.10.38, jsPDF 2.5.1, jspdf-autotable 3.8.2. Fuentes: IBM Plex Sans e IBM Plex Mono (Google Fonts).

---

## 11. Pruebas realizadas

Las pruebas se hicieron con Playwright y Chromium con renderizado por software:

- verificador con los dos TIFF, el PDF conforme y un PDF con RGB, sin sangrado, imagen a 25 ppi, Helvetica sin incrustar y 2 páginas;
- importación del curso con JSON pegado (con marcas de cita) y comprobación de los cambios en `LIM`, el Anexo A y las referencias de tamaño;
- recorrido del tutorial de la fase 1 a la 9, con avance automático, pasos manuales y opcionales, y acelerador de reloj;
- glosario: búsqueda, filtro y apertura desde términos enlazados;
- descarga del reporte PDF y del script con un sustituto de la capacidad `downloads`.

---

## 12. Limitaciones

- Geometría 3D esquemática: los componentes internos no descritos en la ficha se representan sin medidas reales.
- La zona segura de ojales no se mide de forma automática.
- En PDF se analiza solo la página 1. El TAC de las imágenes y el TAC definitivo dependen del perfil de salida del RIP.
- pdf.js se carga desde jsDelivr. Si la política del entorno bloquea su trabajador (worker), pdf.js ejecuta el análisis en el hilo principal, que es más lento en archivos grandes.
- Precios de tinta, laminado, ojales y energía: estimaciones marcadas «reemplazar» hasta contar con cotización local.
- La lectura del cuaderno NotebookLM requiere ejecutar el script con la cuenta del docente o pegar la respuesta del chat.

---

Mg. Mario Quiroz Martínez 2026 — Unidad didáctica de Producción y publicación de piezas gráficas
