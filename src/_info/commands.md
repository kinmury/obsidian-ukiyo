# `${VAULT_PATH}\themes\obsidian-ukiyo>`

## DEV

```bash
sass --no-source-map --watch "./src/main.scss" "../dev.css"
csso ../dev.css --output ../theme.css
```

## PROD

```bash
sass --no-source-map "./src/main.scss" "./prod.css"
csso ./prod.css --output ./theme.css
DEL ./prod.css
```