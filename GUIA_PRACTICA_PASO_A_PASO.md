# 🎯 GUÍA PRÁCTICA: De Idea a Paper Publicable

**Para usar desde claude.chat (sin Claude Code)**

---

## 📌 TU SITUACIÓN

Tienes:
- ✅ Una **idea de investigación** en economía de la salud
- ✅ 2-3 **papers base** que te inspiran o fundamentan tu idea
- ❌ No tienes el paper escrito aún

Quieres:
- 🎯 Un **paper completo** listo para enviar a un journal
- 🎯 Siguiendo estándares académicos (CHEERS 2022, APA 7)
- 🎯 Con revisión simulada de pares

---

## 🚀 PASO A PASO (10 Pasos)

---

# PASO 1: Refina tu Pregunta de Investigación

## ¿Qué hacer?
Convierte tu idea vaga en una pregunta de investigación clara y específica.

## Comando en claude.chat:

```
Tengo una idea de investigación en economía de la salud:

IDEA: [Describe tu idea en 1-2 oraciones]

Ejemplo: "Quiero evaluar si el manejo activo de hemorragia posparto 
es costo-efectivo en Colombia"

Ayúdame a refinar esta idea usando un diálogo socrático que cubra:
1. Carga de enfermedad (magnitud del problema)
2. Intervenciones existentes (qué se hace ahora)
3. Contexto del sistema de salud (perspectiva económica)
4. Brecha de conocimiento (qué falta en la literatura)
5. Relevancia para política (por qué importa)

Al final, dame:
- Pregunta de investigación clara y específica
- Objetivos del estudio (3-4 puntos)
```

## Qué recibirás:
✅ Pregunta de investigación refinada  
✅ Objetivos específicos  
✅ Contexto claro para tu paper

## Guardar:
📝 Copia este output en un documento: `01_research_question.md`

---

# PASO 2: Analiza tus Papers Base

## ¿Qué hacer?
Extrae información clave de los 2-3 papers que fundamentan tu idea.

## Comando en claude.chat (PARA CADA PAPER):

```
Analiza este paper científico siguiendo este framework:

PAPER: [Sube el PDF o pega el título/autores]

Extrae:
1. Research question principal
2. Metodología (diseño, población, perspectiva, horizonte temporal)
3. Findings principales (ICER, costos, efectividad)
4. Implicaciones para política
5. Limitaciones del estudio
6. Cita completa en APA 7

Formato de salida: Estructurado, conciso, máximo 300 palabras por paper
```

## Qué recibirás:
✅ Análisis estructurado de cada paper  
✅ Citas en APA 7 listas para usar  
✅ Identificación de gaps y limitaciones

## Guardar:
📝 Compila los análisis en: `02_papers_analysis.md`

---

# PASO 3: Crea la Estructura de tu Literatura Review

## ¿Qué hacer?
Diseña la estructura de tu revisión de literatura antes de escribirla.

## Comando en claude.chat:

```
Crea una estructura de literatura review para:

TEMA: [Tu pregunta de investigación del Paso 1]

PAPERS BASE: [Pega el análisis del Paso 2]

La estructura debe incluir:
1. Introduction (contexto y alcance)
2. Theoretical frameworks (modelos de evaluación económica: CE, CU)
3. Thematic synthesis
   - Tema 1: Costo-efectividad en países de altos ingresos
   - Tema 2: [Tu tema específico]
   - Tema 3: Barreras de implementación
4. Research gaps (qué falta específicamente para Colombia/tu contexto)
5. Conclusions

IMPORTANTE: Personaliza para economía de la salud con:
- Perspectiva del sistema de salud (SGSSS si es Colombia)
- Énfasis en equidad (rural vs urbano, por ejemplo)
- Transferibilidad de evidencia internacional
- Vocabulario CHEERS 2022 (ICER, QALY, WTP)
```

## Qué recibirás:
✅ Outline detallado de tu literatura review  
✅ Secciones temáticas organizadas  
✅ Gaps de investigación identificados

