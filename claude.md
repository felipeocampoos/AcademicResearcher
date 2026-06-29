# Claude.md - Health Economics Research

## 🎯 Contexto del Proyecto

Este proyecto integra investigación en **economía de la salud** (health economics) con énfasis en:
- Análisis de políticas de salud pública
- Evaluación económica de intervenciones sanitarias
- Estudios de costo-efectividad y costo-utilidad
- Sistemas de salud y acceso
- Equidad y determinantes sociales de la salud
- Investigación en contextos de países en desarrollo (especialmente Colombia/Latinoamérica)

**Flujo típico**: Pregunta de investigación → Revisión de literatura sistemática → Metodología económica → Análisis → Política/Implicaciones

---

## 📚 Marco de Referencia

### Estándares Metodológicos Clave
- **CHEERS 2022**: Consolidated Health Economic Evaluation Reporting Standards
- **PRISMA**: Para revisiones sistemáticas
- **STROBE**: Para estudios observacionales
- **GRADE**: Para evaluación de calidad de evidencia

### Estructura Estándar (IMRAD + Economía)
1. **Introduction**: Carga de enfermedad, brecha en conocimiento, relevancia política
2. **Methods**: Perspectiva económica, población, intervenciones, horizonte temporal, descuento
3. **Results**: Costos, efectividad, análisis de sensibilidad, equidad
4. **Discussion**: Implicaciones para política, limitaciones, generalizabilidad
5. **Conclusions**: Recomendaciones basadas en evidencia

---

## 🌍 Contexto Disciplinario

### Términos Clave (reutilizables en papers)
- **Costo-efectividad (CE)**: Ratio incremental de costo-efectividad (ICER)
- **Costo-utilidad (CU)**: QALY/DALY como medidas de desenlace
- **Evaluación económica**: Análisis comparativo de costos y consecuencias
- **Brecha de conocimiento**: Falta de evidencia local/contextual
- **Determinantes sociales de la salud**: Factores estructurales de inequidad
- **Perspectiva del sistema de salud**: Costos directos médicos
- **Análisis de sensibilidad**: Robustez de resultados a supuestos

### Contexto Colombiano/Latinoamericano
- Sistema General de Seguridad Social en Salud (SGSSS)
- Disponibilidad de datos en bases de mortalidad/morbilidad nacionales
- Relevancia de estudios en poblaciones vulnerables
- Limitaciones de presupuesto para intervenciones

---

## ✍️ Preferencias de Escritura

### Tono y Estilo
- **Formal pero accesible**: Lenguaje académico sin jerga innecesaria
- **Evidencia-centrado**: Toda afirmación respaldada por citas
- **Pragmático**: Énfasis en aplicabilidad e implicaciones para política
- **Crítico**: Reconocimiento de limitaciones y sesgos potenciales

### Estructura de Párrafos
- Máximo 3-4 oraciones por párrafo (excepto métodos)
- Una idea principal por párrafo
- Iniciación con tema (topic sentence)
- Cierre con implicación o enlace

### Convenciones
- Español en borradores iniciales → Inglés académico en versión final
- Mantener vocabulario económico consistente (ICER, QALY, etc.)
- Números: usar separadores según contexto (1.5 vs 1,5)
- Referencias: APA 7th edition
- Siglas con definición al primer uso

### Estructuras Reutilizables

#### Para Brecha de Investigación
"Although [intervention] has shown [benefit] in [context A], [specific gap] remains unexplored in [context B]. This is particularly relevant given [policy/equity implication]."

#### Para Resultados de Costo-Efectividad
"The intervention resulted in [QALY/DALY gain] at an incremental cost of [amount], yielding an ICER of [value] per QALY gained. This [exceeds/is below] the [country-specific/regional] willingness-to-pay threshold of [amount]."

#### Para Equidad
"Stratified analysis revealed [difference] between [subgroups], suggesting [equity implication]. These disparities may reflect [structural factors], underscoring the need for [targeted approach]."

---

## 🔧 Agentes y Workflow

### Fase 1: Planificación Estratégica (Strategist)
**Entrada**: Pregunta de investigación inicial  
**Salida**: Outline detallado, gap analysis, marco teórico

**Preguntas Socráticas Clave**:
1. ¿Cuál es la carga actual de enfermedad?
2. ¿Qué intervenciones existen y cuál es su costo-efectividad?
3. ¿Cuál es el contexto local (población, sistema de salud)?
4. ¿Cuál es la brecha específica de conocimiento/política?
5. ¿Para quién es esta evidencia (tomadores de decisión)?

**Análisis de Brecha**:
- Revisar 5-8 papers clave en economía de la salud del tema
- Identificar: métodos usados, poblaciones, contextos geográficos
- Mapear: ¿qué falta en contextos de bajos/medianos ingresos?
- Formular: pregunta específica y alcance

### Fase 2: Draft Writer (Composer)
**Entrada**: Outline validado + literatura compilada  
**Salida**: Borrador en español (párrafos completos, no bullets)

**Proceso en dos etapas**:
1. Outline detallado por sección con puntos clave + citas
2. Convertir a prosa fluida (párrafos completos, transiciones)

**Validaciones**:
- Cada claim respaldado por cita
- Métodos económicos explicados claramente
- Resultados en formato CHEERS
- Implicaciones vinculadas a pregunta inicial

### Fase 3: Abstract Bilingual Agent
**Entrada**: Paper completo en español  
**Salida**: Abstract en inglés + versión en español

**Requisitos**:
- Máx 250 palabras (inglés)
- Estructura: Background → Methods → Results → Conclusions
- Métodos económicos claros (ej: "cost-effectiveness analysis with ICER")
- Sin citas en abstract

### Fase 4: Citation Compliance Agent
**Entrada**: Draft completo  
**Salida**: Validación de citas, referencias actualizadas

