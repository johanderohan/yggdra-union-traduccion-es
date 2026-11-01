# Yggdra Union: We'll Never Fight Alone — Traducción al español

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Ficha del proyecto, capturas y más traducciones al castellano en **[Parches en Castellano](https://parchesencastellano.com/traducciones/game-boy-advance/yggdra-union)**.

Traducción al **español de España** de *Yggdra Union: We'll Never Fight Alone* (Game Boy Advance,
2006), el juego de estrategia por turnos y cartas de Sting, segundo episodio de la serie
Dept. Heaven, que nunca salió en español.

La traducción se reparte como **parche**: no incluye el juego. Necesitas tu propia copia para
aplicarlo. Se hace **desde el inglés** de la versión europea (la edición europea solo trae inglés);
no es una traducción directa del japonés.

## Estado

Última versión: **[v1.0 — primera versión](../../releases/tag/v1.0)**. Estado: **en revisión**.

| Parte | Estado |
|---|---|
| Diálogos, narraciones y escenas de la historia (14.004 cadenas) | Traducidos |
| Menús, objetos, cartas, clases, habilidades, condiciones y ayudas | Traducidos |
| Texto dibujado en imágenes: narraciones entre capítulos, descripciones, rótulos de lugar, objetivos, tutoriales, fichas, resultados de combate (2.244 imágenes) | Redibujado en castellano |
| Caracteres españoles | **á é í ó ú ü ñ ¡ ¿ « »** en la fuente de diálogos |
| Revisión durante una partida | Parcial (capítulos 1 y 2) |

### Qué se conserva a propósito

- El logotipo del título y el lema **«-WE'LL NEVER FIGHT ALONE-»**.
- Los **rótulos góticos de los conjuros** que aparecen al lanzar una carta: son parte de la
  estética del combate y su sentido se explica en la descripción de cada carta.
- El aviso de salud y legal del arranque.
- Los **nombres propios** de unidades y personajes (Yggdra, Milanor, Durant, Nessiah…).

### Limitaciones conocidas

- Algunos **rótulos de lugar en el mapa** son más largos que en inglés y pueden quedar
  parcialmente tapados por los sprites de las unidades que tienen encima.
- Unos pocos gráficos siguen en inglés: las ilustraciones del Rincón tutorial (los textos que las
  explican sí están traducidos), la pestaña
  «Map» (solo hay sitio para 3 letras), parte de la pantalla de información de clase y alguna
  composición de sprites del combate.
- Las cadenas que el juego escribe con su letra pequeña de 8×8 (p. ej. «Hora», «DE CERCA») van
  **sin tildes**: esa fuente no las tiene.
- En los gráficos el castellano se ha redibujado con fuentes libres parecidas a las originales;
  en algunos rótulos se ve algo más fino o más condensado que el inglés.
- En la ficha de Milanor el recuadro de habilidades tapa la parte de arriba de una letra, igual
  que en el original.

### Qué se ha comprobado

Todo en **emulador** (mGBA mediante libretro). Se ha jugado desde una **partida nueva**, por dos
rutas y en varias rondas: título, introducción y prólogo, tutoriales, el **capítulo 1 completo**
con todos sus combates (elección de cartas, predicción, choque, resultado y botín) hasta el
principio del capítulo 2, menús del mapa, mapa de ayuda, fichas de unidad y de carta, objetos y su
ordenación, suspender y continuar, y guardar la crónica. La última corrección (los nombres de
unidad genéricos en la pantalla de Unión y de experiencia) cambia solo esos gráficos y se ha
comprobado en sus pantallas.

Una auditoría automática comprueba en la ROM montada que cada cadena y cada imagen caben donde
el juego las lee, que todos los punteros apuntan a donde deben, que cada imagen se descomprime
igual que lo hace el juego y que no se ha pisado ningún dato vecino.

