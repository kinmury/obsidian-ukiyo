# Useful Comands

> [!warning] 
> The following syntax needs to be followed in order to not crash the compilation/compression but still keeping the SS-settings

```scss
/*!
/* @settings
*/
```

## src/

```bash
sass --no-source-map --watch --style compressed "./src/main.scss" "./testbench/.obsidian/themes/clean.css"

sass --no-source-map --style compressed "./src/main.scss" "./clean.css"
```