**Validaciones**:
- APA 7th edition consistency
- Citas que de verdad existen (anti-hallucination)
- Autores/años correctos
- URLs actualizadas para papers digitales

### Fase 5: Revision Coach
**Entrada**: Draft + feedback/comentarios  
**Salida**: Iteraciones mejoradas

**Dimensiones de Evaluación**:
1. **Claridad**: ¿Entienden economistas y policy makers?
2. **Rigor metodológico**: ¿Sigue estándares CHEERS?
3. **Relevancia política**: ¿Tiene implicaciones claras?
4. **Equidad**: ¿Considera impactos en subgrupos vulnerables?
5. **Reproducibilidad**: ¿Suficiente detalle para replicar?

---

## 📖 Referencia: Estructura de Paper Típico

```
TITLE
- Framing: intervención + población + contexto

ABSTRACT (250 palabras)
- Background (carga de enfermedad + brecha)
- Methods (tipo de análisis económico + perspectiva)
- Results (ICER + análisis de sensibilidad)
- Conclusions (recomendación + contexto local)

INTRODUCTION
- Carga de enfermedad / importancia del problema
- Intervenciones existentes y su costo-efectividad
- Brecha específica (¿qué no se sabe en este contexto?)
- Relevancia para política/práctica
- Objetivos específicos

METHODS
- Study design (tipo de evaluación económica)
- Population (criterios de inclusión/exclusión)
- Perspective (sistema de salud / sociedad)
- Interventions compared
- Outcomes (medidas de efectividad: QALY, DALY, etc.)
- Time horizon (corto/largo plazo)
- Discount rate (si aplica)
- Data sources (costos, efectividad, utilidades)
- Analysis (costo-efectividad, sensibilidad)

RESULTS
- Base case (ICER principal)
- Subgroup analysis (equidad)
- Sensitivity analysis (robustez)
- Threshold analysis (willingness-to-pay)

DISCUSSION
- Interpretación vs literatura
- Implicaciones para política
- Limitaciones (validez interna/externa)
- Equidad y transferibilidad
- Futuras investigaciones

CONCLUSIONS
- Recomendación clara
- Caveat respecto a contexto

REFERENCES (APA 7th)
```

---

## 🚀 Comandos de Uso

**Para iniciar proyecto nuevo**:
```
/ars-plan "Evaluación de costo-efectividad de [intervención] en [población]"
```
Respuesta: Socratic dialogue para mapear estructura de paper

**Para revisar literatura rápidamente**:
```
/ars-lit-review "health economics [tema] Latin America"
```
Respuesta: Síntesis de 5-8 papers + brecha identificada

**Para drafting**:
```
/ars-draft "Completed outline: [pegar outline validado]"
```
Respuesta: Borrador en español, párrafos completos

**Para validación de citas**:
```
/ars-citation-check
```
Respuesta: Auditoría de referencias + correcciones

---

## 🛡️ Reglas Críticas (IRON RULES)

1. **NUNCA** halucinar citas. Si no encontramos una referencia → decirlo explícitamente
2. **SIEMPRE** reportar costos con divisa/año claramente especificados
3. **SIEMPRE** distinguir entre costo directo e indirecto (cuando sea relevante)
4. **NUNCA** hacer recomendación de política sin limitaciones explícitas
5. **SIEMPRE** reportar ICER con intervalo de confianza o rango de sensibilidad
6. **NUNCA** ignorar equidad: reportar resultados por subgrupos relevantes
7. **SIEMPRE** citar CHEERS 2022 al describir metodología de evaluación económica

---

## 🔍 Anti-Patrones a Evitar

| Anti-Patrón | Por Qué Falla | Comportamiento Correcto |
|------------|---------------|----------------------|
| Confundir eficacia con costo-efectividad | Una intervención eficaz no necesariamente es costo-efectiva | Reportar ambas: ¿funciona? + ¿vale el costo? |
| Ignorar perspectiva económica | El mismo ICER significa diferente cosa desde sistema vs sociedad | Especificar claramente la perspectiva adoptada |
| No reportar descuento | Supuesto oculto sobre valor del tiempo | Siempre explícito: tasa de descuento X% anual |
| Aplicar threshold global | ICER aceptable varía por país y contexto | Usar threshold de país/región específica |
| Ignorar heterogeneidad | Promedios ocultan inequidades | Estratificar por grupos vulnerables |
| Hacer recomendación sin limitaciones | Falsa certeza | Explicar "bajo qué condiciones esta recomendación aplica" |

---

## 📊 Tipo de Análisis Económicos Típicos

- **Costo-Beneficio (CB)**: Costos vs beneficios monetarios (ej: productividad ganada)
- **Costo-Efectividad (CE)**: Costos vs desenlaces naturales (ej: vidas salvadas, DALY evitados)
- **Costo-Utilidad (CU)**: Costos vs QALY (calidad + cantidad de vida)
- **Presupuesto de Impacto**: ¿Cuánto cuesta implementar en un sistema de salud real?
- **Análisis de Desigualdad**: Diferencias en costo-efectividad entre grupos socioeconómicos

---

## 🎓 Vocabulario Técnico (Reutilizable)

**Por traducir con cuidado**:
- QALY = "año de vida ajustado por calidad"
- DALY = "año de vida perdido por discapacidad"
- ICER = "razón incremental de costo-efectividad"
- WTP = "disposición a pagar"
- Willingness-to-pay threshold = "umbral de costo-efectividad"
- Dominance = "dominancia (estrategia superior en costos y efectividad)"

---

## 📋 Checklist Pre-Submisión

- [ ] Abstract ≤250 palabras (inglés)
- [ ] CHEERS 2022 checklist completado
- [ ] Métodos económicos claramente descritos
- [ ] Descuento (si aplica) especificado
- [ ] ICER reportado con intervalo de sensibilidad
- [ ] Equidad: análisis de subgrupos incluido
- [ ] Limitaciones explícitamente discutidas
- [ ] Implicaciones para política claramente vinculadas a resultados
- [ ] Citas: sin hallucinations, APA 7th
- [ ] Conflicto de interés declarado
- [ ] Financiamiento (si aplica) reportado

