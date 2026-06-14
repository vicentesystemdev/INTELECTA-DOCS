# Control de Revisión del Informe Académico

Este documento sirve como registro oficial del estado del informe de Proyecto Integrador I y los límites de validación de los datos.

---

## 1. Metadatos del Informe

| Campo | Detalle |
|---|---|
| **Documento Fuente Original** | `INTEGRADOR_INFORME_FINAL_VICENTE.docx` |
| **Ubicación del Fuente Original** | `docs/06-evidencias/revisiones-docente/INTEGRADOR_INFORME_FINAL_VICENTE.docx` |
| **Documento Convertido** | `docs/01-informe-academico/informe-oficial-convertido.md` |
| **Ubicación del Convertido** | `docs/01-informe-academico/informe-oficial-convertido.md` |
| **Sistema** | INTELECTA |
| **Caso Oficial** | Academia Universitaria Avalancha |

---

## 2. Estado de Validación Académica

*   **Alcance Validado (Base Válida):** Todo el contenido comprendido desde la Introducción (Capítulo 1) hasta el apartado **5.2.4 SPRINT BACKLOG** (inclusive) en el Capítulo 5 se considera **Académicamente Válido y Aprobado**. Este contenido se conserva intacto en [informe-base-validado.md](file:///c:/dev/apps/INTELECTA-DOCS/docs/01-informe-academico/informe-base-validado.md).
*   **Punto de Corte:** A partir del apartado **5.3 FASE 2 – GAME** en adelante, el contenido es catalogado como **Pendiente de Reconstrucción**. Los diagramas de secuencia, colaboración, mapas de navegación y clases no representan la arquitectura real de Laravel 13/PostgreSQL del sistema actual.

---

## 3. Observaciones y Guía de Depuración

Al reconstruir el informe, se deben eliminar de forma estricta las siguientes inconsistencias:

1.  **Referencias a Casa Amandita:** Eliminar cualquier párrafo o tabla que haga alusión al Centro del Adulto Mayor "Casa Amandita", residuo de proyectos académicos anteriores.
2.  **Referencias a Colegio San Antonio de Padua:** Sustituir cualquier nombre de colegio que no esté autorizado por los datos maestros oficiales de la Academia Universitaria Avalancha.
3.  **Terminología de Docente y Estudiante:** Modificar el texto para alinear el vocabulario técnico a **"Tutor Académico"** y **"Postulante"**.
4.  **Módulos en el Capítulo 5:** Reestructurar el desarrollo técnico para describir exactamente los 12 módulos funcionales que componen el alcance actual de `INTELECTA`.