## Guardar:
📝 Guarda como: `03_lit_review_outline.md`

---

# PASO 4: Escribe tu Literatura Review

## ¿Qué hacer?
Convierte el outline del Paso 3 en prosa académica completa.

## Comando en claude.chat:

```
Escribe la literatura review completa basándote en:

OUTLINE: [Pega el outline del Paso 3]
PAPERS ANALIZADOS: [Pega análisis del Paso 2]
PREGUNTA DE INVESTIGACIÓN: [Del Paso 1]

Requisitos de escritura:
- Máximo 3-4 oraciones por párrafo
- Una idea principal por párrafo
- Vocabulario económico consistente (ICER, QALY, DALY, perspectiva económica)
- Citas en APA 7
- Tono formal pero accesible
- La brecha de investigación debe quedar CLARA al final

Longitud objetivo: 1500-2000 palabras (4-5 páginas)
```

## Qué recibirás:
✅ Literatura review completa en prosa  
✅ 4-5 páginas con estructura clara  
✅ Brecha de investigación bien definida

## Guardar:
📝 Guarda como: `04_literature_review.md`

---

# PASO 5: Crea el Outline Completo de tu Paper

## ¿Qué hacer?
Diseña la estructura COMPLETA de tu paper antes de escribirlo.

## Comando en claude.chat:

```
Crea un outline detallado para mi paper de economía de la salud:

PREGUNTA: [Tu pregunta de investigación del Paso 1]
TARGET JOURNAL: Health Economics (o el journal que elijas)
FORMATO: IMRAD + Health Economics (APA 7, CHEERS 2022)
LONGITUD: 6000 palabras

El outline debe incluir:

**Title**
**Abstract** (250 palabras)
  - Background
  - Methods
  - Results  
  - Conclusions

**1. INTRODUCTION** (~800 palabras)
   1.1 Carga de enfermedad en [tu contexto]
   1.2 Intervenciones existentes + evidencia internacional
   1.3 Brecha de conocimiento (específica a tu contexto)
   1.4 Objetivos del estudio

**2. METHODS** (~1500 palabras)
   2.1 Study design (CEA/CUA/CBA)
   2.2 Population and setting
   2.3 Perspective (sistema de salud, sociedad)
   2.4 Interventions compared
   2.5 Model structure (árbol de decisión, Markov, etc.)
   2.6 Data sources (efectividad, costos, utilidades)
   2.7 Time horizon
   2.8 Discount rate
   2.9 Sensitivity analysis
   2.10 Equity analysis (subgrupos)

**3. RESULTS** (~1200 palabras)
   3.1 Base case analysis
   3.2 Cost breakdown
   3.3 Effectiveness outcomes
   3.4 ICER calculation
   3.5 Sensitivity analysis
   3.6 Subgroup analysis (equidad)

**4. DISCUSSION** (~1200 palabras)
   4.1 Main findings vs literatura
   4.2 Policy implications
   4.3 Equity considerations
   4.4 Transferability
   4.5 Limitations
   4.6 Future research

**5. CONCLUSIONS** (~300 palabras)
**REFERENCES** (APA 7)
**APPENDICES** (CHEERS 2022 Checklist)

IMPORTANTE: Incluye notas específicas sobre:
- Qué datos necesito en cada sección
- Qué vocabulario técnico usar
- Qué estándares seguir (CHEERS 2022)
```

## Qué recibirás:
✅ Outline detallado sección por sección  
✅ Guía de contenido para cada parte  
✅ Estructura lista para seguir

## Guardar:
📝 Guarda como: `05_paper_outline.md`

---

# PASO 6: Escribe la INTRODUCTION

## ¿Qué hacer?
Escribe la primera sección completa de tu paper.

## Comando en claude.chat:

