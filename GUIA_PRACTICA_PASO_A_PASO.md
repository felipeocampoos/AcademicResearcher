# 🎯 GUÍA PRÁCTICA: De Idea a Paper Publicable

**Para usar desde claude.ai con Projects**

---

## 📦 SETUP INICIAL (Hacer UNA VEZ)

### Paso 0: Configurar tu Proyecto en Claude.ai

1. **Clona el repositorio en tu PC**:
```bash
git clone https://github.com/felipeocampoos/AcademicResearcher.git
cd AcademicResearcher
```

2. **Crea carpeta para tu proyecto específico**:
```bash
mkdir mi-paper-hpp
cd mi-paper-hpp
```

3. **Ir a claude.ai y crear un Project**:
   - Ve a https://claude.ai
   - Click en "Projects" (menú izquierdo)
   - Click "Create Project"
   - Nombre: "HPP Cost-Effectiveness Colombia" (o tu tema)

4. **Agregar Knowledge al Project**:
   - Click en "Add content" → "Upload files"
   - Sube estos 4 archivos desde tu carpeta `AcademicResearcher/`:
     
     ✅ `claude.md` (instrucciones de economía de la salud)
     ✅ Este archivo: `GUIA_PRACTICA_PASO_A_PASO.md`
     ✅ `example_introduction_hpe.md` (opcional, como referencia)

   - **NO necesitas subir las skills manualmente** — Claude.ai tiene acceso a las skills públicas automáticamente cuando las mencionas

5. **¡Listo para empezar!** Ahora todos tus chats en este Project tendrán:
   - Contexto de economía de la salud
   - Acceso automático a las skills cuando las necesites
   - Esta guía como referencia

---

## 🔧 ¿Cómo Funcionan las Skills en Claude.ai?

**Las skills se activan automáticamente según el tipo de tarea:**

| Paso | Skill Automática | Por qué se activa |
|------|-----------------|-------------------|
| 1-2 | `claude.md` | Pregunta de investigación, contexto salud |
| 3 | `academic-researcher` | Análisis de papers |
| 4-5 | `academic-researcher` + `claude.md` | Estructura lit review |
| 6 | `research-paper-writer` | Outline detallado IMRAD |
| 7-12 | `claude.md` + `research-paper-writer` | Drafting secciones |
| 13 | `academic-paper-reviewer` | Peer review simulation |
| 14-15 | `claude.md` | Revision coaching |
| 16-17 | `claude.md` | CHEERS checklist, APA 7 |

**NO necesitas mencionar las skills explícitamente** — Claude las detecta por contexto.

---

## 🚀 PASO A PASO (17 Pasos)

---

# PASO 1: Refina tu Pregunta de Investigación

**🔧 Skill automática**: `claude.md` (contexto de economía de la salud)

**Comando**:
```
Tengo una idea de investigación en economía de la salud:

IDEA: Evaluar costo-efectividad de manejo activo de hemorragia posparto en Colombia

Ayúdame a refinar esta idea cubriendo:
1. Carga de enfermedad
2. Intervenciones existentes
3. Contexto SGSSS
4. Brecha de conocimiento
5. Relevancia para política

Dame pregunta de investigación clara + objetivos
```

**Guardar**: `01_research_question.md`

---

# PASO 2: Analiza Papers Base

**🔧 Skill automática**: `academic-researcher`

**Comando** (repetir para cada paper):
```
Analiza este paper [sube PDF o pega info]:

Extrae:
- Research question
- Metodología
- Findings (ICER, costos)
- Implicaciones
- Limitaciones
- Cita APA 7
```

**Guardar**: `02_papers_analysis.md`

---

# PASO 3: Estructura Literatura Review

**🔧 Skill automática**: `academic-researcher` + `claude.md`

**Comando**:
```
Crea estructura de lit review para [tu pregunta]

Papers base: [pega análisis del Paso 2]

Incluye:
- Theoretical frameworks (CE, CU)
- Thematic synthesis
- Research gaps (Colombia-specific)
- Vocabulario CHEERS 2022
```

**Guardar**: `03_lit_review_outline.md`

---

# PASO 4: Escribe Literatura Review

**🔧 Skill automática**: `claude.md`

**Comando**:
```
Escribe lit review completa:

Outline: [del Paso 3]
Papers: [del Paso 2]

Requisitos:
- Máx 3-4 oraciones/párrafo
- Vocabulario económico
- APA 7
- 1500-2000 palabras
```

**Guardar**: `04_literature_review.md`

---

# PASO 5: Outline Completo del Paper

**🔧 Skill automática**: `research-paper-writer`

**Comando**:
```
Crea outline detallado:

Pregunta: [del Paso 1]
Journal: Health Economics
Formato: IMRAD + CHEERS 2022
Longitud: 6000 palabras

Incluye subsecciones numeradas para:
- Abstract (250)
- Introduction (800)
- Methods (1500)
- Results (1200)
- Discussion (1200)
- Conclusions (300)
```

**Guardar**: `05_paper_outline.md`

---

# PASO 6: Introduction

**🔧 Skill automática**: `claude.md`

**Comando**:
```
Escribe INTRODUCTION (4 párrafos):

Outline: [sección 1 del Paso 5]
Lit review: [del Paso 4]

Párrafos:
1. Carga HPP en Colombia
2. Intervenciones + CE internacional
3. Brecha Colombia-específica
4. Objetivos

~800 palabras, APA 7
```

**Guardar**: `06_introduction.md`

---

# PASO 7: Methods

