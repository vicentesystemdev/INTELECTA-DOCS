# Alcance Oficial del Proyecto INTELECTA

El sistema INTELECTA está diseñado para dar soporte a la gestión académica y toma de decisiones en la Academia Universitaria Avalancha. El alcance de la implementación se divide en módulos funcionales clasificados en componentes actuales, referenciales y futuros.

---

## 1. Módulos Funcionales del Sistema

### 1.1 Seguridad, Usuarios y Dashboard
*   **Autenticación y Sesión:** Autenticación perimetral protegida.
*   **Dashboard Institucional:** Consolidación de métricas de catálogos, postulantes y estado curricular.
*   **Middleware Perimetral:** `EnsureAdministrativeAccess` restringe el acceso a módulos administrativos y retorna respuestas 403 para peticiones directas de usuarios sin privilegios.

### 1.2 Gestión Institucional
*   **Programas Académicos:** Registro de programas de nivelación, fechas de inicio y fin.
*   **Grupos y Paralelos:** Organización de postulantes en aulas virtuales o paralelos.
*   **Tutores Académicos:** Registro de tutores asignados a coordinaciones.
*   **Asignación de Tutores:** Vinculación de un tutor responsable a un determinado grupo y programa.

### 1.3 Gestión de Postulantes
*   **Postulantes:** CRUD e historial de postulantes matriculados en la academia.
*   **Ficha Académica:** Módulo con vista React dedicada (`/admin/institucional/ficha-academica`) que actúa como expediente unificado con búsqueda, paginación e información de rendimiento del postulante.
*   **Habilitación Académica:** Control de permisos de acceso del estudiante a evaluaciones en base a su matrícula y estado de cuotas.

### 1.4 Gestión Evaluativa y Banco de Preguntas
*   **Materias, Áreas y Temas:** Estructura jerárquica curricular (Materia -> Área -> Tema) con persistencia obligatoria de la materia en las áreas de conocimiento.
*   **Banco de Preguntas:** Taxonomía de preguntas, niveles de dificultad, tipos de ítem (opción múltiple) y almacenamiento de respuestas correctas.
*   **Plantillas de Evaluación:** Composición y ponderación de reactivos (total 100 puntos) para simulacros.
*   **Simulacros Programados:** Calendario y horas para exámenes preuniversitarios.

### 1.5 Reportes e Indicadores
*   **Reportes Académicos:** Cobertura de materias y estadísticas descriptivas de matriculados.
*   **Indicadores de Desempeño:** Identificación de alertas de riesgo académico según rendimiento.

---

## 2. Límites del Alcance (Fases Referenciales y Futuras)

Para fines de la defensa y la claridad metodológica del proyecto:

*   **Resultados Académicos (Referencial):** La pantalla de resultados de simulacros es de lectura y carácter de prototipo referencial en esta fase. No cuenta con flujo transaccional directo de respuestas de postulantes.
*   **Learning Analytics (Conceptual / Propuesta):** El módulo visual se presenta como una propuesta arquitectónica y un panel referencial, sin modelos predictivos ni de Machine Learning (TRI, regresión logística, Random Forest) entrenados de manera activa.
*   **Evaluaciones Operativas en Vivo (Futuro):** La persistencia de respuestas reactivas en tiempo real y el motor de exámenes en el portal del postulante corresponden a la siguiente fase del Proyecto Integrador.