```
Escribe la INTRODUCTION completa de mi paper basándote en:

OUTLINE: [Pega sección 1 del outline del Paso 5]
LITERATURA: [Pega tu lit review del Paso 4]
PREGUNTA DE INVESTIGACIÓN: [Del Paso 1]

Estructura exacta (4 párrafos):
- Párrafo 1: Importancia del problema + carga de enfermedad con datos
- Párrafo 2: Intervenciones existentes + evidencia de costo-efectividad internacional
- Párrafo 3: Brecha de conocimiento (por qué tu contexto es diferente)
- Párrafo 4: Objetivos específicos de tu estudio

Requisitos:
- Máximo 3-4 oraciones por párrafo
- Citas en APA 7
- Énfasis en equidad (disparidades geográficas/socioeconómicas)
- Tono crítico (no sobre-vender la evidencia existente)
- Contexto específico [SGSSS colombiano / tu sistema de salud]

Longitud: ~800 palabras
```

## Qué recibirás:
✅ Introduction completa lista para usar  
✅ ~800 palabras en 4 párrafos  
✅ Con citas y contexto apropiado

## Guardar:
📝 Guarda como: `06_introduction.md`

---

# PASO 7: Escribe los METHODS

## ¿Qué hacer?
Escribe la sección de metodología con rigor técnico.

## Comando en claude.chat:

```
Escribe la sección METHODS completa de mi paper:

OUTLINE: [Pega sección 2 del outline del Paso 5]
TIPO DE ANÁLISIS: [Costo-efectividad / Costo-utilidad / etc.]

Subsecciones requeridas:
2.1 Study design
2.2 Population and setting
2.3 Economic perspective (sistema de salud, sociedad)
2.4 Interventions compared
2.5 Model structure (describe el modelo económico)
2.6 Data sources
    - Clinical effectiveness: [cita tus papers base]
    - Costs: [fuentes de costos locales]
    - Utilities: [si aplica, ej: EQ-5D]
2.7 Time horizon (justifica la elección)
2.8 Discount rate (justifica según guidelines locales)
2.9 Sensitivity analysis (one-way, probabilistic)
2.10 Equity analysis (subgrupos por región/nivel socioeconómico)

IMPORTANTE: 
- Debe ser REPRODUCIBLE (otro investigador podría replicar)
- Seguir CHEERS 2022 guidelines
- Explicar cada supuesto del modelo
- Tono: técnico, preciso, formal

Longitud: ~1500 palabras
```

## Qué recibirás:
✅ Methods completo y técnicamente riguroso  
✅ ~1500 palabras  
✅ CHEERS 2022 compliant

## Guardar:
📝 Guarda como: `07_methods.md`

---

# PASO 8: Escribe RESULTS

## ¿Qué hacer?
Presenta tus hallazgos (o resultados esperados si es propuesta).

## Comando en claude.chat:

```
Escribe la sección RESULTS de mi paper:

OUTLINE: [Pega sección 3 del outline del Paso 5]
TIPO DE ANÁLISIS: [Tu tipo de análisis económico]

Subsecciones:
3.1 Base case analysis
    - ICER principal: [valor] per QALY/DALY
    - Costos: Intervención vs Comparador
    - Effectiveness: [medida principal]

3.2 Cost breakdown
    - Costos directos médicos
    - Costos por categoría (hospitalización, medicamentos, etc.)

3.3 Effectiveness outcomes
    - QALYs ganados / DALYs evitados
    - Efectos clínicos

3.4 ICER calculation
    - Incremental costs
    - Incremental effects
    - ICER = ΔC / ΔE

3.5 Sensitivity analysis
    - One-way: Parámetros críticos
    - Probabilistic: Uncertainty
    - Tornado diagram / Cost-effectiveness plane

3.6 Subgroup analysis (equidad)
    - ICER por región (rural vs urbano)
    - ICER por nivel socioeconómico

IMPORTANTE:
- Reportar con intervalos de confianza
- Ser neutral (solo presentar datos, no interpretar aún)
- Mencionar tablas y figuras (ej: "Table 1 shows...")

Longitud: ~1200 palabras
```

