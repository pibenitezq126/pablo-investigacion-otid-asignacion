# Bitácora de Proceso — Asignación #1: Calculadora con IA
**Observatorio OTID · FICCT · Grupo IA Aplicada**
**Autor:** Pablo Benitez Quispe
**Propósito:** Documentar el flujo de trabajo completo de desarrollo asistido por IA, desde la generación de código hasta el despliegue, para consulta y replicación en futuros proyectos del observatorio.

---

## Índice

- [Revisión 1 — Calculadora básica](#revisión-1--calculadora-básica)
- [Revisión 2 — Flujo profesional completo](#revisión-2--flujo-profesional-completo)
- [Decisiones técnicas y justificación](#decisiones-técnicas-y-justificación)
- [Pendientes](#pendientes)
- [Glosario rápido](#glosario-rápido)

---

## Revisión 1 — Calculadora básica

**Objetivo de la consigna:** programar una calculadora básica en el lenguaje de preferencia y mostrar las herramientas usadas.

**Estado:** ✅ Completado

**Resumen:**
- Se generó una calculadora funcional (operaciones básicas + raíz cuadrada, manejo de error en división entre cero).
- Se evaluaron herramientas candidatas antes de decidir el entorno final.

**Herramientas evaluadas:**

| Herramienta | Tipo | Pros | Contras | Resultado |
|---|---|---|---|---|
| Claude (Artifacts/Skills) | Chat → genera código directo | Sin instalación, resultado inmediato, ideal si hay internet inestable solo en el momento puntual | Necesita internet para generar | Usado para prototipo inicial |
| Cursor | Editor con IA integrada | Funciona con conexión intermitente, control total del código | Requiere instalación previa | Evaluado, no usado finalmente |
| Ollama + modelo local (Llama3, Gemma, Kimi K2) | IA 100% local | Cero dependencia de internet | Configuración más compleja, latencia en hardware sin GPU, no coincide con el objetivo exacto de la consigna (la IA pasaría a ser parte de la app, no el asistente de desarrollo) | Descartado para esta tarea, posible para investigación futura |
| Google Antigravity | Entorno de desarrollo con agentes de IA | — *(en evaluación, ver Revisión 2)* | — | **Seleccionado** |

---

## Revisión 2 — Flujo profesional completo

**Objetivo de la consigna:** mostrar el entorno de trabajo completo — flujo de código, control de versiones, despliegue (tienda o web), ubicación del código, manejo de cambios solicitados por el cliente (decano), documentación, y corrección de errores generados por la IA.

**Estado:** 🔄 En progreso

### Entorno seleccionado

**Google Antigravity** — entorno de desarrollo agentic de Google, ejecutado localmente en laptop.

Documentación de referencia:
- [Codelab oficial de inicio](https://codelabs.developers.google.com/getting-started-google-antigravity?hl=es-419#0)
- [Documentación oficial](https://antigravity.google/docs/home)

### Justificación de "usar lo que ya tenemos antes de pagar"

La facultad FICCT otorga correo institucional, lo cual habilita:

1. **GitHub Student Developer Pack** — acceso gratuito a herramientas profesionales (Copilot, dominios, hosting, etc.) usando el correo institucional.
2. **Google AI Pro** — suscripción anual otorgada (verificar condiciones exactas de la promoción).
3. **Alternativa 100% local** — Ollama con modelos ligeros (Gemma, Kimi K2) como respaldo sin dependencia de servicios externos.

### Infraestructura ya preparada

- [x] Cuenta de GitHub creada
- [x] Repositorio creado
- [x] Google Antigravity instalado y probado
- [ ] Cuenta ORCID *(pendiente)*
- [ ] Cuenta Google Scholar / Google Académico *(pendiente)*

> **Nota sobre ORCID y Google Scholar:** estas no son herramientas de desarrollo — son identificadores de investigador académico. Tiene sentido crearlas en el contexto del observatorio porque cualquier publicación o paper que produzca el grupo de investigación necesitará un ORCID para ser indexado correctamente, y Google Scholar para visibilidad académica. No están directamente atadas al código de la calculadora, sino al perfil investigador de Pablo dentro de OTID.

### Flujo de trabajo a documentar (siguiente paso)

Pendiente de definir en detalle con el código real, pero la consigna pide cubrir:

- [ ] Flujo del código (cómo se genera, revisa, e integra)
- [ ] Control de revisiones con el cliente (Git + GitHub, ramas, commits, pull requests)
- [ ] Proceso de despliegue (¿tienda de apps? ¿página web? — definir según el tipo de calculadora)
- [ ] Ubicación del código (repo público o privado en GitHub)
- [ ] Cómo manejar cambios solicitados por el cliente (flujo de issue → branch → cambio → revisión → merge)
- [ ] Documentación del proyecto (README, comentarios en código)
- [ ] Corrección de errores generados por la IA (proceso de debugging asistido)

---

## Decisiones técnicas y justificación

*(Esta sección se actualiza en cada revisión con el razonamiento detrás de cada decisión clave)*

### ¿Por qué no Ollama para esta tarea puntual?

Aunque es la opción más robusta ante fallas de internet, usar un modelo local cambia el rol de la IA: en vez de ser el *asistente que ayuda a programar*, se vuelve *un componente de la aplicación*. La consigna original pedía mostrar el proceso de generación de código asistido por IA, no construir una app que consume un modelo de IA. Se mantiene como alternativa de respaldo o para un proyecto de investigación futuro del observatorio.

### ¿Por qué Google Antigravity?

*(Pablo: completar con tu razonamiento aquí — qué viste en la documentación que te convenció, qué tal la primera prueba)*

---

## Pendientes

- [ ] Definir y documentar el flujo completo de Git/GitHub (ramas, commits, pull requests)
- [ ] Decidir tipo de despliegue (web estática, ejecutable de escritorio, tienda de apps)
- [ ] Crear cuenta ORCID
- [ ] Crear perfil de Google Scholar
- [ ] Probar el flujo de "cliente pide cambio" de punta a punta al menos una vez antes de la presentación
- [ ] Documentar errores reales encontrados durante el desarrollo y cómo se corrigieron

---

## Glosario rápido

*(Para consulta rápida propia o de quien replique este proceso)*

- **GitHub Student Pack:** paquete gratuito de herramientas de desarrollo para estudiantes verificados con correo institucional.
- **ORCID:** identificador único internacional para investigadores académicos, usado para vincular publicaciones a una persona de forma inequívoca.
- **Google Scholar (Google Académico):** buscador e indexador de literatura académica; un perfil propio agrega visibilidad a las publicaciones de un investigador.
- **Antigravity:** entorno de desarrollo de Google con agentes de IA integrados para asistencia en programación.
- **Pull Request (PR):** solicitud para fusionar cambios de una rama de código a otra, usada como punto de revisión antes de integrar cambios.

---

*Última actualización: 28 de junio de 2026 — Revisión 2 en progreso*
