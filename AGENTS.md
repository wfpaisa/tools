# AGENTS.md

Reglas para cualquier agente que trabaje en este repositorio.

## Cómo debe ser el contenido

- **Todo es estático.** HTML, CSS y JavaScript vanilla. Sin frameworks ni SSR.
  - El JS va embebido en el HTML o en archivos `.js` sueltos; sin bundlers.
  - El CSS compartido vive en `/styles/` y se importa con `<link rel="stylesheet">`.
- **Sin build, sin dependencias, sin compilación.** El sitio debe abrirse
  directamente abriendo el `index.html` en el navegador o sirviendo los
  archivos como están.
- **Excepción — pre-builds:** solo se usan si el usuario lo pide de forma
  explícita. Si no hay una solicitud clara en ese sentido, no agregues pasos de
  build, ni `npm install`, ni transpilación, ni nada que requiera Node para
  ver el resultado.

## Público y privacidad

- Este repositorio se publica en un **GitHub público**.
- **No incluyas información personal delicada** en ningún archivo que se
  commitee:
  - Nombres propios, correos, teléfonos, direcciones, cédulas, cuentas
    bancarias, saldos reales de créditos, fechas personales, etc.
  - Los valores numéricos de ejemplo deben ser genéricos, no datos reales.
- Antes de commitear, revisa que el diff no contenga nada sensible.
