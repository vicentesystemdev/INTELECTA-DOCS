# Repositorio Documental INTELECTA-DOCS

Este repositorio (`INTELECTA-DOCS`) contiene de forma exclusiva la documentación académica, técnica, diagramas, prompts y evidencias del sistema **INTELECTA**, diseñado para el caso de estudio de la **Academia Universitaria Avalancha** (La Paz, Bolivia).

---

## 1. Propósito y Estructura Coherente

Para mantener un orden metodológico y evitar la mezcla de archivos binarios con código fuente, se ha separado la documentación en este repositorio independiente:
*   **Repositorio de Sistema (`INTELECTA`):** Contiene el código fuente funcional (Laravel 13 + React/Inertia + PostgreSQL).
*   **Repositorio de Documentación (`INTELECTA-DOCS`):** Contiene el informe de Proyecto Integrador I, especificaciones de diseño, diagramas de arquitectura, bitácoras de auditoría, capturas de pantalla y prompts utilizados.

---

## 2. Estado Académico del Informe

*   **Base Validada (Hasta 5.2.4):** El contenido del informe académico oficial convertido a Markdown es válido y estable hasta el apartado **5.2.4 SPRINT BACKLOG**. El documento unificado limpio se localiza en:
    *   [`docs/01-informe-academico/informe-base-validado.md`](file:///c:/dev/apps/INTELECTA-DOCS/docs/01-informe-academico/informe-base-validado.md)
*   **Pendiente de Reconstrucción (Desde 5.3):** A partir del apartado **5.3 FASE 2 – GAME** en adelante (incluyendo diagramas de secuencia, casos de uso, diagrama físico de base de datos y mapa de navegación), el informe antiguo presenta inconsistencias y debe ser reescrito según el sistema actual. El checklist detallado se encuentra en:
    *   [`docs/01-informe-academico/pendiente-reconstruccion-desde-5-3.md`](file:///c:/dev/apps/INTELECTA-DOCS/docs/01-informe-academico/pendiente-reconstruccion-desde-5-3.md)

---

## 3. Mapa de Navegación de Carpetas

*   [`docs/00-contexto/`](file:///c:/dev/apps/INTELECTA-DOCS/docs/00-contexto/): Ficha del proyecto, alcance del sistema y decisiones documentales.
*   [`docs/01-informe-academico/`](file:///c:/dev/apps/INTELECTA-DOCS/docs/01-informe-academico/): Capítulos del informe oficial en Markdown, control de revisión y base validada.
*   [`docs/02-documentacion-tecnica/`](file:///c:/dev/apps/INTELECTA-DOCS/docs/02-documentacion-tecnica/): Arquitectura de software, modelo de base de datos relacional y especificaciones de módulos.
*   [`docs/03-diagramas/`](file:///c:/dev/apps/INTELECTA-DOCS/docs/03-diagramas/): Archivos editables (`.drawio`, `.puml`) y exportados de los diagramas del sistema.
*   [`docs/04-prompts/`](file:///c:/dev/apps/INTELECTA-DOCS/docs/04-prompts/): Prompts estructurados de desarrollo, auditorías y preparación para la defensa académica.
*   [`docs/05-auditorias/`](file:///c:/dev/apps/INTELECTA-DOCS/docs/05-auditorias/): Reportes de auditoría de interfaz, backend y base de datos (incluyendo la v1 y v2).
*   [`docs/06-evidencias/`](file:///c:/dev/apps/INTELECTA-DOCS/docs/06-evidencias/): Capturas del sistema en ejecución, el archivo Word original (`.docx`) y evidencias de commits.
*   [`plantillas/`](file:///c:/dev/apps/INTELECTA-DOCS/plantillas/): Plantillas Markdown reutilizables para historias de usuario, casos de uso y bitácoras.

---

## 4. Políticas de Versionamiento y Git

### 4.1 Archivos que NO deben subirse (Exclusiones)
*   **Código fuente del sistema:** (No subir `.php`, `.jsx`, `.js`, `.css` del proyecto).
*   **Archivos temporales de Office:** Archivos ocultos de bloqueo del tipo `~$*.docx`.
*   **Carpetas de dependencias:** Carpetas como `node_modules` o `vendor`.
*   **Archivos ZIP/RAR de respaldo:** Descomprimir siempre los archivos antes de comitear. No se permite subir el ZIP completo del informe.

### 4.2 Flujo de Trabajo con Ramas (Ramas Sugeridas)
Para mantener la rama `main` en un estado de entrega académica pulida, se sugiere el siguiente esquema de ramas:
1.  `docs/informe-validado`: Ajustes de ortografía y formato en las secciones aprobadas (capítulos 1 a 4).
2.  `docs/reconstruccion-5-3`: Edición de diagramas y apartados técnicos del Capítulo 5 a partir de la fase Game.
3.  `docs/diagramas`: Elaboración de archivos `.drawio` y exportaciones PNG de la arquitectura y base de datos.
4.  `docs/auditorias`: Incorporación de nuevas auditorías de calidad de software.

**Flujo recomendado:**
*   Crear la rama correspondiente (`git checkout -b docs/mi-rama`).
*   Realizar cambios documentales y comitear con mensajes descriptivos (siguiendo convenciones de commits convencionales, ej: `docs: agregar caso de uso de matriculacion`).
*   Subir la rama a GitHub y abrir un **Pull Request** hacia `main` para su revisión académica antes de la fusión final.
