# Configuración Híbrida: claude.md + 4 Skills Académicas

## 🎯 Objetivo
Combinar lo **mejor de 5 herramientas** para un workflow académico completo:
1. **Tu `claude.md`**: Instrucciones persistentes específicas para economía de la salud
2. **`academic-researcher`**: Templates genéricos, análisis estructurado, múltiples formatos de citas
3. **`research-paper-writer`**: Escritura formal IEEE/ACM, estructura académica rigurosa
4. **`academic-paper-reviewer`**: Simulación de 5 revisores (EIC + 3 peer reviewers + Devil's Advocate)
5. **`academic-pipeline`** (opcional): Orquestador completo research → write → review → revise

---

## 📦 Setup Híbrido Completo

### Paso 1: Instalar todas las skills

```bash
# Skill 1: Análisis y templates
npx skills add https://github.com/shubhamsaboo/awesome-llm-apps --skill academic-researcher

# Skill 2: Escritura formal IEEE/ACM
npx skills add https://github.com/ailabs-393/ai-labs-claude-skills --skill research-paper-writer

# Skill 3: Revisión por pares simulada
npx skills add https://github.com/imbad0202/academic-research-skills --skill academic-paper-reviewer

# Skill 4 (Opcional): Pipeline completo
npx skills add https://github.com/imbad0202/academic-research-skills --skill academic-pipeline
```

### Paso 2: Mantener tu claude.md en la raíz del proyecto

Tu archivo `claude.md` ya está en `/AcademicResearcher/` — se cargará automáticamente.

### Paso 3: Estructura de proyecto recomendada

```
AcademicResearcher/
├── claude.md                          ← Instrucciones persistentes (economía salud)
├── HYBRID_WORKFLOW.md                 ← Esta guía
├── example_introduction_hpe.md         ← Ejemplo de Introduction
├── skills/                            ← Skills instaladas
│   ├── academic-researcher/
│   ├── research-paper-writer/
│   ├── academic-paper-reviewer/
│   └── academic-pipeline/
└── projects/
    └── my-paper-hpe/
        ├── 01-idea/
        │   ├── research_question.md
        │   └── base_papers/
        ├── 02-literature/
        │   ├── papers_analysis.md
        │   └── literature_review.md
        ├── 03-outline/
        │   └── paper_outline.md
        ├── 04-draft/
        │   └── manuscript_v1.md
        ├── 05-review/
        │   └── peer_review_reports.md
        └── 06-final/
            └── manuscript_final.md
```

---

## 📊 Comparación de Skills

| Skill | Propósito | Cuándo Usar | Fortaleza |
|-------|-----------|-------------|-----------|
| **Tu claude.md** | Instrucciones persistentes economía salud | SIEMPRE (base) | Contexto SGSSS, CHEERS 2022, equidad |
| **academic-researcher** | Templates, análisis, citas | Análisis rápido de papers | Múltiples formatos de citas |
| **research-paper-writer** | Escritura formal académica | Drafting estructurado | IEEE/ACM, iteración por secciones |
| **academic-paper-reviewer** | Simulación de peer review | Pre-submisión | 5 revisores, perspectivas múltiples |
| **academic-pipeline** | Orquestador completo | Proyectos grandes | Research → Write → Review → Finalize |

---

## 🔄 Flujo de Trabajo Híbrido Completo

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

---

# 🎓 EJEMPLO COMPLETO: De Idea a Paper Listo

## Contexto del Ejemplo

**Tu situación**:
- Tienes una **idea de investigación**: Evaluar costo-efectividad de manejo activo de HPP en Colombia
- Tienes **3 papers base**:
  1. Roberts et al. (2015) - CE de manejo activo en UK
  2. Coad et al. (2014) - Efectividad clínica
  3. MinSalud (2023) - Estadísticas de mortalidad materna en Colombia
- Objetivo: Paper para **Health Economics** journal (APA 7, CHEERS 2022)

---

## 📋 FASE 0: Setup Inicial

### Crear proyecto
```bash
cd AcademicResearcher/projects
mkdir hpp-ce-colombia
cd hpp-ce-colombia

# Crear estructura
mkdir -p 01-idea/base_papers
mkdir 02-literature
mkdir 03-outline
mkdir 04-draft
mkdir 05-review
mkdir 06-final
```

### Subir papers base
```bash
# Copia tus 3 PDFs a:
cp ~/Downloads/Roberts2015.pdf 01-idea/base_papers/
cp ~/Downloads/Coad2014.pdf 01-idea/base_papers/
cp ~/Downloads/MinSalud2023.pdf 01-idea/base_papers/
```

---

## 📋 FASE 1: Definir Pregunta de Investigación

### Usar: Tu claude.md (Socratic dialogue)

```bash
# En Claude Code
/ars-plan "Evaluación de costo-efectividad de manejo activo de hemorragia posparto en Colombia"
```

**Output esperado** (Socratic dialogue):
```
🤔 Entendamos tu proyecto paso a paso:

1. **Carga de enfermedad**
   ¿Cuál es la magnitud actual de HPP en Colombia?
   → Tú: ~25% de muertes maternas según MinSalud 2023

2. **Intervenciones existentes**
   ¿Qué se hace actualmente y qué alternativas existen?
   → Tú: Manejo expectante vs activo (oxitocina + masaje)

3. **Contexto del sistema de salud**
   ¿Desde qué perspectiva económica?
   → Tú: Sistema de salud (SGSSS), costos directos médicos

4. **Brecha de conocimiento**
   ¿Qué falta en la literatura?
   → Tú: No hay CE en Colombia, datos solo de países de altos ingresos

5. **Relevancia para política**
   ¿Por qué importa para tomadores de decisión?
   → Tú: Presupuesto limitado + inequidad rural/urbana en acceso

📝 Pregunta de investigación refinada:
"¿Es costo-efectivo el manejo activo de HPP comparado con manejo expectante 
desde la perspectiva del SGSSS colombiano, considerando diferencias regionales?"
```

**Guardar**:
```bash
# Copia el output a:
echo "[output del diálogo]" > 01-idea/research_question.md
```

---

## 📋 FASE 2: Analizar Papers Base

### Usar: academic-researcher skill

```bash
# Analizar cada paper
@academic-researcher analyze paper 01-idea/base_papers/Roberts2015.pdf
```

**Output esperado**:
```
📄 PAPER ANALYSIS: Roberts et al. (2015)

**Research Question:**
Is active management of PPH cost-effective in UK NHS?

**Methodology:**
- Design: Cost-effectiveness analysis
- Population: 10,000 women with PPH
- Perspective: UK NHS
- Time horizon: 5 years
- Outcome: QALY gained

**Findings:**
- ICER: £2,800/QALY (below UK WTP threshold £20,000)
- Active: £450/case, Expectant: £280/case
- Incremental: £170/case, 0.06 QALY gain

**Implications:**
- Cost-effective in UK context
- Requires consistent oxytocin supply

**Limitations:**
- UK-specific costs
- Assumes 100% compliance
- No adverse events in expectant arm

**Citation (APA 7):**
Roberts, M. J., Williams, K., & Thompson, R. (2015). Cost-effectiveness 
of active management of postpartum hemorrhage. Journal of Health Economics, 
34, 245–258. https://doi.org/10.1016/j.jhealeco.2015.03.009
```

**Repetir para los 3 papers**:
```bash
@academic-researcher analyze paper 01-idea/base_papers/Coad2014.pdf
@academic-researcher analyze paper 01-idea/base_papers/MinSalud2023.pdf
```

**Guardar**:
```bash
# Compilar los 3 análisis en:
02-literature/papers_analysis.md
```

---

## 📋 FASE 3: Literatura Review Estructurada

### Usar: academic-researcher + claude.md

**Paso 3.1**: Template genérico (skill)
```bash
@academic-researcher structure literature-review on "cost-effectiveness postpartum hemorrhage management"
```

**Output**:
```
📚 LITERATURE REVIEW STRUCTURE

I. INTRODUCTION
   - Context and importance
   - Scope of review

II. THEORETICAL FRAMEWORKS
    - Economic evaluation models
    - Key concepts (QALY, ICER)

III. THEMATIC SYNTHESIS
     - Theme 1: CE in high-income countries
     - Theme 2: Clinical effectiveness
     - Theme 3: Implementation barriers

IV. RESEARCH GAPS
    - Geographic gaps
    - Methodological gaps

V. CONCLUSIONS
```

**Paso 3.2**: Personalizar con claude.md
```bash
# En Claude Code (con claude.md activo)
Personaliza el template anterior para economía de la salud:

Contexto:
- CHEERS 2022 standards
- Perspectiva SGSSS
- Énfasis en equidad (rural vs urbano)
- Transferibilidad de evidencia internacional a Colombia

Papers base: [pega análisis de Fase 2]

Escribe la literatura review completa siguiendo:
- Máx 3-4 oraciones por párrafo
- Vocabulario económico consistente
- Citas en APA 7
- Brecha específica al final
```

**Output esperado**: Literatura review de 4-5 páginas

**Guardar**:
```bash
02-literature/literature_review.md
```

---

## 📋 FASE 4: Crear Outline Detallado

### Usar: research-paper-writer skill

```bash
@research-paper-writer create-outline

Topic: Cost-effectiveness of active PPH management in Colombia
Venue: Health Economics journal
Format: IMRAD + Health Economics (APA 7)
Length: 6000 words
Special requirements: CHEERS 2022 checklist
```

**Output esperado**:
```
📝 PAPER OUTLINE

**Title:** 
Cost-Effectiveness of Active Management of Postpartum Hemorrhage 
in the Colombian Health System: A Decision-Analytic Model

**Abstract** (250 words)
- Background: HPP burden + knowledge gap
- Methods: CEA, perspective SGSSS, 5-year horizon
- Results: ICER, sensitivity analysis
- Conclusions: Policy implications

**1. INTRODUCTION** (800 words)
   1.1 Burden of PPH in Colombia
   1.2 Active vs expectant management
   1.3 International evidence on CE
   1.4 Knowledge gap: Colombia context
   1.5 Study objectives

**2. METHODS** (1500 words)
   2.1 Study design (CEA)
   2.2 Population and setting
   2.3 Perspective (SGSSS)
   2.4 Interventions compared
   2.5 Model structure (decision tree)
   2.6 Data sources
       - Clinical effectiveness (Coad 2014)
       - Costs (Colombian tariffs)
       - Utilities (EQ-5D)
   2.7 Time horizon (5 years)
   2.8 Discount rate (5% per IETS guidelines)
   2.9 Sensitivity analysis
   2.10 Equity analysis (regional subgroups)

**3. RESULTS** (1200 words)
   3.1 Base case analysis
   3.2 Cost breakdown
   3.3 Effectiveness outcomes
   3.4 ICER calculation
   3.5 Sensitivity analysis
       - One-way (key parameters)
       - Probabilistic (uncertainty)
   3.6 Subgroup analysis (equity)

**4. DISCUSSION** (1200 words)
   4.1 Main findings vs literature
   4.2 Policy implications for Colombia
   4.3 Equity considerations
   4.4 Transferability from UK/US contexts
   4.5 Limitations
       - Data quality
       - Model assumptions
       - External validity
   4.6 Future research

**5. CONCLUSIONS** (300 words)
   - Summary of findings
   - Recommendation (with caveats)
   - Context-specific considerations

**REFERENCES** (APA 7)

**APPENDICES**
- CHEERS 2022 Checklist
- Model parameters table
- Sensitivity analysis details
```

**Personalizar con claude.md**:
```bash
# Refinar outline usando tu experiencia:
Ajusta el outline anterior para incluir:
- Mención explícita de disparidades rural/urbano
- Análisis de costo-oportunidad (budget impact)
- Threshold colombiano (WTP local vs internacional)

Vocabulario de mi claude.md: [términos clave]
```

**Guardar**:
```bash
03-outline/paper_outline.md
```

---

## 📋 FASE 5: Drafting Iterativo

### Usar: claude.md (primario) + research-paper-writer (secundario)

**Estrategia**: Escribir sección por sección

### Sección 1: INTRODUCTION

```bash
# Usar tu claude.md (ya tienes ejemplo)
Escribe la INTRODUCTION basándote en:

Outline: [pegar sección 1 del outline]
Literatura: [02-literature/literature_review.md]
Pregunta de investigación: [01-idea/research_question.md]

Estructura:
- Párrafo 1: Carga de HPP en Colombia
- Párrafo 2: Intervenciones existentes + CE internacional
- Párrafo 3: Brecha de conocimiento (Colombia)
- Párrafo 4: Objetivos específicos

Estilo: Tu claude.md (máx 3-4 oraciones/párrafo, tono crítico, contexto SGSSS)
```

**Output**: Introduction de ~800 palabras

### Sección 2: METHODS

```bash
# Usar research-paper-writer (más técnico)
@research-paper-writer draft-section "Methods"

Context: Cost-effectiveness analysis of PPH management
Outline: [pegar sección 2 del outline]
Special requirements:
- CHEERS 2022 compliance
- Decision tree model
- Colombian cost data sources
- Equity analysis by region

Tone: Technical, precise, reproducible
```

**Output**: Methods de ~1500 palabras

### Sección 3-5: Repetir proceso

**Guardar cada sección**:
```bash
04-draft/01_introduction.md
04-draft/02_methods.md
04-draft/03_results.md
04-draft/04_discussion.md
04-draft/05_conclusions.md
```

**Combinar todo**:
```bash
cat 04-draft/*.md > 04-draft/manuscript_v1.md
```

---

## 📋 FASE 6: Peer Review Simulado

### Usar: academic-paper-reviewer skill

```bash
@academic-paper-reviewer review 04-draft/manuscript_v1.md

Target venue: Health Economics journal
Paper type: Cost-effectiveness analysis
```

**Output esperado**:
```
🔍 PEER REVIEW SIMULATION

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

📋 REVIEWER #1: METHODOLOGY SPECIALIST

**Overall Assessment:** ACCEPT with Minor Revisions

**Strengths:**
✓ Solid decision-analytic model
✓ CHEERS 2022 compliant
✓ Appropriate discount rate (5%)

**Concerns:**
⚠ Uncertainty characterization could be stronger
  - Probabilistic sensitivity analysis: only 1000 iterations?
  - Consider 10,000 for stability

⚠ Model validation
  - No comparison with actual Colombian data
  - Suggest validation against pilot sites

**Minor Issues:**
- Table 2: CI overlaps, difficult to read
- Figure 1: Decision tree could show probabilities

**Recommendation:** Accept after addressing PSA iterations

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

📋 REVIEWER #2: DOMAIN EXPERT (Health Economics)

**Overall Assessment:** ACCEPT with Minor Revisions

**Strengths:**
✓ Clear research question
✓ Appropriate Colombian context
✓ Equity analysis is valuable

**Concerns:**
⚠ Transferability assumptions
  - Effectiveness data from Coad 2014 (UK)
  - How does Colombian clinical context differ?
  - Suggest subgroup analysis by facility capacity

⚠ Cost data sources
  - SOAT tariffs may underestimate true costs
  - Consider sensitivity analysis on cost assumptions

**Minor Issues:**
- Missing discussion of budget impact
- WTP threshold: justify COP 183M choice

**Recommendation:** Accept after clarifying transferability

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

📋 REVIEWER #3: CROSS-DISCIPLINARY (Public Health)

**Overall Assessment:** ACCEPT

**Strengths:**
✓ Policy-relevant question
✓ Addresses equity (rural/urban)
✓ Clear implications for SGSSS

**Concerns:**
⚠ Implementation barriers not discussed
  - Oxytocin cold chain requirements
  - Training needs for healthcare workers

⚠ Equity analysis
  - Good start, but could expand
  - Consider indigenous populations
  - Socioeconomic gradients?

**Minor Issues:**
- Conclusions could be stronger on policy
- Missing call for pilot implementation

**Recommendation:** Accept as is (suggestions optional)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

📋 REVIEWER #4: DEVIL'S ADVOCATE

**Overall Assessment:** ACCEPT with Major Revisions

**Core Argument Challenge:**

❌ Central Claim: "Active management is cost-effective in Colombia"

**Counter-argument:**
Your ICER depends critically on:
1. Effectiveness transfer from UK context
2. Cost estimates from tariffs (not real-world)
3. WTP threshold choice (arbitrary?)

**What if:**
- Colombian compliance rates are lower? (rural areas)
- Real costs are 2x tariff? (common in Colombia)
- Adverse events are higher? (not captured in model)

**Strongest opposing view:**
"This analysis provides UPPER BOUND on cost-effectiveness. 
Real-world implementation likely worse due to:
- Supply chain failures
- Training gaps
- Quality variation across facilities"

**Logical Issues:**
⚠ Circular reasoning in Discussion
  - "CE because ICER < threshold"
  - But threshold itself is debated

⚠ Overstated conclusions
  - "Should be implemented" → Too strong
  - Better: "May be cost-effective IF conditions X, Y, Z"

**Recommendation:** Major revision to qualify claims

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

📋 EDITOR-IN-CHIEF: EDITORIAL DECISION

**Decision:** MINOR REVISIONS REQUIRED

**Synthesis:**
All reviewers see value in this work. The methodology is sound 
(R1, R2), addresses important policy question (R3), but claims 
need qualification (R4).

**Required Revisions:**
1. [R1] Increase PSA to 10,000 iterations
2. [R2] Add sensitivity on transferability assumptions
3. [R4] Qualify conclusions (add "under conditions X, Y, Z")

**Optional (strengthen paper):**
4. [R2] Discuss budget impact
5. [R3] Expand equity analysis
6. [R4] Acknowledge uncertainty in WTP threshold

**Timeline:** 4 weeks for revisions

**Next Steps:** Revise and resubmit
```

**Guardar**:
```bash
05-review/peer_review_reports.md
```

---

## 📋 FASE 7: Revision Basada en Reviews

### Usar: claude.md (revision coach)

```bash
/ars-revision-coach

Context:
- Draft: 04-draft/manuscript_v1.md
- Reviews: 05-review/peer_review_reports.md

Focus on:
1. R1: Increase PSA iterations (Methods)
2. R2: Transferability discussion (Discussion)
3. R4: Qualify conclusions (Conclusions)
```

**Output esperado**:
```
📝 REVISION ROADMAP

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

REVISION #1: Methods - PSA Iterations
**Current:** "We conducted probabilistic sensitivity analysis with 1,000 iterations..."
**Revised:** "We conducted probabilistic sensitivity analysis with 10,000 iterations to ensure stable confidence intervals..."
**Location:** Methods, Section 2.9, Line 245

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

REVISION #2: Discussion - Transferability
**Add new paragraph after Line 487:**

"The clinical effectiveness estimates in our model derive primarily from 
UK-based trials (Coad et al., 2014), which may not fully capture Colombian 
clinical contexts. Differences in facility capacity, healthcare worker 
training, and patient characteristics could affect real-world effectiveness. 
However, the intervention's mechanism (oxytocin-induced uterine contraction) 
is physiologically universal, suggesting transferability of effect size is 
reasonable. We addressed this uncertainty through sensitivity analysis on 
effectiveness parameters (Figure 3B), showing cost-effectiveness is robust 
to ±30% variation in relative risk reduction."

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

REVISION #3: Conclusions - Qualification
**Current:** "Active management should be implemented nationwide."
**Revised:** "Active management appears cost-effective in Colombia under 
the following conditions: (1) consistent oxytocin supply chain, (2) adequate 
healthcare worker training, and (3) facility capacity to manage complications. 
Implementation should be phased, prioritizing high-volume facilities with 
quality improvement systems, followed by evaluation before broader scale-up."
**Location:** Conclusions, Lines 612-615

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

**Apply revisions? Y/N**
```

**Aplicar y guardar**:
```bash
# Versión revisada
06-final/manuscript_v2_revised.md
```

---

## 📋 FASE 8: Re-Review (Verificación)

### Usar: academic-paper-reviewer (re-review mode)

```bash
@academic-paper-reviewer re-review 06-final/manuscript_v2_revised.md

Original reviews: 05-review/peer_review_reports.md
Focus: Verify required revisions were addressed
```

**Output esperado**:
```
✅ RE-REVIEW VERIFICATION

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

R1 CONCERN: PSA iterations
✅ ADDRESSED: Methods now states 10,000 iterations (Line 246)

R2 CONCERN: Transferability
✅ ADDRESSED: New Discussion paragraph (Lines 488-496)

R4 CONCERN: Overstated conclusions
✅ ADDRESSED: Conclusions qualified with conditions (Lines 612-615)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

📋 EDITOR DECISION: ACCEPT

All required revisions satisfactorily addressed.
Manuscript ready for publication.
```

---

## 📋 FASE 9: Formateo Final

### Usar: academic-researcher (citas) + research-paper-writer (formato)

```bash
# Validar todas las citas APA 7
@academic-researcher validate-citations 06-final/manuscript_v2_revised.md

# Formatear según Health Economics journal
@research-paper-writer format-for-journal "Health Economics" 06-final/manuscript_v2_revised.md
```

**Guardar versión final**:
```bash
06-final/manuscript_FINAL_health_econ.md
06-final/manuscript_FINAL_health_econ.docx  # Si conviertes con Pandoc
```

---

## 📋 FASE 10: CHEERS 2022 Checklist

### Usar: claude.md

```bash
Valida que mi paper cumple CHEERS 2022:

Paper: 06-final/manuscript_FINAL_health_econ.md

Genera checklist completa con:
- Item number
- Recommendation
- Location in manuscript (page/section)
- Compliance status (✓/✗)
```

**Output esperado**:
```
✅ CHEERS 2022 COMPLIANCE CHECKLIST

Item 1: Title - Identify the study as an economic evaluation
  ✓ Compliant (Title clearly states "Cost-Effectiveness")

Item 2: Abstract - Structured summary
  ✓ Compliant (Background, Methods, Results, Conclusions)

Item 3: Background and objectives
  ✓ Compliant (Introduction, Lines 45-98)

...

Item 28: Funding sources
  ⚠ Missing - Add funding statement or "No funding" declaration

OVERALL: 27/28 items compliant (96%)
ACTION: Add funding statement to comply 100%
```

---

## 🎉 RESULTADO FINAL

Has completado el workflow completo:

✅ **Idea refinada** → Research question clara y enfocada
✅ **Literatura revisada** → 3 papers base + síntesis temática
✅ **Outline validado** → Estructura IMRAD + Health Economics
✅ **Draft completo** → 6000 palabras, CHEERS 2022 compliant
✅ **Peer review simulado** → 5 revisores independientes
✅ **Revisiones aplicadas** → Versión mejorada basada en feedback
✅ **Re-review aprobado** → Verificación de cambios
✅ **Formato final** → Listo para Health Economics journal
✅ **CHEERS checklist** → 100% compliant

**Total time**: ~2-3 semanas (vs 6+ meses tradicional)

---

## 📊 Matriz de Decisión: Qué Skill Usar Cuándo

| Fase | Tarea | Tool Principal | Tool Secundario | Rationale |
|------|-------|---------------|-----------------|-----------|
| 1 | Definir pregunta | claude.md | - | Socratic dialogue específico para salud |
| 2 | Analizar papers | academic-researcher | - | Análisis rápido estructurado |
| 3 | Lit review | claude.md | academic-researcher | Profundidad + templates |
| 4 | Outline | research-paper-writer | claude.md | Estructura académica + personalización |
| 5 | Drafting | claude.md | research-paper-writer | Contextualización > estructura genérica |
| 6 | Peer review | academic-paper-reviewer | - | Simulación multi-perspectiva única |
| 7 | Revision | claude.md | - | Revision coach especializado |
| 8 | Re-review | academic-paper-reviewer | - | Verificación automática |
| 9 | Formateo | research-paper-writer | academic-researcher | Formato journal + citas |
| 10 | Checklist | claude.md | - | CHEERS 2022 conocimiento |

---

## 🚀 Quick Commands Summary

```bash
# Setup
cd AcademicResearcher/projects && mkdir my-paper && cd my-paper

# Fase 1: Pregunta
/ars-plan "Tu idea de investigación"

# Fase 2: Análisis
@academic-researcher analyze paper [file.pdf]

# Fase 3: Lit review
@academic-researcher structure literature-review on "[topic]"
# Luego personalizar con claude.md

# Fase 4: Outline
@research-paper-writer create-outline

# Fase 5: Drafting
# Usar claude.md para cada sección

# Fase 6: Review
@academic-paper-reviewer review manuscript.md

# Fase 7: Revision
/ars-revision-coach

# Fase 8: Re-review
@academic-paper-reviewer re-review manuscript_v2.md

# Fase 9: Formateo
@academic-researcher validate-citations manuscript.md
@research-paper-writer format-for-journal "[journal name]" manuscript.md

# Fase 10: Checklist
# Usar claude.md para CHEERS 2022
```

---

**Versión**: 2.0 (Completa con 4 skills + ejemplo end-to-end)  
**Fecha**: Mayo 2026  
**Basado en**: ARS v3.7.3 + Lishix520 + academic-researcher + research-paper-writer + academic-paper-reviewer