## Qué recibirás:
✅ Results estructurado y completo  
✅ ~1200 palabras  
✅ Presentación neutral de hallazgos

## Guardar:
📝 Guarda como: `08_results.md`

---

# PASO 9: Escribe DISCUSSION

## ¿Qué hacer?
Interpreta los resultados y discute implicaciones.

## Comando en claude.chat:

```
Escribe la sección DISCUSSION de mi paper:

OUTLINE: [Pega sección 4 del outline del Paso 5]
RESULTS: [Resumen de tus hallazgos del Paso 8]
LITERATURA: [Tus papers base del Paso 2]

Subsecciones:
4.1 Main findings vs literatura
    - ¿Cómo se comparan tus resultados con evidencia internacional?
    - ¿Por qué son similares/diferentes?

4.2 Policy implications
    - ¿Qué significa esto para tomadores de decisión?
    - ¿Es costo-efectivo bajo qué condiciones?
    - ¿Cuál es el siguiente paso para implementación?

4.3 Equity considerations
    - ¿Cómo varían los resultados entre subgrupos?
    - ¿Qué implica esto para equidad en salud?

4.4 Transferability
    - ¿Qué tan aplicables son estos resultados a otros contextos?
    - ¿Qué supuestos limitan la generalización?

4.5 Limitations
    - Data quality
    - Model assumptions
    - External validity
    **SÉ HONESTO: No ocultar limitaciones**

4.6 Future research
    - ¿Qué preguntas quedan sin responder?
    - ¿Qué estudios se necesitan?

IMPORTANTE:
- Tono crítico pero constructivo
- Reconocer limitaciones sin debilitar el mensaje principal
- Vincular todo de vuelta a la pregunta de investigación original

Longitud: ~1200 palabras
```

## Qué recibirás:
✅ Discussion completa con análisis crítico  
✅ ~1200 palabras  
✅ Limitaciones honestas + implicaciones claras

## Guardar:
📝 Guarda como: `09_discussion.md`

---

# PASO 10: Escribe CONCLUSIONS

## ¿Qué hacer?
Resume hallazgos y da recomendación final (con caveats).

## Comando en claude.chat:

```
Escribe la sección CONCLUSIONS de mi paper:

PREGUNTA DE INVESTIGACIÓN: [Del Paso 1]
HALLAZGOS PRINCIPALES: [Del Paso 8]
LIMITACIONES: [Del Paso 9]

La conclusión debe:
1. Resumir hallazgo principal en 2-3 oraciones
2. Dar recomendación CALIFICADA (no absoluta)
   - Ejemplo: "La intervención parece costo-efectiva BAJO LAS SIGUIENTES CONDICIONES..."
   - NO: "La intervención debe implementarse inmediatamente"
3. Mencionar contexto específico de aplicabilidad
4. Cerrar con llamado a acción (siguiente paso: piloto, más estudios, etc.)

IMPORTANTE:
- NO sobre-vender los hallazgos
- Ser honesto sobre incertidumbres
- Dar recomendación práctica pero calificada

Longitud: ~300 palabras (máximo 1 página)
```

## Qué recibirás:
✅ Conclusions concisas y honestas  
✅ ~300 palabras  
✅ Recomendación calificada apropiada

## Guardar:
📝 Guarda como: `10_conclusions.md`

---

# PASO 11: Crea el ABSTRACT

## ¿Qué hacer?
Resume todo el paper en 250 palabras.

## Comando en claude.chat:

