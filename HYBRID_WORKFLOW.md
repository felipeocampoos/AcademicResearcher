# Configuración Híbrida: claude.md + academic-researcher

## 🎯 Objetivo
Combinar lo **mejor de ambos mundos**:
- **Tu `claude.md`**: Instrucciones persistentes específicas para economía de la salud
- **`academic-researcher` skill**: Templates genéricos, análisis estructurado, múltiples formatos de citas

---

## 📦 Setup Híbrido

### Paso 1: Instalar la skill

```bash
npx skills add https://github.com/shubhamsaboo/awesome-llm-apps --skill academic-researcher
```

### Paso 2: Mantener tu claude.md en la raíz del proyecto

Tu archivo `claude.md` ya está en `/AcademicResearcher/` — se cargará automáticamente.

### Paso 3: Crear archivo de referencia rápida

He creado `HYBRID_WORKFLOW.md` que incluye:
- Cuándo usar cada herramienta
- Workflows recomendados
- Comandos de ejemplo

---

## 🔄 Flujo de Trabajo Híbrido

### Escenario 1: Análisis Rápido de Paper

**Usa**: `academic-researcher` skill

```bash
# En Claude Code
@academic-researcher analyze paper "Smith et al 2023 - Cost-effectiveness of HPP"

# Respuesta rápida con:
# - Research question
# - Methodology
# - Findings
# - Implications
# - Limitations
# - Citation en APA/MLA/Chicago
```

**Cuándo usar**: Cuando necesitas resumen rápido sin contexto específico de economía de la salud.

---

### Escenario 2: Escribir Introduction para tu Paper

**Usa**: Tu `claude.md`

```bash
# En Claude Code (con claude.md activo)
/ars-plan "Costo-efectividad de manejo activo de HPP en Colombia"

# Luego:
Escribe la INTRODUCTION basándote en:
[contexto específico de tu investigación]
```

**Por qué**: Tu `claude.md` entiende:
- CHEERS 2022 standards
- Contexto SGSSS colombiano
- Equidad y disparidades
- Términos económicos específicos (ICER, QALY, WTP)

---

### Escenario 3: Literatura Review Completa

**Usa**: Ambas

**Fase 1**: Estructura (academic-researcher)
```
@academic-researcher structure literature-review on 
"cost-effectiveness HPP management"

# Te da template básico con:
# - Theoretical frameworks
# - Thematic synthesis sections
# - Research gaps
# - Conclusions structure
```

**Fase 2**: Personalización (tu claude.md)
```
Usando el template anterior, adapta para economía de la salud:
- Enfatiza perspectiva del sistema de salud (SGSSS)
- Incluye análisis de equidad por región
- Vincula cada gap a política colombiana
- Usa vocabulario de CHEERS 2022

Mi contexto: [tus papers clave + pregunta específica]
```

---

### Escenario 4: Gestión de Citas

**Usa**: `academic-researcher` skill

```bash
@academic-researcher format-citations

Paper 1: Roberts et al., Journal Health Economics, 2015, vol 34
Paper 2: Coad et al., Lancet Maternal Health, 2014

Formatos: APA 7, MLA 9, Chicago 17
```

**Luego**: Verifica en tu `claude.md` que sean **APA 7** (tu estándar) y úsalas en tu draft.

---

## 🛠️ Comandos Híbridos Recomendados

### Para iniciación de proyecto

```bash
# Paso 1: Estructura básica (skill)
@academic-researcher structure paper on "your-topic"

# Paso 2: Contexto específico (claude.md)
/ars-plan "Tu pregunta específica en salud"

# Paso 3: Combine ambos outputs
```

### Para revisión de literatura

```bash
# Paso 1: Papers encontrados (skill)
@academic-researcher summarize-batch [papers.txt]

# Paso 2: Síntesis con contexto económico-sanitario (claude.md)
Sintetiza estos papers en el marco de:
[contexto de tu investigación + CHEERS 2022]
```

### Para drafting

```bash
# Usa SOLO tu claude.md (más específico)
/ars-draft [outline-validado]

# El draft seguirá tu estilo de economía de la salud
```

---

## 📋 Matriz de Decisión: ¿Cuándo usar cada cosa?

| Tarea | academic-researcher | Tu claude.md | Ambas |
|-------|-------------------|------------|-------|
| Analizar paper genérico | ✅ Perfecto | ❌ Overkill | - |
| Escribir Introduction | ❌ Muy genérico | ✅✅ Perfecto | - |
| Estructura lit review | ✅ Buenos templates | ✅ Mejor contexto | ✅ Combina |
| Citas múltiples formatos | ✅✅ Especializada | ✅ Solo APA7 | - |
| Methods (economía salud) | ❌ No entiende | ✅✅ Perfecta | - |
| Análisis equidad | ❌ No menciona | ✅✅ Integrado | - |
| Discussión (política) | ❌ No aplica | ✅✅ Perfecta | - |
| Graphical abstract | ✅ Puede ayudar | ✅ Siguiendo estándares | ✅ Combina |

---

## 🎓 Ejemplo Completo: Proyecto Nuevo

### Setup Inicial

