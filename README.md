# Escudo AR

Experiencia de realidad aumentada hecha con **A-Frame 1.5.0** y **MindAR 1.2.5**. La cámara reconoce la tarjeta del escudo y muestra el modelo 3D encima.

## Archivos

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La página de realidad aumentada |
| `targets.mind` | La tarjeta del escudo compilada para MindAR (objetivo 0) |
| `marcador-escudo.png` | La imagen que reconoce la cámara: imprímela o ábrela en otra pantalla |
| `escudo.glb` | Modelo 3D del escudo (optimizado, 1.8 MB) |

## Cómo probarlo

1. Sube los 4 archivos a la misma carpeta de un repositorio y publícalo con GitHub Pages (la cámara necesita **https**).
2. En la computadora también puedes probar con un servidor local: `npx serve .` y abre la dirección `http://localhost:...` que te dé.
3. Acepta el permiso de la cámara y apunta a la tarjeta.

## Ajustes

En `index.html`, dentro de `<a-gltf-model>`:

- `scale`: tamaño del modelo. La tarjeta mide 1 de ancho.
- `position`: posición sobre la tarjeta (x, y, z).
- `rotation`: giro del modelo en grados (x, y, z).

Si cambias la imagen de la tarjeta, vuelve a compilar `targets.mind` con el [compilador de MindAR](https://hiukim.github.io/mind-ar-js-doc/tools/compile).