```
Escribe el ABSTRACT de mi paper siguiendo estructura estándar:

INTRODUCTION: [Del Paso 6]
METHODS: [Del Paso 7]
RESULTS: [Del Paso 8]
CONCLUSIONS: [Del Paso 10]

Estructura del Abstract (4 párrafos, máx 250 palabras):

**Background** (40-50 palabras)
- Carga de enfermedad
- Brecha de conocimiento
- Objetivo del estudio

**Methods** (60-70 palabras)
- Diseño del estudio
- Población
- Perspectiva económica
- Horizonte temporal
- Fuentes de datos principales

**Results** (70-80 palabras)
- ICER principal
- Costos incrementales
- Efectividad incremental
- Resultado de análisis de sensibilidad
- Hallazgo de equidad (si relevante)

**Conclusions** (40-50 palabras)
- Interpretación del ICER (¿costo-efectivo?)
- Recomendación calificada
- Contexto de aplicabilidad

IMPORTANTE:
- Máximo 250 palabras TOTALES
- Sin citas en el abstract
- Auto-contenido (se puede leer sin el paper)
- Métodos económicos claros (ej: "cost-effectiveness analysis with ICER")
```

## Qué recibirás:
✅ Abstract completo de 250 palabras  
✅ Estructura estándar de 4 párrafos  
✅ Auto-contenido y claro

## Guardar:
📝 Guarda como: `11_abstract.md`

---

# PASO 12: Combina Todo en Manuscrito Completo

## ¿Qué hacer?
Une todas las secciones en un solo documento.

## Comando en claude.chat:

```
Combina todas las secciones en un manuscrito completo:

ABSTRACT: [Del Paso 11]
INTRODUCTION: [Del Paso 6]
METHODS: [Del Paso 7]
RESULTS: [Del Paso 8]
DISCUSSION: [Del Paso 9]
CONCLUSIONS: [Del Paso 10]
REFERENCES: [Compila todas las citas de los pasos anteriores]

Formato final:
- Título en la primera página
- Abstract en página separada
- Secciones numeradas (1. INTRODUCTION, 2. METHODS, etc.)
- Referencias en APA 7 al final
- Transiciones suaves entre secciones

Genera el manuscrito completo en formato Markdown listo para:
1. Copiar a Word
2. Convertir a PDF
3. Enviar a journal
```

## Qué recibirás:
✅ Manuscrito completo de ~6000 palabras  
✅ Todas las secciones integradas  
✅ Listo para formateo final

## Guardar:
📝 Guarda como: `12_manuscript_complete.md`

---

# PASO 13: Simulación de Peer Review

## ¿Qué hacer?
Obtén feedback crítico ANTES de enviar a un journal real.

## Comando en claude.chat:

```
Simula una revisión de pares (peer review) de mi manuscrito.

MANUSCRIPT: [Pega tu manuscrito completo del Paso 12]
TARGET JOURNAL: Health Economics
PAPER TYPE: Cost-effectiveness analysis

Necesito que simules 5 revisores independientes:

**REVIEWER #1: Methodology Specialist**
- Evalúa diseño del estudio
- Valida métodos económicos
- Revisa análisis de sensibilidad
- Da recomendación: Accept / Minor Revisions / Major Revisions / Reject

**REVIEWER #2: Domain Expert (Health Economics)**
- Evalúa relevancia de pregunta de investigación
- Valida supuestos económicos
- Revisa transferibilidad de datos
- Da recomendación

**REVIEWER #3: Cross-Disciplinary (Public Health)**
- Evalúa relevancia para política
- Valida equidad en análisis
- Revisa barreras de implementación
- Da recomendación

**REVIEWER #4: Devil's Advocate**
- Desafía argumentos principales
- Identifica lógica circular
- Propone contra-argumentos más fuertes
- Da recomendación

**EDITOR-IN-CHIEF:**
- Sintetiza las 4 reviews
- Da decisión editorial final
- Lista revisiones REQUERIDAS
- Lista revisiones OPCIONALES

IMPORTANTE: Sé CRÍTICO pero constructivo.
```

## Qué recibirás:
✅ 5 reviews independientes completas  
✅ Decisión editorial (Accept/Revise/Reject)  
✅ Lista clara de cambios requeridos

## Guardar:
📝 Guarda como: `13_peer_reviews.md`

---

# PASO 14: Aplicar Revisiones

## ¿Qué hacer?
Mejora tu manuscrito basándote en el feedback del Paso 13.