```bash
# 1. Crear proyecto
mkdir mi-paper-hpe
cd mi-paper-hpe

# 2. Clonar tu repo con claude.md
git clone https://github.com/felipeocampoos/AcademicResearcher.git
# Ahora tienes claude.md + example_introduction_hpe.md

# 3. Instalar skill
npx skills add https://github.com/shubhamsaboo/awesome-llm-apps --skill academic-researcher

# 4. Crear archivo de proyecto
touch PROJECT.md
```

### Fase 1: Planificación (claude.md)

```
En Claude Code, con claude.md activo:

/ars-plan "Evaluación de costo-efectividad de [tu intervención] en [población colombiana]"

# Respuesta: Diálogo socrático que mapea:
# - Carga de enfermedad
# - Intervenciones existentes
# - Brecha específica
# - Contexto SGSSS
```

### Fase 2: Estructura de Lit Review (Skill + claude.md)

```
Primero (skill):
@academic-researcher structure literature-review on "your-topic"
# Te da template genérico

Luego (claude.md):
Personaliza este template para:
- Health economics perspective
- CHEERS 2022 framework
- Colombian health system context
- Equity considerations

# Respuesta: Template adaptado a tu dominio
```

### Fase 3: Análisis Rápido de Papers (Skill)

```
@academic-researcher analyze paper "Author Year - Title"

# Respuesta rápida:
# - Research question
# - Methods
# - Results
# - Limitations
# - Citation en múltiples formatos
```

### Fase 4: Drafting (claude.md)

```
Con claude.md activo:

/ars-draft "Completed outline: [pega tu outline]"

# Respuesta: Borrador en prosa siguiendo:
# - IMRAD + Health Economics
# - Tono crítico
# - Énfasis en equidad
# - Contexto colombiano
```

### Fase 5: Validación de Citas (Skill)

```
@academic-researcher validate-citations draft.md

# O si necesitas reformatear:
@academic-researcher convert-citations --from apa --to chicago

# Luego verifica que sean APA 7 (tu estándar)
```

### Fase 6: Revisión Final (claude.md)

```
/ars-revision-coach

# Dimensiones de evaluación (de tu claude.md):
# - Claridad
# - Rigor metodológico
# - Relevancia política
# - Equidad
# - Reproducibilidad
```

---

## 🔗 Integración en tu Repositorio

Tu estructura debería ser:

```
AcademicResearcher/
├── claude.md                          ← Instrucciones persistentes
├── example_introduction_hpe.md         ← Referencia
├── HYBRID_WORKFLOW.md                 ← Este archivo (guía)
├── skills/
│   └── academic-researcher/           ← Skill instalada
└── projects/
    └── my-paper-hpe/
        ├── outline.md
        ├── draft.md
        ├── literature-review.md
        └── citations.bib
```

---

## 🚀 Quick Start: Tu Primer Paper

### Comando 1: Inicializar
```bash
/ars-plan "Costo-efectividad de [intervención] en [población]"
```

### Comando 2: Buscar literatura
```bash
/ars-lit-review "health economics [tema] Colombia"
```

### Comando 3: Analizar papers encontrados
```bash
@academic-researcher summarize-batch [papers-encontrados.txt]
```

### Comando 4: Crear outline personalizado
```
Usando síntesis anterior + output de /ars-lit-review, 
crea un outline IMRAD que incluya:
- Contexto de carga de enfermedad (datos colombianos)
- Brecha específica (¿qué falta localmente?)
- Relevancia para SGSSS
```

### Comando 5: Drafting
```bash
/ars-draft "[outline-validado]"
```

### Comando 6: Validación de citas
```bash
@academic-researcher validate-citations draft.md
```

### Comando 7: Revisión
```bash
/ars-revision-coach
```

---

## ⚡ Ventajas del Setup Híbrido

✅ **Lo mejor de ambos mundos**:
- academic-researcher: Rápido, múltiples formatos, templates probados
- Tu claude.md: Profundo, contextualizado, agentes especializados

✅ **Flexibilidad**:
- Usa skill para tareas genéricas
- Usa claude.md para lo específico de tu dominio

✅ **Eficiencia**:
- Skill para análisis rápidos
- claude.md para profundidad

✅ **Escala**:
- Ambas herramientas se complementan
- No hay conflicto, sino sinergia

---

## 🚨 Reglas Críticas (IRON RULES)

1. **Para economía de la salud**: SIEMPRE usa tu `claude.md` (es más específico)
2. **Para templates genéricos**: Puedes usar `academic-researcher` pero personalizalo con `claude.md`
3. **Para citas**: Usa `academic-researcher` para generar en múltiples formatos, pero valida con APA 7 (tu estándar)
4. **Para CHEERS 2022 compliance**: SOLO tu `claude.md` lo entiende
5. **Para contexto colombiano**: SOLO tu `claude.md` lo tiene

---

## 📚 Archivos de Referencia

En tu repositorio ya tienes:
- ✅ `claude.md` — Instrucciones persistentes
- ✅ `example_introduction_hpe.md` — Ejemplo de Introduction
- ✅ `HYBRID_WORKFLOW.md` — Este archivo (guía de uso)

Próximo paso: Crear tu primer proyecto usando este workflow híbrido.

---

**Versión**: 1.0  
**Fecha**: Mayo 2026  
**Basado en**: ARS v3.7.3 + Lishix520 + academic-researcher skill
