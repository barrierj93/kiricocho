# KIRICOCHO · PLANETA FÚTBOL

Cuatro versiones del logo y sus favicons, listas para una web.

## Carpetas

- `01-fanzine`: grabado con textura y letras irregulares.
- `02-estencil`: letras de esténcil.
- `04-editorial`: composición horizontal con la mano a la izquierda.
- `05-sello`: composición circular.

## Archivos de cada versión

- `logo.svg`: logo en el color de la propuesta original y con fondo transparente.
- `logo-claro.svg`: tinta marfil para fondos oscuros.
- `logo-negro.svg`: tinta negra para fondos claros.
- `favicon.svg`: mano simplificada sobre un cuadrado negro con esquinas redondeadas.
- `favicon.ico`: respaldo con tamaños de 16, 32 y 48 píxeles.
- `favicon-16.png`, `favicon-32.png`, `favicon-48.png`: iconos en tamaños nativos.
- `favicon-180.png`: icono para accesos directos de Apple.

Los SVG contienen trazados vectoriales reales. No llevan fotografías incrustadas, fuentes externas, scripts ni dependencias. El texto está convertido a contornos. La vectorización conserva los contornos y la textura de las propuestas; los fondos se han eliminado y los márgenes se han recortado para facilitar su uso. Los favicons tienen menos detalle y un ajuste óptico de anchura para funcionar en pequeño.

Abre `vista-previa.html` para comparar los logos sobre fondo claro y oscuro, y revisar los iconos a su tamaño real. Funciona sin conexión.

## Integración

Copia los archivos de tu versión elegida a `/assets/kiricocho/` y añade lo siguiente dentro de `<head>`:

```html
<link rel="icon" href="/assets/kiricocho/favicon.ico" sizes="16x16 32x32 48x48">
<link rel="icon" type="image/svg+xml" href="/assets/kiricocho/favicon.svg">
<link rel="apple-touch-icon" sizes="180x180" href="/assets/kiricocho/favicon-180.png">
```

Para mostrar el logo en una cabecera con fondo oscuro:

```html
<img src="/assets/kiricocho/logo-claro.svg"
     alt="Kiricocho · Planeta Fútbol"
     style="display:block;width:260px;max-width:100%;height:auto">
```

Para fondos claros, usa `logo-negro.svg`.
