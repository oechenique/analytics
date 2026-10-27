# analytics — resumen en español

[🇬🇧 English](README.md)

Geoanálisis inmobiliario en Buenos Aires: cuántos departamentos en venta hay a 800 m de una estación de subte, en línea recta y caminando. Un notebook que corre en Colab o en local, sin credenciales.

- **Datos**: avisos de venta de Properati (`data/real_estate_data.zip`), calles y estaciones de OpenStreetMap, y los barrios de Buenos Aires Data para el contorno de la ciudad.
- **El caso**: la estación Congreso de Tucumán (línea D). En el círculo de 800 m hay **535 departamentos**, pero a 800 m caminando por las calles hay **316**: el 41 % del círculo queda más lejos a pie.
- **El error de 2023**: el buffer estaba en grados (`0,0072°`), que a 34,6°S es una elipse de ~800 × 660 m (470 departamentos), y el mapa de calor mezclaba precios por m² en pesos y en dólares. Ahora todo se mide en metros (POSGAR 2007 / Argentina 5, EPSG:5347) y en USD/m².

El notebook original de 2023 y tres borradores sobre Japón que nunca corrieron quedan en `legacy/`.
