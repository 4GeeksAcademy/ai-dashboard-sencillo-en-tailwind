# Especificación: Dashboard de campañas para influencer

## Objetivo
Crear un dashboard que consolide métricas de Instagram, TikTok y YouTube para que una influencer pueda revisar comisiones, ingresos, conversión, retorno y engagement por plataforma y producto.

## Requisitos técnicos
- Usar únicamente HTML y Tailwind CSS v4 mediante `https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4`.
- No usar JavaScript, React, Vue, CSS personalizado, Charts.css ni otras librerías.
- Usar clases utility de Tailwind; no añadir etiquetas `<style>` ni estilos inline.
- Construir el diseño mobile-first y usar breakpoints Tailwind `sm:`, `md:` y `lg:`.
- Usar HTML semántico: `header`, `nav`, `main`, `section`, `article`, listas y tablas con `caption`, `thead`, `tbody`, `tfoot` y `scope`.

## Estructura
- Cabecera con nombre del dashboard y navegación a sus secciones.
- Bloque superior con al menos 3 KPI.
- Bloque intermedio con al menos 3 drivers de rendimiento.
- Bloque inferior con detalles por plataforma y por producto.
- Reutilizar una estructura y estilo consistentes para tarjetas y datos similares.

## Datos de negocio
- Producto A: 50 €.
- Producto B: 120 €.
- Producto C: 80 €.
- Comisión: 15 % por venta.

## Fórmulas
- Ingresos: suma de ventas por producto multiplicadas por su precio.
- Comisión: ingresos × 0,15.
- Conversión: ventas / alcance × 100.
- Engagement rate: interacciones / alcance × 100.
- ROI: comisión / coste de anuncios.

## Datos de ejemplo por plataforma
| Plataforma | Ventas A/B/C | Ventas | Ingresos | Comisión | Alcance | Coste | Interacciones |
|---|---:|---:|---:|---:|---:|---:|---:|
| Instagram | 120/40/60 | 220 | 15.600 € | 2.340 € | 85.000 | 1.200 € | 5.100 |
| TikTok | 180/25/70 | 275 | 17.600 € | 2.640 € | 150.000 | 1.500 € | 9.750 |
| YouTube | 60/55/45 | 160 | 13.200 € | 1.980 € | 40.000 | 800 € | 1.800 |
| Total | 360/120/175 | 655 | 46.400 € | 6.960 € | 275.000 | 3.500 € | 16.650 |

## Métricas derivadas por plataforma
| Plataforma | Conversión | Engagement | ROI |
|---|---:|---:|---:|
| Instagram | 0,26 % | 6,0 % | 1,95× |
| TikTok | 0,18 % | 6,5 % | 1,76× |
| YouTube | 0,40 % | 4,5 % | 2,48× |
| Total | 0,24 % | 6,1 % | 1,99× |

## Datos de ejemplo por producto
| Producto | Precio | Ventas | Ingresos | Comisión | Alcance | Interacciones | Conversión | Engagement |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| A | 50 € | 360 | 18.000 € | 2.700 € | 120.000 | 7.800 | 0,30 % | 6,5 % |
| B | 120 € | 120 | 14.400 € | 2.160 € | 70.000 | 3.500 | 0,17 % | 5,0 % |
| C | 80 € | 175 | 14.000 € | 2.100 € | 85.000 | 5.350 | 0,21 % | 6,3 % |
| Total | — | 655 | 46.400 € | 6.960 € | 275.000 | 16.650 | 0,24 % | 6,1 % |

## Contenido mínimo
- KPI: comisiones totales, ingresos generados y ROI global.
- Drivers: conversión por plataforma, engagement por plataforma e ingresos por producto.
- Detalle: datos completos por plataforma y producto, incluido engagement por producto.
- Los valores destacados deben poder leerse también como texto; no depender solo del color o de las barras.

## Criterios de aceptación
- La información se presenta en tres bloques con jerarquía visual clara.
- En móvil y tablet, las tablas se presentan como fichas apiladas; en escritorio, como tablas.
- La página no produce scroll horizontal ni contenido superpuesto en móvil, tablet o escritorio.
- Los KPI y drivers se ven correctamente en al menos tres tamaños de pantalla.
- Las tablas y listas incluyen etiquetas comprensibles y semántica accesible.
- Los totales, porcentajes y fórmulas coinciden con los datos proporcionados.
