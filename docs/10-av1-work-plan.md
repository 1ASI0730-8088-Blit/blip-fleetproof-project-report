# Plan de Trabajo AV1

## Roles y aportes de AV1

La distribución final de aportes de la entrega AV1 coincide con la registrada en el [Student Outcome](01-student-outcome.md) y en el `README.md` del repositorio.

| Integrante | Rol AV1 | Responsabilidad principal | Evidencia |
|---|---|---|---|
| Reyes Limo Sebastian | Team Leader, SCM and Rubric Owner | Organizar el repositorio del informe, definir GitFlow, mantener el control de rúbrica y desarrollar el Capítulo II (análisis competitivo, entrevistas, Needfinding, Big Picture Event Storming y Ubiquitous Language). | Estructura Markdown del informe, ramas y Pull Requests integrados en `develop`, control de rúbrica, registro de evidencias y `feature/landing-subscription-plans` (PR #4) en la Landing Page. |
| Palomino Murga Daniel Stalin | Landing Page Owner | Implementar el primer feature de la Landing Page, publicarla en GitHub Pages y definir los Style Guidelines, la Information Architecture y el diseño de UI para escritorio y móvil. | `feature/landing-navigation` (PR #1), sitio desplegado en GitHub Pages y wireframes y mock-ups de escritorio y móvil. |
| Becerra Durand Sebastian Uriel | Capítulo IV Owner | Documentar el diseño UX/UI (wireframes, wireflows, mock-ups, prototipado y diagramas de flujo) y la arquitectura de software, Event Storming, diseño orientado a objetos y modelo de base de datos. | `feature/sprint1-capitulo-4` (PR #3) y `feature/landing-hero-benefits` (PR #2). |
| Gómez De La Torre Huertas Rodrigo Fernando | Capítulo V Owner | Documentar la implementación, validación y despliegue del producto y coordinar con el equipo el control de versiones en GitHub. | `feature/sprint1-capitulo-5` (PR #4) y `feature/localization-accesibility-support` (feature 5 de la Landing Page, en curso). |
| Payesa Torres Harrison Hubert | Capítulo I y III Owner | Definir y describir la startup y el producto, desarrollar el Lean UX Process y los segmentos objetivo, y elaborar las User Stories, el Impact Mapping y el Product Backlog. | `feature/sprint1-capitulos-1-3` (PR #1) y `feature/landing-product-solutions` (PR #3). |

## Por qué Reyes Limo Sebastian debe tomar Technical Lead, SCM and Rubric Owner

Reyes Limo Sebastian debe asumir el rol de Technical Lead, SCM and Rubric Owner porque tendrá apoyo directo para revisar estructura, redacción, GitFlow, releases, trazabilidad y cumplimiento de rúbrica. Ese rol no significa hacer todo el proyecto, sino asegurar que cada integrante entregue evidencia correcta y que nada quede fuera de la evaluación.

## Ramas y Pull Requests de AV1

Las ramas se crearon a partir del plan de trabajo del sprint y se integraron en `develop` mediante Pull Requests revisados.

| Rama | Pull Request | Contenido | Estado |
|---|---|---|---|
| `feature/sprint1-capitulos-1-3` | PR #1 | Capítulos I y III: Startup Profile, Solution Profile, Lean UX, User Stories, Impact Mapping y Product Backlog. | Mergeado en `develop` |
| `feature/sprint1-capitulo-2` | PR #2 | Capítulo II: análisis competitivo, entrevistas, Needfinding, Big Picture Event Storming y Ubiquitous Language. | Mergeado en `develop` |
| `feature/sprint1-capitulo-4` | PR #3 | Capítulo IV: diseño UX/UI, wireframes, wireflows, mock-ups, arquitectura de software y modelo de base de datos. | Mergeado en `develop` |
| `feature/sprint1-capitulo-5` | PR #4 | Capítulo V: implementación, validación y despliegue. | Mergeado en `develop` |
| `feature/student-outcome` | PR #5 | Student Outcome con los aportes de los integrantes. | Mergeado en `develop` |
| `feature/conclusions` | PR #6 | Conclusiones y recomendaciones de AV1. | Mergeado en `develop` |
| `feature/landing-navigation` | PR #1 (Landing Page) | Landing Page: navegación y layout base (feature 1). | Mergeado en `develop` |
| `feature/landing-hero-benefits` | PR #2 (Landing Page) | Landing Page: hero y beneficios del producto (feature 2). | Mergeado en `develop` |
| `feature/landing-product-solutions` | PR #3 (Landing Page) | Landing Page: soluciones y flujo de trabajo (feature 3). | Mergeado en `develop` |
| `feature/landing-subscription-plans` | PR #4 (Landing Page) | Landing Page: planes de suscripción (feature 4). | Mergeado en `develop` |
| `feature/localization-accesibility-support` | PR #5 (Landing Page) | Landing Page: localización ES/EN, accesibilidad, sección About us y rutas de demostración (feature 5). | Mergeado en `develop` |
| `develop` → `main` | PR #6 (Landing Page) | Integración del release `v1.0.0` de la Landing Page en `main` y despliegue en GitHub Pages. | Mergeado en `main` |

## Entregables AV1

| Entregable | Responsable | Fecha de cierre | Estado |
|---|---|---|---|
| Informe Markdown hasta Capítulo V | Reyes Limo Sebastian | 2026-09-20 | Completado |
| Capítulo I: Startup Profile, Solution Profile y Lean UX Process | Payesa Torres Harrison | 2026-09-20 | Completado |
| Capítulo II: competidores, entrevistas y Needfinding | Reyes Limo Sebastian | 2026-09-20 | Completado |
| Capítulo III: User Stories, Impact Mapping y Product Backlog | Payesa Torres Harrison | 2026-09-20 | Completado |
| Capítulo IV: Product Design (UX/UI, wireframes y mock-ups) | Becerra Durand Sebastian Uriel | 2026-09-20 | Completado |
| Capítulo V: Implementation, Validation & Deployment | Gómez De La Torre Huertas Rodrigo Fernando | 2026-09-20 | Completado |
| Landing Page v1.0.0 desplegada en GitHub Pages | Palomino Murga Daniel Stalin | 2026-09-20 | Completado |
| Keynote AV1 | Equipo | 2026-09-20 | Completado |
| Video de exposición AV1 | Equipo | 2026-09-20 | Completado |
| Participant Performance Report | Team Leader | 2026-09-20 | Completado |

## Checklist diario

- Cada integrante registra al menos un avance en su rama.
- Cada rama mantiene commits pequeños y con Conventional Commits.
- Cada sección nueva tiene evidencia o `TODO` explícito.
- Cada imagen va en `assets/images/`, `assets/diagrams/` o `assets/screenshots/`.
- Cada entrega parcial se revisa contra Programación, Redacción y GitHub.
