# Página web de cumpleaños

Estructura:

cumple_web/
├── index.html
├── styles.css
├── script.js
└── assets/
    ├── images/
    ├── audio/
    └── video/

## 1. Personalizar nombre y edad

Abre `script.js` y modifica:

```js
const birthday = {
  name: "NAME",
  age: 20
};
```

## 2. Agregar mensajes

En `script.js`, dentro de `messages`, agrega:

```js
{
  from: "Mamá",
  text: "Feliz cumpleaños...",
  icon: "💜"
}
```

## 3. Agregar audios

Copia el archivo a `assets/audio/`, por ejemplo:

`assets/audio/mama.mp3`

Luego agrega en `audios`:

```js
{
  name: "Mamá",
  description: "Un mensaje desde casa",
  file: "assets/audio/mama.mp3",
  icon: "🎙️"
}
```

## 4. Agregar videos

Copia el video a `assets/video/`.

Recomendación: MP4 con H.264 + AAC.

Luego agrega:

```js
{
  name: "La familia",
  description: "Un saludo especial",
  file: "assets/video/familia.mp4",
  poster: ""
}
```

## 5. Agregar fotos

Copia tus imágenes en `assets/images/`.

Después agrega objetos al arreglo `photos`:

```js
{
  file: "assets/images/foto-5.jpg",
  alt: "Recuerdo con la familia"
}
```

## 6. Probar en tu PC

Puedes abrir directamente `index.html`.

Para una prueba más parecida a GitHub Pages, desde VS Code puedes usar Live Server si ya lo tienes instalado.

## 7. Publicar en GitHub Pages

1. Crea un repositorio nuevo.
2. Copia todos estos archivos al repositorio.
3. Haz commit y push.
4. En GitHub abre:
   Settings → Pages.
5. En Source selecciona:
   Deploy from a branch.
6. Rama:
   `main`
7. Carpeta:
   `/ (root)`
8. Guarda.

GitHub te mostrará la URL pública de la página.

## Nota importante sobre archivos multimedia

Si subes videos muy pesados, GitHub puede limitar el tamaño del archivo. Para una página ligera, intenta comprimir los videos antes de subirlos.

GitHub normalmente no acepta archivos individuales mayores de 100 MB mediante Git tradicional.
