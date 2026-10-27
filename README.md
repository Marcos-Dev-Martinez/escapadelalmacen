# Escapa del almacén

Escape room web sobre **condiciones de seguridad en el trabajo** (Actividad 2 · U2 · SMR).
Se juega en el navegador, de forma individual; la profesora cuelga el enlace en Aules.

- 4 pruebas: cuadro eléctrico, altillo, papelera ardiendo y pasillo bloqueado (código del candado: 5941).
- Prueba extra opcional de señales de seguridad (+5 s por acierto).
- 4 minutos, −10 s por fallo, estrellas y récord al final.
- Fuentes: INSST (riesgo eléctrico, incendios), RD 486/1997 (lugares de trabajo) y RD 485/1997 (señalización).

## Publicar

```
firebase login
firebase deploy --only hosting
```

Dirección: https://escapa-del-almacen.web.app

Si el ID del proyecto en Firebase no es `escapa-del-almacen`, cámbialo en `.firebaserc`
y en las etiquetas `og:url` y `og:image` de `public/index.html`.
