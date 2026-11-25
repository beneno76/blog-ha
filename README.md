# Domótica desde AliExpress

Blog en Hugo (tema PaperMod) con reviews de dispositivos de AliExpress para Home Assistant.

## Nueva review

```bash
hugo new content --kind review posts/nombre-del-producto/index.md
```

Las fotos van en la misma carpeta que el `index.md` (`portada.jpg`, `caja.jpg`, `placa.jpg`, `ha.png`). Conviene comprimirlas a ~1600 px de ancho antes de subirlas.

Cambia `draft: true` a `draft: false` para publicar.

## Vista previa local

```bash
git clone --recurse-submodules https://github.com/beneno76/blog-ha.git
cd blog-ha
hugo server -D
```

Abre http://localhost:1313

## Cloudflare Pages

| Campo | Valor |
|---|---|
| Framework preset | Hugo |
| Build command | `hugo --minify` |
| Build output directory | `public` |
| Variable de entorno | `HUGO_VERSION` = `0.170.1` |