---

## 🔗 Recursos Externos

- **CHEERS 2022**: https://www.journals.elsevier.com/value-in-health
- **GRADE**: https://www.gradeworkinggroup.org/
- **Health Economics**: Journal oficial de la disciplina
- **Cochrane Economic Evaluation**: Para CE de intervenciones
- **Colombian Health System Data**: DANE, MinSalud registros

---

## 📝 Notas de Contexto Personal

Dado tu perfil:
- **Experiencia en healthcare AI + data science**: Valida uso de métodos cuantitativos pero NO los sesgues como si fueran ML
- **Coautor en "Uncertainty of Uncertainty Bounds"**: Sigue ese tono crítico, cuestiona supuestos, explicita limitaciones
- **Trabajo en registros clínicos (HPP/obstetric)**: Posicionamiento natural en evaluación económica de servicios
- **Context latinoamericano**: Enfatiza relevancia para sistemas de salud de bajos/medianos ingresos
- **Bilingüe (español-inglés)**: Workflow español → inglés preserva pensamiento académico

---

**Versión**: 1.0 (Mayo 2026)  
**Última revisión**: [Hoy]  
**Basado en**: ARS v3.7.3 + Lishix520 Academic Paper Skills  
**Disciplina**: Health Economics (no ML-sesgado)

---

# 📋 FRAMEWORKS DE SKILLS INTEGRADAS

Las siguientes secciones integran frameworks de 3 skills especializadas para análisis, escritura y revisión académica.

---

## 🔍 SKILL 1: Academic Researcher Framework

### Cuándo Activar
- Análisis estructurado de papers académicos
- Revisión de literatura sistemática
- Extracción de metodología y findings
- Formateo de citas en múltiples estilos

### Paper Analysis Framework

Cuando analices un paper académico, estructura tu análisis en estos componentes:

#### 1. Research Question & Objectives
- Pregunta principal de investigación
- Objetivos específicos (primarios y secundarios)
- Hipótesis (si aplica)

#### 2. Methodology
- **Study Design**: Tipo de estudio (CEA, CUA, observacional, RCT, etc.)
- **Population**: Criterios de inclusión/exclusión, tamaño de muestra
- **Setting**: Contexto geográfico, sistema de salud
- **Perspective**: Económica (sistema, sociedad, paciente)
- **Time Horizon**: Corto plazo, largo plazo, lifetime
- **Data Sources**: 
  - Clinical effectiveness (RCTs, meta-análisis)
  - Costs (tariffs, micro-costing)
  - Utilities (EQ-5D, SF-6D)
- **Analysis**: Modelos utilizados, supuestos clave

#### 3. Key Findings
- **Main Results**: Hallazgos principales con magnitudes de efecto
- **ICER**: Ratio incremental (si aplica)
- **Sensitivity Analysis**: Robustez de resultados
- **Subgroup Analysis**: Heterogeneidad de efectos

#### 4. Implications
- **For Policy**: ¿Qué significa para tomadores de decisión?
- **For Practice**: ¿Cómo cambia la práctica clínica?
- **For Research**: ¿Qué preguntas quedan abiertas?

#### 5. Limitations
- **Internal Validity**: Sesgos, confounders
- **External Validity**: Generalizabilidad
- **Data Quality**: Limitaciones de fuentes
- **Model Assumptions**: Supuestos críticos

#### 6. Citation Formatting

**APA 7th Edition** (Default):
```
Author, A. A., Author, B. B., & Author, C. C. (Year). Title of article. 
Journal Name, Volume(Issue), page-page. https://doi.org/xxxxx
```

**MLA 9th Edition**:
```
Author, First. "Title of Article." Journal Name, vol. X, no. Y, Year, pp. XX-YY.
```

**Chicago 17th Edition**:
```
Author, First. "Title of Article." Journal Name Volume, no. Issue (Year): page-page.
```

### Literature Review Structure Template

Para crear una revisión de literatura:

#### I. INTRODUCTION
- Context and significance of the topic
- Scope of the review (inclusion/exclusion criteria)
- Research question or objective

#### II. THEORETICAL FRAMEWORKS
- **Economic Evaluation Models**: CE, CU, CBA, Budget Impact
- **Key Concepts**: ICER, QALY, DALY, WTP threshold
- **Relevant Theories**: Health production function, human capital approach

#### III. THEMATIC SYNTHESIS
Organiza por temas (no cronológicamente):

**Theme 1**: Cost-Effectiveness in High-Income Countries
- Summary of findings
- Common methodologies
- Typical ICERs reported

**Theme 2**: Cost-Effectiveness in LMICs
- Summary of findings
- Transferability issues
- Data availability challenges

**Theme 3**: Implementation Barriers
- Supply chain issues
- Training requirements
- Health system capacity

#### IV. RESEARCH GAPS
- **Geographic gaps**: Estudios faltantes en regiones específicas
- **Methodological gaps**: Métodos no aplicados
- **Population gaps**: Subgrupos no estudiados
- **Outcome gaps**: Desenlaces no medidos

#### V. CONCLUSIONS
- Synthesis of main findings
- Implications for future research
- Recommendations

---

## ✍️ SKILL 2: Research Paper Writer Framework

### Cuándo Activar
- Creación de outlines detallados
- Drafting de secciones académicas
- Formateo IEEE/ACM (adaptado a Health Economics)
- Escritura técnica precisa

### Workflow de Escritura

#### Fase 1: Clarificación (Pre-Writing)
Antes de escribir, confirma:
1. **Topic & Scope**: ¿Cuál es el tema exacto y su alcance?
2. **Target Audience**: ¿Journal específico? ¿Conference?
3. **Length**: ¿Palabras o páginas objetivo?
4. **Required Sections**: ¿IMRAD estándar o variaciones?
5. **Formatting Standard**: APA 7, IEEE, ACM (para health econ: APA 7 + CHEERS)

