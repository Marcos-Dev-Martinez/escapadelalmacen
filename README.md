# Escapa del almacén

Dos escape rooms web sobre condiciones de seguridad en el trabajo: un almacén y un taller de informática que incumplen las normas. En cada sala, para abrir el candado de la salida tienes que corregir sus riesgos antes de que se acabe el tiempo. Hecho para el ciclo de SMR.

**En vivo:** https://escapa-del-almacen.web.app

## Tecnologías

- HTML5
- CSS3 (Grid, propiedades personalizadas, media queries)
- JavaScript (sin frameworks ni dependencias)
- Web Audio API
- Firebase Hosting

## Qué tiene de particular

- **Dos salas, cuatro pruebas y una extra en cada una**:
  - *Escapa del almacén*: riesgo eléctrico, caídas a distinto nivel, incendios y vías de evacuación, más una prueba opcional de señales de seguridad.
  - *Escapa del taller de informática*: extintores, condiciones ambientales, almacenaje y orden, más una prueba opcional del botiquín.
- **El código del candado cambia en cada partida**.
- **Contenido con fuente**: cada dato sale del INSST, de los Reales Decretos 486/1997 (lugares de trabajo) y 485/1997 (señalización) o, en los extintores, del Servicio de Prevención de la Universidad de Huelva, y el repaso final cita la fuente de cada uno.
- **Sonido sin archivos**: música, efectos, fuego y sirena se generan en el navegador con Web Audio.
- **Accesible (WCAG 2.1 AA)**: se juega entero con teclado, con atajos para todo; contraste AA comprobado en ordenador y móvil; las salas tienen descripción para lectores de pantalla, y respeta `prefers-reduced-motion`.
- **Adaptado a móvil**, en vertical y en horizontal.
- **Sin base de datos ni cookies**: el récord se guarda solo en el navegador de cada jugador.
- **Sin peticiones a terceros**: las tipografías (Oswald y Barlow, licencia OFL) se sirven desde la propia web, no desde Google Fonts.
- **Aviso legal y privacidad** propios, y página 404.

## Estructura

```
firebase.json     Configuración de Firebase Hosting y cabeceras de caché
.firebaserc       A qué proyecto de Firebase se despliega
public/           Todo lo que se publica
├── index.html    El juego entero (HTML, CSS y JavaScript)
├── aviso-legal.html, privacidad.html, 404.html
└── fonts/        Oswald y Barlow en woff2, con sus licencias
```

## Cómo desplegarlo

```bash
firebase deploy --only hosting
```

---

Hecho por **Marcos Martínez** — desarrollador web en Valencia.
