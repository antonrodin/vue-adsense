# Componente Adsense para Vue.js

Componente básico para insertar anuncios adsense dentro de una app
que utilice Vue.js. Primero añade esto dentro de tu index.html, entre las etiquetas __<head>__ o al final de __<body>__, pero fuera de tu #app...

```html
    <script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
```

Asi mismo para utilizar el componente solo tendrias que registrarlo y poner esto donde quieras mostrar tu anuncio:

```html
<adsense 
    ad-slot="XXXXXXX" 
    ad-format="auto"
    ad-client="ca-pub-XXXXXXXXXX"
    ad-style="display:block"></adsense>
```

Las variables dependen del bloque de anuncios en cuestión, dependiendo de que anuncios uses, es posible que sea suficiente con poner solo esto:

```html
<adsense ad-slot="XXXXXXXX"></adsense>
```

Ya que por regla general el cliente, el formato de anuncio (responsive) o estilo suele ser el mismo en todos tus anuncios...