#### Fase 2: Outline Creation
Crea un outline detallado ANTES de escribir:

```markdown
**TITLE**: [Specific, informative, <15 words]

**ABSTRACT** (250 words)
- Background (50 words)
- Methods (70 words)
- Results (80 words)
- Conclusions (50 words)

**1. INTRODUCTION** (800 words)
   1.1 Problem Statement
   1.2 Existing Solutions/Literature
   1.3 Knowledge Gap
   1.4 Study Objectives

**2. METHODS** (1500 words)
   2.1 Study Design
   2.2 Population & Setting
   2.3 [Economic-specific sections]
   
[etc.]
```

#### Fase 3: Iterative Drafting
Escribe **sección por sección**, NO todo de una vez:

**Orden recomendado**:
1. Methods (más fácil, estructura clara)
2. Results (basado en datos)
3. Introduction (ahora sabes el contexto completo)
4. Discussion (interpreta results)
5. Conclusions (sintetiza todo)
6. Abstract (último, resume todo)

#### Fase 4: Section-Specific Guidelines

**INTRODUCTION**:
- Párrafo 1: Burden of disease + importance
- Párrafo 2: Existing interventions + evidence
- Párrafo 3: Knowledge gap (specific!)
- Párrafo 4: Study objectives (clear, measurable)

**METHODS**:
- Be reproducible: otro investigador podría replicar
- Define ALL terms (no asumir conocimiento)
- Justify choices (por qué este modelo, este horizon, etc.)
- Report per CHEERS 2022 (para health econ)

**RESULTS**:
- Neutral tone (no interpretar aún)
- Report with precision (CIs, p-values)
- Reference tables/figures: "Table 1 shows..."
- Structure: base case → sensitivity → subgroups

