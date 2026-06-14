# Estructura del Repositorio INTELECTA-DOCS

Este documento describe detalladamente la organización y el propósito de cada una de las carpetas de este repositorio.

---

```
INTELECTA-DOCS/
├── README.md                           # Presentación general y guía de flujo de trabajo
├── ESTRUCTURA.md                       # Detalle de la estructura física de carpetas (este archivo)
├── CHANGELOG.md                        # Registro cronológico de versiones de la documentación
├── .gitignore                          # Exclusiones de Git para asegurar un repositorio puramente documental
│
├── docs/                               # Contenido principal de la documentación
│   ├── 00-contexto/                    # Datos administrativos y alcance oficial del proyecto
│   │   ├── ficha-proyecto.md           # Títulos, autores, tutores y stack técnico
│   │   ├── alcance-oficial.md          # Módulos reales del sistema e hitos
│   │   └── decisiones-documentales.md  # Justificación de las metodologías aplicadas
│   │
│   ├── 01-informe-academico/           # Informe de Proyecto Integrador en Markdown
│   │   ├── 00-control-revision.md      # Registro de cambios aplicados al informe
│   │   ├── informe-oficial-convertido.md # Conversión completa del Word original
│   │   ├── informe-base-validado.md    # Texto aprobado y validado (hasta 5.2.4)
│   │   ├── pendiente-reconstruccion-desde-5-3.md # Checklist de tareas para las secciones siguientes
│   │   ├── capitulo-1-introduccion/    # Subcarpeta para descomponer el Cap. 1
│   │   ├── capitulo-2-justificacion/   # Subcarpeta para descomponer el Cap. 2
│   │   ├── capitulo-3-diseno-teorico/  # Subcarpeta para descomponer el Cap. 3
│   │   ├── capitulo-4-dispositivo-prueba/ # Subcarpeta para el dispositivo de prueba
│   │   ├── capitulo-5-desarrollo/      # Subcarpeta para el desarrollo ágil Scrum
│   │   ├── conclusiones-recomendaciones/ # Borradores de conclusiones y recomendaciones
│   │   ├── glosario/                   # Glosario de términos académicos y técnicos
│   │   ├── bibliografia/               # Referencias bibliográficas (normas APA 7)
│   │   └── anexos/                     # Encuestas, cronogramas y cartas de aceptación
│   │
│   ├── 02-documentacion-tecnica/       # Documentación específica del software
│   │   ├── arquitectura/               # Detalles de arquitectura limpia por dominios
│   │   ├── base-datos/                 # Diccionario de datos y relaciones de PostgreSQL
│   │   ├── modulos/                    # Especificación detallada de los 12 módulos funcionales
│   │   ├── roles-permisos/             # Diseño del esquema de control de acceso de Spatie
│   │   ├── pruebas/                    # Estrategias de testing y reporte de PHPUnit
│   │   └── despliegue/                 # Manual de instalación y configuración de servidores
│   │
│   ├── 03-diagramas/                   # Modelado del sistema y diagramas UML
│   │   ├── drawio/                     # Archivos de diagramación editables de Draw.io
│   │   ├── plantuml/                   # Archivos fuente basados en código PlantUML
│   │   ├── imagenes-exportadas/        # Exportaciones finales (PNG/SVG) para el informe
│   │   └── fuentes/                    # Archivos fuente adicionales
│   │
│   ├── 04-prompts/                     # Prompts utilizados para interactuar con la IA
│   │   ├── desarrollo/                 # Prompts de desarrollo de controladores y lógica
│   │   ├── documentacion/              # Prompts para redactar o formatear textos
│   │   ├── diagramas/                  # Prompts para modelado o diagramación
│   │   ├── auditorias/                 # Prompts para testing y seguridad
│   │   └── defensa/                    # Prompts de preparación para preguntas de la defensa
│   │
│   ├── 05-auditorias/                  # Revisiones e informes de calidad de software
│   │   ├── ui/                         # Informes de auditoría de interfaz y diseño responsive
│   │   ├── backend/                    # Informes de rendimiento y lógica
│   │   ├── base-datos/                 # Evaluaciones de índices, llaves y normalización 3FN
│   │   └── documentacion/              # Informes de auditoría documental (ej: v1 y v2)
│   │
│   ├── 06-evidencias/                  # Certificaciones de pruebas y trabajo realizado
│   │   ├── capturas/                   # Pantallazos de interfaces reales funcionando
│   │   ├── media-informe/              # Imágenes oficiales extraídas del informe original
│   │   ├── pruebas/                    # Logs y reportes de ejecución de PHPUnit
│   │   ├── revisiones-docente/         # Documento Word original (.docx) y feedback escrito
│   │   └── commits/                    # Registro histórico de entregas de código
│   │
│   └── 99-archivo/                     # Borradores desestimados o documentación histórica
│
├── plantillas/                         # Archivos base de formato para agilizar documentación
│   ├── plantilla-caso-uso.md
│   ├── plantilla-historia-usuario.md
│   ├── plantilla-auditoria.md
│   ├── plantilla-bitacora.md
│   ├── plantilla-prompt.md
│   ├── plantilla-observaciones-docente.md
│   └── plantilla-control-revision.md
│
└── recursos/                           # Herramientas de soporte
    ├── guia-documentacion/             # Directrices de redacción científica y académica
    └── ejemplos/                       # Ejemplos prácticos de redacción y modelado
```