**No se ha probado**: una partida completa (solo el capítulo 1 y el principio del 2), los finales,
la consola real ni flashcart. La traducción, la revisión editorial y la QA están hechas con
asistencia de IA, **sin revisión humana independiente**. No se han probado las ediciones USA ni
japonesa.

## Cómo aplicar el parche

1. Descarga el parche `.xdelta` de la sección **[Releases](../../releases)**.
2. Consigue tu copia del juego en versión **europea** (código `BYUP`). El parche solo funciona con
   esa versión exacta: no sirve la estadounidense ni la japonesa.
3. **Comprueba que tu copia es la correcta** antes de nada:

   | | |
   |---|---|
   | Archivo | `Yggdra Union - We'll Never Fight Alone (Europe).gba` |
   | Tamaño | 33.554.432 bytes (32 MiB) |
   | MD5 | `34469cbe444c6561a5a24c1159f0697e` |
   | SHA-1 | `e419c835200457f67d5ab7e3c236583980b922d9` |

   ```bash
   md5sum "Yggdra Union - We'll Never Fight Alone (Europe).gba"     # Linux
   md5 "Yggdra Union - We'll Never Fight Alone (Europe).gba"        # macOS
   CertUtil -hashfile "Yggdra Union - We'll Never Fight Alone (Europe).gba" MD5   # Windows
   ```

   Si no coincide, el parche fallará o dará un resultado corrupto.
4. Aplica el parche con una de estas herramientas:
   - **Windows**: [Delta Patcher](https://github.com/marco-calautti/DeltaPatcher/releases)
   - **En línea**: [Rom Patcher JS](https://www.marcrobledo.com/RomPatcher.js/)
   - **Linux / macOS**: `xdelta3 -d -s "Yggdra Union - We'll Never Fight Alone (Europe).gba" yggdra-union-gba-es-v1.0.xdelta "Yggdra Union (Castellano).gba"`
5. Comprueba que la ROM resultante mide **33.554.432 bytes** y que su MD5 es
   **`cd37dbdfdfa207795270e22cbdae37c2`** (v1.0).
6. Empieza una **partida nueva**. No se ha comprobado que las partidas guardadas con la versión
   inglesa se lleven bien con la traducción, y los estados instantáneos del emulador hechos con otra
   versión pueden mostrar texto mezclado o colgarse.

Aplica cada versión sobre la **ROM europea original**, no sobre una ROM ya traducida.

## Cambios por versión

### v1.0 — primera versión

Traducción completa de diálogos, narraciones, menús, cartas, objetos, clases y ayudas, y redibujado
en castellano del texto que el juego guarda dentro de imágenes. Primera publicación: en revisión.

## Créditos

- Traducción y herramientas: johanderohan, con asistencia de modelos de IA para la ingeniería
  inversa, la traducción, la revisión editorial y las pruebas.
- El texto de las imágenes se ha dibujado a partir de estas fuentes libres:
  - **Liberation Serif / Liberation Sans** (Red Hat; SIL Open Font License 1.1).
  - **DejaVu Serif / DejaVu Sans** y **Bitstream Vera Serif** (DejaVu fonts y Bitstream;
    licencia Bitstream Vera, libre).
  - **Fira Sans** (Mozilla / Carrois; SIL Open Font License 1.1).
  - **Open Sans** (Steve Matteson; SIL Open Font License 1.1).
  - **Noto Serif / Noto Serif Display** (Google; SIL Open Font License 1.1).
- Pruebas: mGBA mediante libretro. Parches: xdelta3.

## Aviso

Este proyecto es una traducción hecha por afición, sin ánimo de lucro y sin relación alguna con
Sting, Atlus, su distribuidora europea ni Nintendo. *Yggdra Union* y todos los nombres, personajes y marcas
asociados pertenecen a sus titulares. Aquí no se distribuye el juego ni ninguna parte de él: solo
un parche que modifica una copia que ya tengas.

Si eres el titular de los derechos y quieres que retire esto, abre una incidencia y lo hago.
