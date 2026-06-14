# Pendiente de Reconstrucción Desde Sección 5.3

Este archivo detalla las tareas, checklists, actores y módulos reales que deben guiar la reconstrucción académica del informe a partir del apartado **5.3 FASE 2 – GAME**.

---

## 1. Checklist de Secciones Pendientes

- [ ] **Rehacer 5.3 FASE 2 – GAME:** Estructurar el análisis de diseño en base a la metodología Scrum y las fases de desarrollo reales.
- [ ] **Rehacer Diagrama de Paquetes:** Definir los paquetes lógicos del backend (Laravel por dominios) y frontend (React/Inertia por páginas y componentes).
- [ ] **Rehacer Diagramas de Casos de Uso:** Diseñar los diagramas enfocados en los actores de la Academia Universitaria Avalancha.
- [ ] **Rehacer Especificaciones de Casos de Uso:** Completar las fichas descriptivas de los casos de uso críticos.
- [ ] **Rehacer Diagramas de Secuencia:** Diagramar flujos transaccionales reales (como la creación de plantillas de examen o la asignación de tutorías).
- [ ] **Rehacer Diagramas de Colaboración / Comunicación:** Reflejar la interacción de objetos y controladores en Laravel.
- [ ] **Rehacer Diagrama de Clases de Alto Nivel:** Representar la arquitectura conceptual del sistema.
- [ ] **Rehacer Diagrama de Clases de Bajo Nivel:** Modelar las clases y controladores reales del backend.
- [ ] **Rehacer Diagrama Físico de Base de Datos:** Reflejar fielmente la base de datos relacional de PostgreSQL con sus 30+ tablas normalizadas.
- [ ] **Rehacer Mapa Navegacional:** Mapear la navegación real basada en rutas de Inertia.js y el sidebar jerárquico.
- [ ] **Redactar Arquitectura de Software:** Describir la arquitectura limpia y modular implementada en INTELECTA.
- [ ] **Redactar Conclusiones:** Conclusiones enfocadas en la viabilidad del prototipo para la Academia Universitaria Avalancha.
- [ ] **Redactar Recomendaciones:** Recomendaciones técnicas y metodológicas para el Proyecto Integrador II.
- [ ] **Corregir Glosario:** Normalizar términos técnicos.
- [ ] **Verificar Bibliografía:** Asegurar que las referencias cumplan estrictamente con las normas APA 7.
- [ ] **Rehacer Anexos:** Alinear cronogramas y encuestas de análisis a la Academia Universitaria Avalancha.

---

## 2. Definición de Actores Académicos

### 2.1 Actores Válidos y Oficiales
*   **Super Administrador:** Acceso implícito total en el sistema.
*   **Administrador:** Coordinador académico encargado de planificar programas, grupos y asignaciones.
*   **Dirección:** Rol de visualización de reportes e indicadores estratégicos.
*   **Secretaría:** Gestión operativa y cobro de matrículas/cuotas.
*   **Tutor Académico:** Perfil profesional encargado de la docencia y retroalimentación de postulantes.
*   **Postulante:** Usuario preuniversitario en proceso de nivelación.
*   **Sistema:** Automatizaciones en segundo plano (Redis, colas, cálculo automático de habilitaciones).

### 2.2 Términos y Actores Prohibidos (No utilizar)
*   *Docente* (Sustituir por **Tutor Académico**)
*   *Estudiante* (Sustituir por **Postulante**)
*   *Retos* (Módulo desestimado de gamificación)
*   *Casa Amandita* (Caso de estudio ajeno)
*   *Colegio San Antonio de Padua* (Nombre no oficial en seeders)

---

## 3. Módulos Reales a Considerar en la Reconstrucción

1.  **Seguridad, usuarios y dashboard** (Acceso perimetral y métricas base)
2.  **Gestión institucional** (Programas, grupos y paralelos)
3.  **Gestión de postulantes** (Registro de aspirantes y expediente de ficha académica)
4.  **Gestión evaluativa** (Materias, áreas de conocimiento y temas curriculares)
5.  **Banco de preguntas** (Taxonomía, dificultades y respuestas correctas)
6.  **Plantillas de evaluación** (Estructura de simulacros ponderados a 100 pts)
7.  **Aplicación de evaluaciones** (Fase futura de toma de exámenes)
8.  **Resultados académicos** (Vista referencial del rendimiento de simulacros)
9.  **Reportes académicos** (Estadísticas descriptivas de cobertura de materias)
10. **Indicadores de desempeño** (Alertas de riesgo académico)
11. **Learning Analytics** (Propuesta conceptual de apoyo curricular)
12. **Roles y permisos** (Spatie Permission con control de acceso)
