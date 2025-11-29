# Estructura del Repositorio - Física Moderna

Este documento describe la organización completa del repositorio.

## 📁 Estructura General

```
fisica-moderna/
├── README.md                      # Descripción general del proyecto
├── ESTRUCTURA.md                  # Este archivo
├── index.md                       # Página principal del sitio Jekyll
├── _config.yml                    # Configuración de Jekyll
├── Gemfile                        # Dependencias Ruby
├── .gitignore                     # Archivos ignorados por Git
│
├── _includes/                     # Componentes personalizados Jekyll
│   └── head_custom.html          # Configuración MathJax
│
├── programa/                      # 📘 Planeación Académica
│   ├── README.md
│   ├── syllabus.md               # Plan completo del curso
│   └── cronograma-detallado.md   # [PENDIENTE] Planificación sesión por sesión
│
├── docs/                          # 📚 Contenido del Sitio Web (Unidades)
│   ├── unidad-0/                 # U0: Introducción y Diagnóstico
│   │   ├── index.md              ✅ Completo
│   │   ├── sesiones/             # Material específico por sesión
│   │   └── evaluacion/           # Instrumentos de evaluación de la unidad
│   │
│   ├── unidad-1/                 # U1: Fundamentos de Teoría Cuántica
│   │   ├── index.md              ✅ Completo
│   │   ├── sesiones/
│   │   └── evaluacion/
│   │
│   ├── unidad-2/                 # U2: Dualidad Onda-Partícula
│   │   ├── index.md              ⚠️ Esqueleto
│   │   ├── sesiones/
│   │   └── evaluacion/
│   │
│   ├── unidad-3/                 # U3: Ecuación de Schrödinger
│   │   ├── index.md              ⚠️ Esqueleto
│   │   ├── sesiones/
│   │   └── evaluacion/
│   │
│   ├── unidad-4/                 # U4: Átomos y Estructura
│   │   ├── index.md              ⚠️ Esqueleto
│   │   ├── sesiones/
│   │   └── evaluacion/
│   │
│   └── unidad-5/                 # U5: Introducción al Estado Sólido
│       ├── index.md              ⚠️ Esqueleto
│       ├── sesiones/
│       └── evaluacion/
│
├── recursos-didacticos/          # 📊 Materiales Didácticos
│   ├── README.md
│   ├── presentaciones/           # PPTs organizadas por unidad/sesión
│   ├── apuntes/                  # Material teórico complementario
│   ├── ejercicios/               # Problemas propuestos y resueltos
│   └── manuales/                 # Documentos formales (manuales de asignatura)
│
├── simulaciones/                  # 🔬 Simulaciones Interactivas
│   ├── README.md
│   ├── guias/                    # Guías paso a paso por simulación
│   └── recursos/                 # Enlaces, capturas, materiales de apoyo
│
├── evaluacion/                    # 📝 Instrumentos de Evaluación
│   ├── README.md
│   ├── rubricas/                 # Rúbricas por tipo de actividad
│   ├── examenes/                 # Banco de preguntas y exámenes
│   └── proyectos/                # Guías de proyecto integrador
│
└── herramientas-ia/              # 🤖 Recursos de IA para el Curso
    ├── README.md
    ├── guia-uso-etico.md         # [PENDIENTE] Lineamientos de uso ético
    ├── prompts-efectivos.md      # [PENDIENTE] Ejemplos de prompts por tema
    └── recursos-recomendados.md  # [PENDIENTE] Herramientas recomendadas
```

---

## 🎯 Propósito de Cada Carpeta

### `/programa`
Contiene la planeación académica oficial del curso: syllabus, cronogramas y documentos institucionales.

### `/docs`
**Contenido web principal.** Cada unidad tiene su página index.md que se despliega en el sitio Jekyll. Incluye teoría, actividades, recursos y navegación.

### `/recursos-didacticos`
Materiales de apoyo para la impartición del curso. **No se publican en el sitio web** (excluidos en `_config.yml`).

### `/simulaciones`
Guías de uso y recursos para simulaciones interactivas (principalmente PhET). Se usan en actividades prácticas.

### `/evaluacion`
Instrumentos de evaluación por competencias: rúbricas, exámenes, proyectos. Alineados al sistema EBC de UTEQ.

### `/herramientas-ia`
Documentación y guías para uso ético de herramientas de IA como apoyo al aprendizaje en el curso.

---

## 📊 Estado Actual del Proyecto

### ✅ Completado
- Estructura base de carpetas
- Configuración Jekyll (tema Just the Docs)
- MathJax configurado para ecuaciones LaTeX
- Página principal (index.md)
- Syllabus completo
- Unidades 0 y 1 con contenido completo
- Documentación README en carpetas principales

### ⚠️ En Progreso
- Unidades 2-5 (esqueleto creado, falta contenido)
- Cronograma detallado sesión por sesión

### 📋 Pendiente
- Material por sesiones individuales
- Guías de simulaciones específicas
- Instrumentos de evaluación (rúbricas, exámenes)
- Guías de uso de IA
- Recursos didácticos (presentaciones, ejercicios)

---

## 🚀 Uso del Repositorio

### Para desarrollo local:
```bash
# Instalar dependencias
bundle install

# Ejecutar servidor local
bundle exec jekyll serve

# Abrir en navegador
http://localhost:4000/fisica-moderna/
```

### Para publicación en GitHub Pages:
1. Subir a repositorio GitHub
2. Configurar GitHub Pages desde rama `main`
3. Actualizar `url` y `baseurl` en `_config.yml`

---

**Última actualización:** 29 de noviembre de 2025
**Responsable:** Profesor - UTEQ