**🔧 Skill automática**: `research-paper-writer` + `claude.md`

**Comando**:
```
Escribe METHODS siguiendo CHEERS 2022:

Outline: [sección 2 del Paso 5]

Incluye:
- Study design (CEA)
- Perspective (SGSSS)
- Model structure
- Data sources
- Discount rate
- Sensitivity analysis
- Equity subgroups

~1500 palabras, reproducible
```

**Guardar**: `07_methods.md`

---

# PASO 8-10: Results, Discussion, Conclusions

**🔧 Skill automática**: `claude.md`

**Comando similar al anterior** para cada sección, siguiendo el outline.

**Guardar**: 
- `08_results.md`
- `09_discussion.md`
- `10_conclusions.md`

---

# PASO 11: Abstract

**🔧 Skill automática**: `claude.md`

**Comando**:
```
Escribe ABSTRACT (250 palabras):

Secciones: [del Paso 6-10]

Estructura:
- Background (50)
- Methods (70)
- Results (80)
- Conclusions (50)

Sin citas, auto-contenido
```

**Guardar**: `11_abstract.md`

---

# PASO 12: Manuscrito Completo

**🔧 Skill automática**: `claude.md`

**Comando**:
```
Combina todas las secciones en manuscrito:

Abstract: [Paso 11]
Introduction: [Paso 6]
Methods: [Paso 7]
Results: [Paso 8]
Discussion: [Paso 9]
Conclusions: [Paso 10]

Formato Markdown, transiciones suaves
```

**Guardar**: `12_manuscript_complete.md`

---

# PASO 13: Peer Review Simulado

**🔧 Skill automática**: `academic-paper-reviewer`

**Comando**:
```
Simula peer review:

Manuscript: [del Paso 12]
Journal: Health Economics

5 revisores:
1. Methodology Specialist
2. Health Economics Expert
3. Public Health (cross-disciplinary)
4. Devil's Advocate
5. Editor-in-Chief

Decisión final + revisiones requeridas
```

**Guardar**: `13_peer_reviews.md`

---

# PASO 14: Roadmap de Revisión

**🔧 Skill automática**: `claude.md`

**Comando**:
```
Crea revision roadmap:

Manuscript: [Paso 12]
Reviews: [Paso 13]

Para cada revisión REQUERIDA:
- Ubicación (sección, línea)
- Texto actual
- Texto revisado
- Justificación
```

**Guardar**: `14_revision_roadmap.md`

---

# PASO 15: Manuscrito Final

**🔧 Skill automática**: `claude.md`

**Comando**:
```
Aplica revisiones y genera:

Original: [Paso 12]
Roadmap: [Paso 14]

Output:
- Manuscript revisado
- Track changes
- Response to reviewers
```

**Guardar**: `15_manuscript_FINAL.md`

---

# PASO 16: CHEERS 2022 Checklist

**🔧 Skill automática**: `claude.md`

**Comando**:
```
Valida CHEERS 2022:

Manuscript: [Paso 15]

Checklist de 28 items:
- Item, recommendation, ubicación, status
- % compliance
- Acciones faltantes
```

**Guardar**: `16_CHEERS_checklist.md`

---

# PASO 17: Referencias APA 7

**🔧 Skill automática**: `claude.md`

**Comando**:
```
Valida y formatea referencias APA 7:

Manuscript: [Paso 15]

- Lista completa ordenada
- Verificar in-text vs lista
- DOIs correctos
- Formato consistente
```

**Guardar**: `17_references_APA7.md`

---

# ✅ CHECKLIST FINAL

Antes de enviar al journal:

- [ ] Manuscript completo (~6000 palabras)
- [ ] Abstract ≤ 250 palabras
- [ ] CHEERS 2022: 28/28 items ✓
- [ ] Referencias APA 7 correctas
- [ ] Peer review simulado completado
- [ ] Revisiones aplicadas
- [ ] Response to reviewers preparada
- [ ] Limitaciones honestas incluidas
- [ ] Recomendaciones calificadas (no absolutas)

---

# 📊 RESUMEN: Comandos Clave

| Paso | Comando | Skill |
|------|---------|-------|
| 1 | "Ayúdame a refinar esta idea..." | claude.md |
| 2 | "Analiza este paper..." | academic-researcher |
| 3-4 | "Crea/escribe lit review..." | academic-researcher + claude.md |
| 5 | "Crea outline detallado..." | research-paper-writer |
| 6-12 | "Escribe [sección]..." | claude.md |
| 13 | "Simula peer review..." | academic-paper-reviewer |
| 14-17 | "Aplica revisiones/valida..." | claude.md |

---

# ⏱️ TIEMPO ESTIMADO

- Pasos 1-5 (Preparación): 2-3 horas
- Pasos 6-12 (Drafting): 4-6 horas
- Pasos 13-15 (Review): 2-3 horas
- Pasos 16-17 (Validación): 1 hora

**TOTAL: 10-14 horas** (vs 3-6 meses tradicional)

---

# 💡 TIPS

✅ Trabaja en un solo Project de Claude.ai  
✅ Guarda cada output en archivos separados  
✅ Revisa manualmente cada sección antes de continuar  
✅ No saltes el peer review (Paso 13)  
✅ Sé honesto con limitaciones  

❌ No copies texto exacto de papers  
❌ No ignores feedback del peer review  
❌ No sobre-vendas conclusiones  
❌ No envíes sin completar CHEERS checklist  

---

**Versión**: 2.0  
**Para**: Claude.ai Projects  
**Audiencia**: Investigadores economía de la salud
