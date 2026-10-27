# Escapa del almacén

Un escape room web sobre condiciones de seguridad en el trabajo. Estás encerrado en un almacén que incumple las normas, y para abrir el candado de la salida tienes que corregir sus riesgos antes de que se acabe el tiempo. Hecho para el ciclo de SMR.

**En vivo:** https://escapa-del-almacen.web.app

## Tecnologías

- HTML5
- CSS3 (Grid, propiedades personalizadas, media queries)
- JavaScript (sin frameworks ni dependencias)
- Web Audio API
- Firebase Hosting

## Qué tiene de particular

- **Cuatro pruebas y una extra**: riesgo eléctrico, caídas a distinto nivel, incendios y vías de evacuación, más una prueba opcional de señales de seguridad que suma tiempo.
- **Contenido con fuente**: cada dato sale del INSST o de los Reales Decretos 486/1997 (lugares de trabajo) y 485/1997 (señalización), y el repaso final cita la fuente de cada uno.
- **Sonido sin archivos**: música, efectos, fuego y sirena se generan en el navegador con Web Audio.
- **Se juega con teclado**, con atajos para todo, y respeta `prefers-reduced-motion`.
- **Adaptado a móvil**, en vertical y en horizontal.
- **Sin base de datos ni cookies**: el récord se guarda solo en el navegador de cada jugador.

## Estructura

```
firebase.json     Configuración de Firebase Hosting y cabeceras de caché
.firebaserc       A qué proyecto de Firebase se despliega
public/           Todo lo que se publica
```

## Cómo desplegarlo

```bash
firebase deploy --only hosting
```

---

Hecho por **Marcos Martínez** — desarrollador web en Valencia.