## Comando en claude.chat:

```
Ayúdame a revisar mi manuscrito basándome en peer reviews.

MANUSCRIPT ORIGINAL: [Del Paso 12]
PEER REVIEWS: [Del Paso 13]

Por cada revisión REQUERIDA:
1. Identifica la ubicación exacta en el manuscrito (sección, línea)
2. Muestra el texto ACTUAL
3. Propone el texto REVISADO
4. Explica el cambio

Enfócate primero en:
- Revisiones del Reviewer #1 (metodología)
- Revisiones del Reviewer #2 (economía de la salud)
- Revisiones del Reviewer #4 (calificación de claims)

Dame un "Revision Roadmap" paso a paso.
```

## Qué recibirás:
✅ Roadmap de revisión claro  
✅ Texto actual vs texto revisado  
✅ Justificación de cada cambio

## Guardar:
📝 Guarda como: `14_revision_roadmap.md`

---

# PASO 15: Manuscrito Final Revisado

## ¿Qué hacer?
Genera la versión final incorporando todas las revisiones.

## Comando en claude.chat:

```
Genera el manuscrito FINAL incorporando todas las revisiones:

MANUSCRIPT ORIGINAL: [Del Paso 12]
REVISION ROADMAP: [Del Paso 14]

Aplica TODOS los cambios sugeridos y genera:
- Manuscrito completo revisado
- Track changes (qué se cambió en cada sección)
- Response to reviewers (carta explicando cómo se abordó cada comentario)

Formato final para envío a journal.
```

## Qué recibirás:
✅ Manuscrito final revisado  
✅ Document con track changes  
✅ Response to reviewers lista para enviar

## Guardar:
📝 Guarda como: `15_manuscript_FINAL.md`

---

# PASO 16: CHEERS 2022 Checklist

## ¿Qué hacer?
Verifica que tu paper cumple con todos los estándares de reporte.

## Comando en claude.chat:

```
Valida que mi manuscrito cumple con CHEERS 2022 Checklist.

MANUSCRIPT: [Del Paso 15]

Genera una checklist completa con los 28 items de CHEERS 2022:

Para cada item:
- Item number
- Recommendation del CHEERS guideline
- Location en mi manuscrito (sección, página)
- Compliance status (✓ Compliant / ✗ Missing / ⚠ Partial)
- Si falta algo: ¿qué debo agregar?

Al final:
- % de compliance (X/28 items)
- Lista de acciones para llegar a 100%

IMPORTANTE: Sé estricto. Prefiero saber ahora qué falta que descubrirlo 
después de enviar al journal.
```

## Qué recibirás:
✅ Checklist completa de 28 items  
✅ % de compliance actual  
✅ Lista de acciones para completar

## Guardar:
📝 Guarda como: `16_CHEERS_checklist.md`

---

# PASO 17: Formatear Referencias (APA 7)

## ¿Qué hacer?
Asegura que todas las citas estén en formato correcto.

## Comando en claude.chat:

```
Valida y formatea todas las referencias de mi manuscrito en APA 7.

MANUSCRIPT: [Del Paso 15]

Extrae TODAS las referencias citadas en el texto y:

1. Genera la lista de REFERENCES completa en APA 7
2. Verifica que cada cita in-text coincida con la lista
3. Ordena alfabéticamente por apellido del primer autor
4. Verifica formato:
   - Journal articles
   - Books
   - Book chapters
   - Reports
   - Websites
   - Datasets

5. Identifica errores comunes:
   - DOI faltante
   - Año incorrecto
   - Formato inconsistente

Dame la lista final de REFERENCES lista para copiar-pegar.
```

## Qué recibirás:
✅ Lista de referencias completa en APA 7  
✅ Verificación de consistencia  
✅ Listo para copiar al manuscrito

## Guardar:
📝 Guarda como: `17_references_APA7.md`

---

# ✅ RESULTADO FINAL

Después de estos 17 pasos, tienes:

