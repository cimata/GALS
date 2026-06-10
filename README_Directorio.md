# Directorio de gestores y analistas — Janus Henderson

Buscador filtrado de gestores (PMs) y analistas de Janus Henderson para
peticiones de prensa: encuentra rápidamente a quién preguntar según el tema,
la clase de activo, la región o el rol.

El archivo es **`JH_PMs_Analysts.xlsx`**. Toda la búsqueda vive en la pestaña
**`Directorio`**; los datos están en la pestaña **`JHers`** (130 profesionales).

## Cómo usarlo

Escribe o elige en la fila de filtros (fila 5). Deja un filtro **en blanco**
para "cualquiera". Los resultados se actualizan solos debajo.

| Filtro | Cómo funciona |
|---|---|
| **Buscador global 🔎** (columna A, la primera) | Estilo Google y **la casilla por defecto para buscar**: rastrea **todos** los campos a la vez (nombre, rol, clase, sub-clase, región, temática, fondo, ISIN y URLs). Admite **varias palabras** (deben aparecer todas, en cualquier campo y orden: `esg credito`), **términos incompletos** (`biotec`, `sostenib`) e **ignora tildes** (`japon` encuentra «Japón»). |
| **Clase de activo** | Desplegable limpio (Renta variable, Renta fija, Multiactivo, Alternativos, Perfil ejecutivo). Coincidencia por texto, así que "Renta fija" también encuentra a quien gestiona "Renta variable / Renta fija". |
| **Sub-clase / estilo** | Texto libre (p. ej. `growth`, `crédito`, `cuantitativo`). |
| **Región** | Desplegable limpio (Global, Estados Unidos, Europa, Reino Unido, Japón, Asia Pacífico, Mercados emergentes, China, Australia, América, Norteamérica, Latinoamérica). Por texto: "Europa" también encuentra "Europa / Global". |
| **Temática / palabra clave** | Texto libre y **amplio**: busca a la vez en temática, rol oficial, sub-clase y nombre del fondo. Ideal para consultas tipo `tech`, `ESG`, `high yield`, `japan`. |
| **Tipo de rol** | Desplegable (Portfolio Manager, Analista, Portfolio Manager + Analista, Otro). |
| **Nombre contiene** (última columna) | Texto libre. Busca solo dentro del nombre. |

Puedes combinar varios filtros a la vez (p. ej. Clase de activo = *Renta
variable* + Región = *Estados Unidos*). Para limpiar, borra el contenido de las
celdas de la fila 5.

## Qué mejora respecto a la versión anterior

- **Desplegables limpios y curados** en clase de activo, región y tipo de rol
  (antes mostraban valores duplicados, `NO_DATO` y categorías combinadas).
- **Coincidencia por texto** en clase y región: una categoría base encuentra
  también las entradas combinadas (antes exigía coincidencia exacta).
- **Búsqueda por palabra clave ampliada**: el campo de temática ahora también
  mira el rol, la sub-clase y el fondo, así que una palabra de prensa encuentra
  al profesional aunque el término esté en su cargo o en el nombre del fondo.
- **Sub-clase como texto libre** en lugar de un desplegable de ~100 valores.
- **Buscador global estilo Google** en la **primera columna** (celda A5): una
  sola caja que busca en todos los campos, con varias palabras, términos
  incompletos y sin tildes; colocada la primera para ir a ella de forma intuitiva.

## Requisitos

Excel con funciones de matriz dinámica (`FILTER`, `CHOOSECOLS`):
Microsoft 365 o Excel 2021+. El resultado se "derrama" automáticamente bajo la
cabecera de la fila 8.

## Mantener los datos

Para añadir o corregir profesionales, edita la pestaña `JHers`
(las columnas A–K). El buscador de `Directorio` los recoge automáticamente.
