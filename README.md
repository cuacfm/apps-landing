# CUAC FM — Landing da app

Páxina de aterraxe (*landing page*) da app móbil oficial de **CUAC FM**, a radio
comunitaria da Coruña. Presenta a aplicación e enlaza ás descargas en Google Play
e App Store.

🔗 **En produción:** <https://cuacfm.org/apps/>

## Características

- Sitio **estático** (HTML + CSS + JavaScript puro, sen *frameworks* nin *build*).
- **Multiidioma:** galego (raíz), castelán (`es/`) e portugués (`pt/`), con
  `hreflang` e `canonical` por idioma.
- Carrusel e galería de capturas animadas en JavaScript sen dependencias.
- SEO: `sitemap.xml`, `robots.txt`, Open Graph, Twitter Cards e JSON-LD.

## Estrutura

```
.
├── index.html          # galego (idioma por defecto)
├── es/index.html       # castelán
├── pt/index.html       # portugués
├── cuac_app_*.png/gif  # capturas e animacións da app
├── cuac_favicon.svg    # favicon
├── sitemap.xml
└── robots.txt
```

As versións `es/` e `pt/` comparten os recursos de imaxe da raíz mediante rutas
relativas (`../cuac_app_*`).

## Desenvolvemento

Ao ser un sitio estático, abonda con servir o directorio cun servidor local:

```bash
python3 -m http.server 8000
# abrir http://localhost:8000/
```

## Despregue

O contido publícase como sitio estático en <https://cuacfm.org/apps/>. Os recursos
externos (tipografías de Google Fonts, iconas de Lucide e o logo) cárganse desde CDN.

## A app

A app oficial de CUAC FM permite escoitar a radio comunitaria da Coruña en directo,
acceder a centos de podcasts, crear *playlists* e activar alertas de novos episodios.
Gratuíta para Android e iOS.

- [Google Play](https://play.google.com/store/apps/details?id=com.app.cuacfm.radio.coruna)
- [App Store](https://apps.apple.com/es/app/cuac-fm/id536600585)

## Licenza

© CUAC FM. Todos os dereitos reservados salvo indicación contraria.
