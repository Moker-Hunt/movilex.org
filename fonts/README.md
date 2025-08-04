# Fuentes del Sitio Web

Esta carpeta debe contener las siguientes fuentes en formato .woff2:

## Orbitron Font Family
- `Orbitron-Regular.woff2` - Peso normal (400)
- `Orbitron-Bold.woff2` - Peso bold (700)

## Descarga de Fuentes

Las fuentes Orbitron se pueden descargar desde Google Fonts:
https://fonts.google.com/specimen/Orbitron

### Pasos para descarga:
1. Visitar Google Fonts
2. Seleccionar Orbitron
3. Descargar los archivos .woff2
4. Renombrar según la estructura anterior

## Uso en CSS

Las fuentes están configuradas en `src/input.css`:

```css
@font-face {
  font-family: 'Orbitron';
  src: url('../fonts/Orbitron-Regular.woff2') format('woff2');
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: 'Orbitron';
  src: url('../fonts/Orbitron-Bold.woff2') format('woff2');
  font-weight: bold;
  font-style: normal;
}
```

## Fallback Fonts

Si las fuentes locales no cargan, el sitio usará:
- Courier New (monospace)
- Fuentes del sistema

## Optimización

- Formato .woff2 para mejor compresión
- Solo los pesos necesarios (Regular y Bold)
- Preload en HTML para mejor rendimiento 