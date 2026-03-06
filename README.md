# Landing

Sources of https://gridnev.tech/ website.

## CSS

Styles are compiled from `input.css` using the [Tailwind standalone CLI](https://github.com/tailwindlabs/tailwindcss/releases). The binary is not committed — download it once:

```bash
curl -sL https://github.com/tailwindlabs/tailwindcss/releases/download/v4.0.9/tailwindcss-macos-arm64 -o tailwindcss && chmod +x tailwindcss
```

After changing classes in `index.html`, rebuild `style.css`:

```bash
./tailwindcss -i input.css -o style.css --minify
```

Commit the updated `style.css` alongside your HTML changes — no build step on the server needed.