📄 **Manuscrito completo** (~6000 palabras)
- Title
- Abstract (250 palabras)
- Introduction (800 palabras)
- Methods (1500 palabras)
- Results (1200 palabras)
- Discussion (1200 palabras)
- Conclusions (300 palabras)
- References (APA 7)

📋 **Materiales de soporte**
- Literatura review completa
- Análisis de papers base
- Peer review simulado (5 revisores)
- Revision roadmap
- Response to reviewers
- CHEERS 2022 checklist

🎯 **Listo para**
- Enviar a Health Economics (o tu journal objetivo)
- Responder a revisores si es necesario
- Defender tu metodología

---

# 📊 RESUMEN: Comandos por Fase

| Fase | Qué Hacer | Comando Clave |
|------|-----------|---------------|
| 1 | Refinar idea | "Ayúdame a refinar esta idea usando diálogo socrático..." |
| 2 | Analizar papers | "Analiza este paper científico siguiendo este framework..." |
| 3 | Estructura lit review | "Crea una estructura de literatura review para..." |
| 4 | Escribir lit review | "Escribe la literatura review completa basándote en..." |
| 5 | Outline completo | "Crea un outline detallado para mi paper..." |
| 6 | Introduction | "Escribe la INTRODUCTION completa..." |
| 7 | Methods | "Escribe la sección METHODS completa..." |
| 8 | Results | "Escribe la sección RESULTS..." |
| 9 | Discussion | "Escribe la sección DISCUSSION..." |
| 10 | Conclusions | "Escribe la sección CONCLUSIONS..." |
| 11 | Abstract | "Escribe el ABSTRACT de mi paper..." |
| 12 | Combinar todo | "Combina todas las secciones en un manuscrito completo..." |
| 13 | Peer review | "Simula una revisión de pares de mi manuscrito..." |
| 14 | Roadmap revisión | "Ayúdame a revisar mi manuscrito basándome en reviews..." |
| 15 | Final revisado | "Genera el manuscrito FINAL incorporando revisiones..." |
| 16 | CHEERS checklist | "Valida que mi manuscrito cumple con CHEERS 2022..." |
| 17 | Referencias APA 7 | "Valida y formatea todas las referencias en APA 7..." |

---

# 💡 TIPS FINALES

## ✅ DO's:
- ✅ Sigue los pasos EN ORDEN (cada paso usa outputs del anterior)
- ✅ Guarda CADA output en un archivo separado
- ✅ Sé ESPECÍFICO en tus comandos (más contexto = mejor output)
- ✅ Revisa y edita cada sección antes de pasar a la siguiente
- ✅ Usa el peer review simulado ANTES de enviar al journal real

## ❌ DON'Ts:
- ❌ No saltes pasos (especialmente el peer review)
- ❌ No ignores las limitaciones que Claude identifique
- ❌ No sobre-vendas tus hallazgos en conclusions
- ❌ No copies texto exacto de otros papers (parafrasea siempre)
- ❌ No envíes sin completar CHEERS 2022 checklist

---

# 🎯 TIEMPO ESTIMADO

- **Pasos 1-5** (Preparación): 2-3 horas
- **Pasos 6-11** (Drafting): 4-6 horas
- **Paso 12** (Combinar): 30 minutos
- **Pasos 13-15** (Review + Revisión): 2-3 horas
- **Pasos 16-17** (Validación): 1 hora

**TOTAL**: ~10-14 horas de trabajo activo

(vs 3-6 meses del proceso tradicional)

---

# 📞 ¿NECESITAS AYUDA?

Si en algún paso te atascas:

```
Estoy en el PASO [número] y tengo este problema:
[describe tu problema específico]

¿Puedes ayudarme a:
[qué necesitas específicamente]
```

Claude te ayudará a desbloquearte.

---

**Versión**: 1.0  
**Última actualización**: Mayo 2026  
**Para usar en**: claude.chat  
**Audiencia**: Investigadores en economía de la salud
