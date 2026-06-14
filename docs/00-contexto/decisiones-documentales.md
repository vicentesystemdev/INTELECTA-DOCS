# Decisiones de Arquitectura Documental

Para garantizar la consistencia académica, claridad del proyecto y coherencia metodológica, se han tomado las siguientes decisiones respecto al repositorio de documentación:

---

## 1. Separación de Código y Documentación

*   **Decisión:** Crear el repositorio `INTELECTA-DOCS` de forma independiente a la base de código funcional de `INTELECTA`.
*   **Motivo:** Evitar la saturación del repositorio de software con binarios pesados (como archivos `.docx` de informes) y permitir que el versionamiento documental avance de forma separada del flujo de desarrollo ágil y despliegue del código.

---

## 2. Definición del Punto de Corte Metodológico

*   **Decisión:** Establecer el apartado **5.2.4 SPRINT BACKLOG** como el límite de contenido validado y aprobado en el informe de Proyecto Integrador.
*   **Motivo:** La estructura y diagramas posteriores en el informe Word original (`INTEGRADOR_INFORME_FINAL_VICENTE.docx`) contienen inconsistencias de terminología, diagramas de bases de datos heredados y módulos antiguos que no corresponden a la base de datos real en PostgreSQL y al framework Laravel 13.
*   **Acción:** Se genera el archivo `informe-base-validado.md` cortando el reporte convertido exactamente en la sección 5.2.4. Todo el material posterior se clasifica en el archivo de pendientes para su reconstrucción controlada.

---

## 3. Normalización Terminológica y Académica

Se establece una regla de depuración obligatoria para reemplazar términos incorrectos del informe antiguo:

1.  **Rol Educativo:** Sustituir "Docente" por **"Tutor Académico"**, tanto en vistas, documentación y roles, a menos que existan identificadores técnicos legados en bases de datos que requieran migración controlada.
2.  **Rol Discente:** Sustituir "Estudiante" por **"Postulante"**, en concordancia con el caso institucional de nivelación preuniversitaria.
3.  **Casos e Instituciones Ajenas:** Eliminar cualquier mención heredada a "Centro del Adulto Mayor Casa Amandita", "Colegio San Antonio de Padua" o "Retos/Gamificación". El único caso de estudio oficial es la **Academia Universitaria Avalancha** de La Paz, Bolivia.
4.  **Módulos del Sistema:** Centrar la documentación técnica del Capítulo 5 exclusivamente en los 12 módulos de software reales de INTELECTA.

---

## 4. Control de Versiones Documental

*   **Esquema de Ramas:** Se promueve el uso de ramas Git para el informe (`docs/informe-validado`), los diagramas (`docs/diagramas`), y la reconstrucción de secciones (`docs/reconstruccion-5-3`), aplicando Pull Requests para integrar cambios a la rama principal `main`.
*   **Exclusiones en .gitignore:** Se bloquea la subida de archivos temporales de Office y archivos del sistema, permitiendo únicamente formatos legibles por texto plano (Markdown), binarios de diagramas (`.drawio`), imágenes y hojas de cálculo complementarias.