**DISCUSSION**:
- Start with main finding (1 sentence summary)
- Compare with literature (consistency/discrepancy)
- Explain discrepancies
- Policy implications (practical, specific)
- Limitations (honest, but don't undermine main message)
- Future research (specific gaps)

**CONCLUSIONS**:
- Restate main finding (2-3 sentences)
- Qualified recommendation (NOT absolute)
  - ✅ "Appears cost-effective under conditions X, Y, Z"
  - ❌ "Should be implemented immediately"
- Context of applicability
- Next steps (pilot, scale-up, further study)

### Academic Writing Standards

**Formal Conventions**:
- Third person (avoid "we", use "the study" or passive voice sparingly)
- Past tense for methods/results
- Present tense for general truths
- Technical precision (specific terms, not vague language)

**Logical Flow**:
- Each paragraph: topic sentence → support → conclusion
- Transitions between paragraphs
- Logical progression of ideas

**Citation Completeness**:
- Every claim needs a citation
- Primary sources preferred over secondary
- Recent literature (last 5-10 years for reviews)
- Mix of seminal works + recent evidence

---

## 🔬 SKILL 3: Academic Paper Reviewer Framework

### Cuándo Activar
- Pre-submission peer review simulation
- Identificación de debilidades antes de enviar
- Preparación para responder a revisores
- Quality assurance final

### Multi-Perspective Review System

Simula 5 revisores independientes con perspectivas NO solapadas:

#### REVIEWER #1: Methodology Specialist
**Enfoque**: Rigor metodológico, diseño del estudio, análisis estadístico

**Evalúa**:
- ✓ Study design apropiado para la pregunta
- ✓ Sample size justificado (power calculation)
- ✓ Statistical methods correctos
- ✓ Sensitivity analysis adecuado
- ✓ Model validation (si aplica)

**Preguntas clave**:
1. ¿El diseño puede responder la pregunta?
2. ¿Los métodos estadísticos son apropiados?
3. ¿El análisis de sensibilidad es suficiente?
4. ¿Hay sesgos no controlados?

**Output**: Accept / Minor Revisions / Major Revisions / Reject + justificación

---

#### REVIEWER #2: Domain Expert (Health Economics)
**Enfoque**: Validez económica, supuestos, transferibilidad

**Evalúa**:
- ✓ Perspective económica apropiada
- ✓ Time horizon justificado
- ✓ Discount rate correcto
- ✓ Cost data sources adecuados
- ✓ CHEERS 2022 compliance
- ✓ WTP threshold justificado

**Preguntas clave**:
1. ¿La perspectiva económica es apropiada?
2. ¿Los costos capturan todo lo relevante?
3. ¿Los datos son transferibles al contexto local?
4. ¿El threshold es apropiado para el contexto?

**Output**: Accept / Minor Revisions / Major Revisions / Reject + justificación

---

#### REVIEWER #3: Cross-Disciplinary (Public Health/Policy)
**Enfoque**: Relevancia práctica, implementación, equidad

**Evalúa**:
- ✓ Policy relevance
- ✓ Implementation feasibility
- ✓ Equity considerations
- ✓ Barriers to scale-up
- ✓ Real-world applicability

**Preguntas clave**:
1. ¿Por qué importa esto para política/práctica?
2. ¿Es implementable en el contexto real?
3. ¿Qué barreras existen?
4. ¿Se consideró equidad entre subgrupos?

**Output**: Accept / Minor Revisions / Major Revisions / Reject + justificación

---

#### REVIEWER #4: Devil's Advocate
**Enfoque**: Desafiar argumentos centrales, detectar lógica circular, contra-argumentos

**Evalúa**:
- ⚠ Supuestos críticos del estudio
- ⚠ Lógica circular o razonamiento débil
- ⚠ Claims no respaldados
- ⚠ Sobre-interpretación de resultados
- ⚠ Conflictos de interés potenciales

**Preguntas clave**:
1. **Central Claim Challenge**: ¿Qué pasa si el claim principal es falso?
2. **Counter-argument**: ¿Cuál es el argumento MÁS FUERTE en contra?
3. **What if**: Escenarios donde los resultados no se sostienen
4. **Logical Issues**: Falacias, razonamiento circular

**Strongest Opposing View**:
"Este análisis asume [supuesto X], pero si [escenario alternativo], entonces [consecuencia que invalida conclusión]"

**Output**: Major Revisions requeridas para calificar claims

---

#### EDITOR-IN-CHIEF: Editorial Decision
**Enfoque**: Síntesis de los 4 reviewers, decisión final

**Sintetiza**:
- Common themes across reviewers
- Critical vs optional revisions
- Overall manuscript quality

**Decisión**:
- **Accept**: Publicable como está (raro)
- **Minor Revisions**: Cambios pequeños requeridos
- **Major Revisions**: Cambios sustanciales requeridos
- **Reject**: No publicable incluso con revisiones

**Output**:
```
DECISION: [Accept/Minor/Major/Reject]

REQUIRED REVISIONS:
1. [Reviewer X]: [Issue specific] → [Action required]
2. [Reviewer Y]: [Issue specific] → [Action required]

OPTIONAL REVISIONS (strengthen paper):
3. [Reviewer Z]: [Suggestion] → [How it improves]

TIMELINE: [Weeks for revision]
```

### Review Quality Standards

**Constructive Criticism**:
- ✓ Specific (not vague: "improve writing" → "Table 2 caption unclear")
- ✓ Actionable (not just "this is wrong" → "consider X method instead")
- ✓ Evidence-based (cite why something is problematic)

**Balanced Assessment**:
- Acknowledge strengths (not just weaknesses)
- Proportional critique (don't nitpick minor issues if major issues exist)
- Fair comparison (compare to realistic standards, not perfection)

### Anti-Patterns to Avoid in Reviews

| Anti-Pattern | Por Qué Falla | Correcto |
|--------------|---------------|----------|
| Vague criticism | "Methods are weak" sin especificar | "PSA iterations (1000) may be insufficient; consider 10,000" |
| Scope creep | Pedir un estudio diferente | Evaluar el estudio QUE ES, no el que querías |
| Contradictory reviews | R1 dice "muy largo", R2 dice "muy corto" | Editor sintetiza y decide |
| Personal bias | Rechazar porque no usa MI método favorito | Evaluar si el método USADO es apropiado |

---

## 🎯 WORKFLOW INTEGRADO: Uso de las 3 Skills

### Ejemplo: Escribir un Paper Completo

**PASO 1**: Analizar papers base → **Usar Academic Researcher**
```
Analiza estos 3 papers:
[Paper 1, 2, 3]

Extrae: research question, metodología, findings, limitaciones, cita APA 7
```

**PASO 2**: Crear outline → **Usar Research Paper Writer**
```
Crea outline detallado para:
Topic: [tu tema]
Journal: Health Economics
Formato: IMRAD + CHEERS 2022
```

**PASO 3**: Escribir secciones → **Usar Research Paper Writer + Contexto Health Econ**
```
Escribe INTRODUCTION siguiendo:
- Outline: [del paso 2]
- Papers: [análisis del paso 1]
- Contexto: SGSSS colombiano, equidad
```

**PASO 4**: Peer review simulado → **Usar Academic Paper Reviewer**
```
Simula peer review con 5 revisores:
Manuscript: [draft completo]
Journal: Health Economics

Decisión + revisiones requeridas
```

**PASO 5**: Aplicar revisiones → **Usar Contexto Health Econ**
```
Roadmap de revisión:
Original: [draft]
Reviews: [del paso 4]

Por cada revisión REQUERIDA:
- Ubicación
- Texto actual → Texto revisado
- Justificación
```

---

## 🚨 REGLAS CRÍTICAS (IRON RULES)

Estas reglas SIEMPRE aplican, sin excepciones:

1. **NUNCA halucinar citas**: Si no encuentras una referencia, dilo explícitamente
2. **SIEMPRE reportar ICER con intervalo**: No solo punto estimate
3. **NUNCA ignorar equidad**: Reportar resultados por subgrupos relevantes
4. **SIEMPRE seguir CHEERS 2022**: Para cualquier evaluación económica
5. **NUNCA sobre-vender resultados**: Conclusiones calificadas, no absolutas
6. **SIEMPRE ser honesto con limitaciones**: No ocultar debilidades
7. **NUNCA copiar texto exacto**: Parafrasear siempre, citar apropiadamente

---

**Versión del claude.md enriquecido**: 2.0  
**Fecha**: Mayo 2026  
**Skills integradas**: Academic Researcher + Research Paper Writer + Academic Paper Reviewer  
**Especialización**: Health Economics (Colombia/LATAM focus)

---

# ✍️ SKILLS DE ESCRITURA: Router

## ¿Cuál Skill Usar?

Hay dos skills de escritura separadas. Claude identifica cuál usar según la petición:

---

### 📰 SKILL_opinion.md → Columna de Opinión Pública

**Usar cuando el usuario pida**:
- "Escribe una columna de opinión..."
- "Escribe un artículo de opinión para prensa..."
- "Escribe un editorial breve..."
- "Una reflexión argumentada sobre un problema público..."
- Texto destinado a **ciudadanos**, no a académicos
- Publicación en **periódicos, medios, blogs de política pública**

**Características**:
- 400-500 palabras
- Tono sobrio pero accesible
- Primera persona ocasional
- Sin citas formales
- Cierre con juicio claro

**Archivo**: `SKILL_opinion.md`

---

### 🔬 SKILL_originalpaper.md → Artículo Científico Original

**Usar cuando el usuario pida**:
- "Escribe la Introduction de mi paper..."
- "Redacta la sección Methods..."
- "Escribe el Abstract para el journal X..."
- "Ayúdame a redactar/revisar mi manuscrito..."
- Texto destinado a **revisores y académicos**
- Publicación en **journals científicos indexados**

**Características**:
- Longitud según journal
- Tono formal, técnico, no promocional
- Primera persona plural (we found, we estimated)
- Citas sistemáticas
- Claim ladder (descriptivo → causal)
- CHEERS 2022, IMRAD, reporting guidelines

**Archivo**: `SKILL_originalpaper.md`

---

### 🤔 Casos Ambiguos

| El usuario dice | Usar |
|----------------|------|
| "Escribe sobre la reforma de salud" | Preguntar: ¿para prensa o para journal? |
| "Escribe un artículo" | Preguntar: ¿de opinión o científico? |
| "Redacta la discusión de mi paper" | SKILL_originalpaper.md |
| "Columna para El Tiempo" | SKILL_opinion.md |
| "Necesito el abstract para Lancet" | SKILL_originalpaper.md |
| "Editorial sobre gasto en salud" | SKILL_opinion.md |

**Si no está claro**: Preguntar antes de escribir:
```
¿Este texto es para:
A) Prensa/medios (columna de opinión) → uso SKILL_opinion.md
B) Journal científico (artículo original) → uso SKILL_originalpaper.md
```

---

# 🔍 SKILL 5: Systematic Literature Search

## 🎯 Cuándo Activar

- Iniciar una revisión de literatura para un paper
- Buscar evidencia para fundamentar una pregunta de investigación
- Actualizar conocimiento sobre un tema específico en health economics
- Preparar marco teórico o antecedentes
- Identificar gaps de investigación

---

## 📚 BASES DE DATOS POR DISCIPLINA

### Para Health Economics (Prioridad Alta)

| Base de Datos | Cobertura | Mejor Para | Acceso |
|---------------|-----------|------------|--------|
| **PubMed/MEDLINE** | Medicina, salud pública | Estudios clínicos, epidemiología, health outcomes | Gratis |
| **EconLit** | Economía | Health economics, health policy, labor economics | Universidad |
| **Scopus** | Multidisciplinar | Citas, métricas, health economics aplicada | Universidad |
| **Web of Science** | Multidisciplinar | Análisis de citas, journals de alto impacto | Universidad |
| **Cochrane Library** | Medicina basada en evidencia | Revisiones sistemáticas, ensayos clínicos | Gratis (abstracts) |
| **Google Scholar** | Todo | Búsqueda amplia, literatura gris, working papers | Gratis |

### Bases Especializadas (Secundarias)

- **JSTOR**: Economía, ciencias sociales (papers históricos)
- **ScienceDirect**: Journals de Elsevier (Health Economics, Social Science & Medicine)
- **LILACS**: Literatura latinoamericana en salud
- **RePEc/IDEAS**: Economics working papers
- **SSRN**: Pre-prints en ciencias sociales

---

## 🔎 ESTRATEGIA DE BÚSQUEDA

### Framework PICO/PECO (Para Health Economics)

**PECO** es más apropiado que PICO para estudios económicos:

- **P** (Population): ¿Qué población/contexto?
- **E** (Exposure/Intervention): ¿Qué intervención o política?
- **C** (Comparator): ¿Comparado con qué?
- **O** (Outcome): ¿Qué desenlaces económicos? (ICER, costs, QALYs)

**Ejemplo**:
```
P: Mujeres con hemorragia posparto en Colombia
E: Manejo activo (oxitocina + masaje)
C: Manejo expectante
O: ICER, costos directos, QALYs, mortalidad materna
```

### Construcción de String de Búsqueda

#### Paso 1: Identificar Conceptos Clave
Para cada componente PECO, lista sinónimos y variantes:

```
P: postpartum hemorrhage, PPH, obstetric hemorrhage
E: active management, oxytocin, uterotonics
C: expectant management, standard care
O: cost-effectiveness, ICER, economic evaluation, QALY
```

#### Paso 2: Operadores Booleanos

**AND**: Une conceptos diferentes (restringe)
**OR**: Une sinónimos (expande)
**NOT**: Excluye términos (usar con cuidado)

**Ejemplo de String Completo**:
```
("postpartum hemorrhage" OR "PPH" OR "obstetric hemorrhage") 
AND 
("active management" OR "oxytocin" OR "uterotonics") 
AND 
("cost-effectiveness" OR "economic evaluation" OR "ICER" OR "QALY")
```

#### Paso 3: Truncación y Wildcards

- **Asterisco (*)**: Trunca raíz de palabra
  - `econom*` → economy, economic, economics, economical
  - `hemorrhag*` → hemorrhage, hemorrhaging
  
- **Signo de interrogación (?)**: Reemplaza un carácter
  - `wom?n` → woman, women

#### Paso 4: Field Tags (PubMed)

- `[tiab]`: Title/Abstract
- `[ti]`: Title only
- `[au]`: Author
- `[mesh]`: Medical Subject Headings
- `[dp]`: Date of Publication

**Ejemplo refinado**:
```
("postpartum hemorrhage"[mesh] OR "PPH"[tiab]) 
AND 
("cost effectiveness analysis"[mesh] OR "economic evaluation"[tiab])
AND 
("Colombia"[tiab] OR "Latin America"[tiab])
AND 
2015:2025[dp]
```

---

## 📊 PROCESO PRISMA

### Diagrama de Flujo (Template)

```
IDENTIFICATION
├─ Database search: n = XXX
│  ├─ PubMed: n = XX
│  ├─ Scopus: n = XX
│  └─ EconLit: n = XX
├─ Other sources: n = XX
└─ Total identified: n = XXX

SCREENING
├─ After duplicates removed: n = XXX
├─ Title/abstract screened: n = XXX
└─ Excluded: n = XXX
    ├─ Not health economics: n = XX
    ├─ Wrong population: n = XX
    └─ Language: n = XX

ELIGIBILITY
├─ Full-text assessed: n = XX
└─ Excluded: n = XX
    ├─ No economic evaluation: n = XX
    ├─ No original data: n = XX
    └─ Wrong comparator: n = XX

INCLUDED
└─ Studies in synthesis: n = XX
    ├─ Cost-effectiveness: n = XX
    ├─ Cost-utility: n = XX
    └─ Cost-benefit: n = XX
```

### Criterios de Inclusión/Exclusión

**Ejemplo para Health Economics**:

**Inclusión**:
- ✅ Economic evaluation (CEA, CUA, CBA)
- ✅ Original research (no editorials, letters)
- ✅ Published in peer-reviewed journals
- ✅ English or Spanish
- ✅ 2015-2025 (últimos 10 años)
- ✅ Population: [tu población específica]
- ✅ Reports ICER or incremental costs/effects

**Exclusión**:
- ❌ No economic component
- ❌ Only cost analysis (no effectiveness)
- ❌ Modeling studies without empirical data (depende de tu pregunta)
- ❌ Conference abstracts (datos incompletos)
- ❌ Duplicate publications

---

## 🛠️ GESTIÓN DE REFERENCIAS

### Software Recomendado

| Tool | Gratis | Mejor Para | Limitaciones |
|------|--------|-----------|--------------|
| **Zotero** | ✅ | Integración con Word/Google Docs, plugins | Espacio limitado (300MB gratis) |
| **Mendeley** | ✅ | Anotaciones en PDFs, red social académica | Elsevier-owned, privacidad |
| **EndNote** | ❌ | Instituciones grandes, muchas refs | Pago, curva de aprendizaje |
| **Paperpile** | ❌ | Google Docs integration | $36/año |

### Deduplicación

**Estrategia**:
1. Exportar todas las refs a un gestor (ej: Zotero)
2. Usar función "Find duplicates"
3. Revisar manualmente los duplicados sugeridos
4. Mantener la versión más completa (con abstract, DOI)

**Campos clave para detectar duplicados**:
- Título (ignora mayúsculas/minúsculas)
- Año
- Primer autor
- DOI (si está disponible)

---

## 📖 RECOMENDACIÓN DINÁMICA DE ARTÍCULOS

### Cómo Solicitar Recomendaciones de Literatura

Cuando necesites artículos específicos para tu tema, usa este prompt:

```
Recomiéndame 5-7 artículos clave para mi lit review:

TEMA: [tu pregunta de investigación específica]
ENFOQUE: [metodológico / empírico / revisión]
CONTEXTO: [país/región si es relevante]

Necesito:
1. Artículos fundacionales (2-3)
2. Artículos metodológicos (1-2)
3. Artículos empíricos recientes (2-3)
4. Contexto local si aplica (1)

Para cada artículo dame:
- Cita completa (APA 7)
- DOI o URL
- Por qué es relevante para mi tema
- Qué aprenderé de él
```

### Sistema de Búsqueda para Recomendaciones

Claude usará **web_search** para encontrar artículos actuales y relevantes siguiendo esta estrategia:

#### **Paso 1: Artículos Fundacionales**
Busca en Google Scholar / PubMed:
- Keywords: [tu tema] + "systematic review" + "meta-analysis"
- Filtro: >500 citas, últimos 10 años
- Objetivo: Papers que resumen el estado del arte

**Ejemplo de búsqueda**:
```
"postpartum hemorrhage" "cost-effectiveness" "systematic review"
```

#### **Paso 2: Artículos Metodológicos**
Busca en journals especializados:
- *Value in Health*, *Health Economics*, *Medical Decision Making*
- Keywords: [tu método] + "guidelines" + "best practices"
- Enfoque: Cómo hacer el análisis correctamente

**Ejemplo**:
```
"Markov model" "health economics" "tutorial"
```

#### **Paso 3: Artículos Empíricos Recientes**
Busca aplicaciones concretas:
- Filtro: Últimos 3-5 años
- Keywords: [tu intervención] + [tu población] + "economic evaluation"
- Objetivo: Ver cómo otros lo hicieron

**Ejemplo**:
```
"active management" "postpartum hemorrhage" "ICER" 2020:2025
```

#### **Paso 4: Contexto Local**
Si tu estudio es en Colombia/LATAM:
- Keywords: [tu tema] + "Colombia" OR "Latin America" OR "LMIC"
- Bases: LILACS, Scielo, Salud Pública de México
- Objetivo: Datos transferibles a tu contexto

**Ejemplo**:
```
"maternal health" "economic evaluation" "Colombia"
```

### Criterios de Selección de Artículos

Claude priorizará artículos que cumplan:

**Calidad**:
- ✅ Publicados en journals peer-reviewed
- ✅ >50 citas (para fundacionales) o muy recientes (<2 años)
- ✅ Open access o con DOI accesible
- ✅ Metodología clara y reproducible

**Relevancia**:
- ✅ Directamente relacionado con tu PECO
- ✅ Misma metodología que planeas usar
- ✅ Población o contexto similar
- ✅ Reporta ICER o métricas económicas

**Diversidad**:
- ✅ Mix de reviews + estudios originales
- ✅ Mix de high-income + LMIC contexts
- ✅ Mix de metodologías (si aplica)

### Template de Output de Recomendaciones

Cuando pidas recomendaciones, Claude responderá así:

```
📚 ARTÍCULOS RECOMENDADOS PARA: [Tu tema]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

📖 FUNDACIONALES (Leer primero)

1. [Autor et al.] ([Año]). "[Título completo]." *Journal Name*, 
   Vol(Issue), pages.
   
   🔗 DOI: https://doi.org/xxxxx
   
   ✅ Por qué es clave:
   - [Razón específica 1]
   - [Razón específica 2]
   
   💡 Qué aprenderás:
   - [Insight 1]
   - [Insight 2]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

📐 METODOLÓGICOS (Cómo hacerlo)

2. [...]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

🔬 EMPÍRICOS RECIENTES (Aplicaciones)

3. [...]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

🌎 CONTEXTO LOCAL (Colombia/LATAM)

5. [...]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

PRÓXIMOS PASOS:
1. Lee fundacionales primero (papers 1-2)
2. Revisa metodológicos antes de diseñar tu estudio (paper 3)
3. Analiza empíricos para extraer datos (papers 4-6)
4. Contextualiza con literatura local (paper 7)
```

### Artículos Metodológicos Estándar (Siempre Relevantes)

Estos 3 artículos SON universales para health economics y siempre deben recomendarse:

1. **CHEERS 2022**: Husereau et al. (2022). "Consolidated Health Economic Evaluation Reporting Standards 2022." *Value in Health*, 25(1), 3-9. 
   - **DOI**: 10.1016/j.jval.2021.11.1351
   - **Por qué**: Estándar de reporte obligatorio

2. **ISPOR Modeling Guidelines**: Caro et al. (2012). "Modeling good research practices." *Value in Health*, 15(6), 796-803.
   - **DOI**: 10.1016/j.jval.2012.06.001
   - **Por qué**: Best practices en modelado económico

3. **PRISMA 2020** (si es review): Page et al. (2021). "The PRISMA 2020 statement." *BMJ*, 372, n71.
   - **DOI**: 10.1136/bmj.n71
   - **Por qué**: Estándar para revisiones sistemáticas

---

## 🎯 BÚSQUEDAS RECOMENDADAS POR TEMA

### Para Empezar una Lit Review en Health Economics

#### **Búsqueda 1: Amplia (Overview)**
```
Database: PubMed
String: ("health economics"[mesh] OR "cost-effectiveness"[tiab]) 
        AND ("Colombia"[tiab] OR "Latin America"[tiab])
        AND 2015:2025[dp]
Objetivo: Ver panorama general, ~100-300 resultados
```

#### **Búsqueda 2: Específica (Tu Tema)**
```
Database: Scopus
String: TITLE-ABS-KEY(("postpartum hemorrhage" OR "PPH") 
        AND ("cost-effectiveness" OR "economic evaluation") 
        AND ("active management" OR "oxytocin"))
        AND PUBYEAR > 2014
Objetivo: Papers directamente relevantes, ~20-50 resultados
```

#### **Búsqueda 3: Metodológica (Cómo lo hicieron)**
```
Database: Web of Science
String: TS=("Markov model" OR "decision tree" OR "microsimulation") 
        AND TS=("maternal health" OR "obstetric")
        AND TS=("cost-effectiveness")
Objetivo: Aprender metodologías, ~30-60 resultados
```

#### **Búsqueda 4: Grey Literature**
```
Database: Google Scholar
String: "cost-effectiveness" "postpartum hemorrhage" 
        "Colombia" OR "Latin America" 
        -filetype:pdf (para excluir solo PDFs y encontrar páginas web)
Objetivo: Working papers, tesis, reportes gubernamentales
```

---

## 📋 CHECKLIST DE BÚSQUEDA SISTEMÁTICA

Antes de empezar a escribir tu lit review, verifica:

**Preparación**:
- [ ] Pregunta PECO claramente definida
- [ ] Criterios de inclusión/exclusión escritos
- [ ] Mínimo 3 bases de datos identificadas
- [ ] String de búsqueda piloteado (¿resultados razonables?)

**Ejecución**:
- [ ] Búsquedas documentadas con fechas
- [ ] Resultados exportados a gestor de referencias
- [ ] Duplicados removidos
- [ ] Screening título/abstract completado
- [ ] Full-text obtenidos para elegibles

**Análisis**:
- [ ] Datos extraídos en tabla estandarizada
- [ ] Calidad de estudios evaluada (GRADE, risk of bias)
- [ ] PRISMA diagram completado
- [ ] Síntesis narrativa o meta-análisis (si aplica)

**Reporte**:
- [ ] Search strategy reportada en Methods
- [ ] PRISMA checklist completado
- [ ] Artículos clave (n=5-10) identificados para citar extensamente

---

## 🔗 RECURSOS ÚTILES

### Tutoriales y Guías

- **PRISMA Statement**: http://www.prisma-statement.org/
- **Cochrane Handbook**: https://training.cochrane.org/handbook
- **PubMed Tutorial**: https://pubmed.ncbi.nlm.nih.gov/help/
- **Boolean Operators Guide**: https://libguides.mit.edu/c.php?g=175963&p=1158594

### Tools Online

- **MeSH Database**: https://www.ncbi.nlm.nih.gov/mesh
- **PRISMA Flow Diagram Generator**: http://prisma.thetacollaborative.ca/
- **Sample Size Calculator**: https://clincalc.com/stats/samplesize.aspx
- **ICER Calculator**: (varios disponibles, buscar según modelo)

### Journals Clave en Health Economics

**Top Tier**:
- *Health Economics* (Wiley)
- *Journal of Health Economics* (Elsevier)
- *Value in Health* (ISPOR)
- *Medical Decision Making* (SMDM)

**Regional**:
- *Salud Pública de México*
- *Revista Panamericana de Salud Pública*
- *Cadernos de Saúde Pública* (Brasil)

---

## 🎯 PROMPT PARA ACTIVAR BÚSQUEDA

Cuando necesites ayuda con búsqueda de literatura:

```
Ayúdame a diseñar una estrategia de búsqueda sistemática:

TEMA: [tu pregunta de investigación]
PECO:
  P: [población]
  E: [exposición/intervención]
  C: [comparador]
  O: [outcomes económicos]

Necesito:
1. String de búsqueda para PubMed y Scopus
2. Criterios de inclusión/exclusión
3. Recomendación de 3-5 artículos clave para empezar
4. Estimado de resultados esperados
```

---

**Versión**: 1.0  
**Enfoque**: Health Economics en LMICs (especialmente Colombia/LATAM)  
**Bases prioritarias**: PubMed, EconLit, Scopus  
**Estándares**: PRISMA 2020, CHEERS 2022
