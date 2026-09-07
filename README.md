# ALI

Landing de **ALI**, plataforma de inteligencia socioemocional para colegios y universidades.

El sitio presenta el sistema y la investigación publicada en Springer Nature (ICITS 2026): reconocimiento emocional, autorreportes y contexto para colaborar con docentes y psicólogos.

**Capítulo:** [Integrating Artificial Intelligence and Self-reports for Emotional Recognition and Management in Primary and Secondary Education](https://doi.org/10.1007/978-3-032-27538-7_66)

- ICITS 2026 · Lecture Notes in Networks and Systems, vol. 1966, cap. 66, pp. 1–10
- Fabrication Laboratory · Universidad Continental · Cusco, Perú
- DOI: [10.1007/978-3-032-27538-7_66](https://doi.org/10.1007/978-3-032-27538-7_66)

## Requisitos

- Node.js ≥ 22.12
- [Bun](https://bun.sh) (también funciona con npm)

## Arranque

```sh
bun install
bun run dev
```

El servidor queda en [http://localhost:4321](http://localhost:4321).

Si Astro indica que ya hay un proceso en ese puerto:

```sh
npx astro dev stop
bun run dev
```

| Comando | Qué hace |
| --- | --- |
| `bun install` | Instala dependencias |
| `bun run dev` | Servidor local en `localhost:4321` |
| `bun run build` | Build de producción en `./dist/` |
| `bun run preview` | Previsualiza el build |

## Stack

- [Astro](https://docs.astro.build) 7
- [Tailwind CSS](https://tailwindcss.com) 4 (`@tailwindcss/vite`)
- Tipografía: Inter Tight (Google Fonts)

La barra de desarrollo de Astro está desactivada en `astro.config.mjs`.

## Estructura

```text
/
├── public/
│   └── favicon.svg
├── src/
│   ├── assets/images/     # Fotografías de aula, campus e investigación
│   ├── components/        # Secciones de la landing
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       └── global.css     # Tokens, tipografía y utilidades
├── astro.config.mjs
└── package.json
```

La página es una sola ruta (`/`). Cada bloque de la narrativa es un componente:

| Componente | Sección |
| --- | --- |
| `Hero` | Headline y visual del aula |
| `Trust` | Cinta de respaldo (Springer, Continental, FACS) |
| `Institutions` | Colegios y universidades |
| `Problem` | Contexto público (OMS, UNICEF, MINSA, Minedu) |
| `Proposal` | Cómo colabora ALI con el equipo educativo |
| `Pipeline` | Captura → FACS → triangulación |
| `Heart` | IA, estudiante, contexto y patrón |
| `Results` | Cifras del estudio (90 estudiantes, >75% AU, 68%) |
| `Patterns` | 6.° primaria, 2.° A y 2.° B |
| `Dashboard` | Distribución emocional del reconocimiento ALI |
| `Ethics` | Datos, anonimización y trabajo con el equipo |
| `Research` | Capítulo Springer, autores y DOI |
| `Future` | Líneas de evolución |
| `Footer` | Universidad Continental y enlaces |

## Contenido

- **Contexto externo:** diagnóstico OMS (7% en 5–9 años → 14% en 10–19), 16 millones en ALC (UNICEF), 30% de NNA en riesgo en Perú (MINSA–UNICEF), 4/10 en secundaria (Minedu 2024). Esas cifras no se mezclan con los resultados de ALI.
- **Resultados del paper:** muestra efectiva de 90 estudiantes (11–15 años) en dos colegios del sur del Perú; calibración previa con ~300; >75% en Action Units; 68% de coincidencia con autorreportes.
- **Ética del protocolo:** sin videos almacenados, landmarks anonimizados, consentimiento de estudiantes, familias y docentes.

## Autores

Eduardo Ñaupa Yapura (correspondencia), Antony Elio Ayansi Huisa, Anthony Dennis Oyola Saloma, Daniel Hachircana Méndez, Yadira Melina Zapata Ttito y Diana Salas Sanchez.

## Licencia de la investigación

© 2026 The Author(s), under exclusive license to Springer Nature Switzerland AG.
