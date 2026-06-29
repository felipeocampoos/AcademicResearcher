# 🎯 GUÍA PRÁCTICA: De Idea a Paper Publicable

**Para usar desde claude.ai con Projects**

---

## 📦 SETUP INICIAL (Hacer UNA VEZ)

### Paso 0: Configurar tu Proyecto en Claude.ai

**1. Clona el repositorio en tu PC**:
```bash
git clone https://github.com/felipeocampoos/AcademicResearcher.git
```

**2. Ve a claude.ai y crea un Project**:
- Click en "Projects" (menú izquierdo)
- Click "Create Project"
- Nombre: tu tema (ej: "HPP Cost-Effectiveness Colombia")

**3. Sube los archivos al Project Knowledge**:
- Click en "Add content" → "Upload files"
- Sube estos 3 archivos obligatorios:

```
✅ claude.md                  ← Instrucciones base + router de skills
✅ SKILL_opinion.md           ← Skill para columnas de opinión
✅ SKILL_originalpaper.md     ← Skill para artículos científicos
```

**4. ¡Listo!** Claude ahora tiene:
- Contexto de economía de la salud
- Sabe cuándo escribir para prensa vs para journal
- Aplica el estilo correcto automáticamente

---

## 🔧 ¿Cómo Sabe Claude Qué Skill Usar?

El `claude.md` tiene un **router** que detecta automáticamente:

| Si pides... | Claude activa... |
|------------|-----------------|
| "Escribe una columna de opinión..." | `SKILL_opinion.md` |
| "Escribe un editorial para El Tiempo..." | `SKILL_opinion.md` |
| "Escribe la Introduction de mi paper..." | `SKILL_originalpaper.md` |
| "Redacta los Methods para Lancet..." | `SKILL_originalpaper.md` |
| "Escribe un artículo..." (ambiguo) | Claude pregunta primero |

**No necesitas mencionar las skills** — Claude las detecta por el tipo de petición.

---

## 📝 PARTE 1: ARTÍCULO CIENTÍFICO ORIGINAL

*Usa `SKILL_originalpaper.md` — Para publicar en journals indexados*

---

### PASO 1: Refina tu Pregunta de Investigación

**🔧 Skill**: `claude.md` (contexto de economía de la salud)

**Comando**:
```
Tengo una idea de investigación en economía de la salud:

IDEA: [describe tu idea en 1-2 oraciones]

Ayúdame a refinarla cubriendo:
1. Carga de enfermedad
2. Intervenciones existentes
3. Contexto SGSSS
4. Brecha de conocimiento
5. Relevancia para política

Dame pregunta de investigación clara + objetivos específicos
```

**Guardar**: `01_research_question.md`

---

### PASO 2: Analiza tus Papers Base

**🔧 Skill**: `claude.md` (Academic Researcher framework)

**Comando** (repetir para cada paper):
```
Analiza este paper [sube PDF o pega info]:

Extrae:
- Research question
- Diseño metodológico
- Findings principales (ICER, costos, efectividad)
- Implicaciones para política
- Limitaciones
- Cita en APA 7
```

**Guardar**: `02_papers_analysis.md`

---

### PASO 3: Busca Literatura Adicional

**🔧 Skill**: `claude.md` (Systematic Literature Search)

**Comando**:
```
Diseña una estrategia de búsqueda para:

TEMA: [tu pregunta de investigación]
PECO:
  P: [población]
  E: [exposición/intervención]
  C: [comparador]
  O: [desenlaces económicos]

Necesito:
1. String de búsqueda para PubMed y Scopus
2. Criterios de inclusión/exclusión
3. Recomendación de 5 artículos clave
```

**Guardar**: `03_search_strategy.md`

---

### PASO 4: Estructura la Literatura Review

**🔧 Skill**: `claude.md`

**Comando**:
```
Crea estructura de lit review para [tu pregunta]

Papers analizados: [pega del Paso 2]

Incluye:
- Theoretical frameworks (CE, CU, CBA)
- Thematic synthesis (por temas, no cronológico)
- Research gaps específicos para Colombia/LATAM
- Vocabulario CHEERS 2022
```

**Guardar**: `04_lit_review_outline.md`

---

### PASO 5: Escribe la Literatura Review

**🔧 Skill**: `SKILL_originalpaper.md`

**Comando**:
```
Escribe la literatura review completa siguiendo SKILL_originalpaper:

Outline: [del Paso 4]
Papers: [del Paso 2]
Pregunta: [del Paso 1]

Requisitos:
- Escalera epistémica correcta (no conviertas asociación en causalidad)
- Vocabulario económico consistente
- APA 7
- 1500-2000 palabras
- Brecha de investigación clara al final
```

**Guardar**: `05_literature_review.md`

---

### PASO 6: Crea el Outline Completo

**🔧 Skill**: `SKILL_originalpaper.md`

**Comando**:
```
Crea outline detallado para mi paper siguiendo SKILL_originalpaper:

Pregunta: [del Paso 1]
Journal objetivo: [Health Economics / Lancet / Value in Health / etc.]
Formato: IMRAD + CHEERS 2022
Longitud: [6000 palabras o límite del journal]

Incluye subsecciones numeradas para:
- Abstract (250 palabras)
- Introduction (~800 palabras)
- Methods (~1500 palabras)
- Results (~1200 palabras)
- Discussion (~1200 palabras)
- Conclusions (~300 palabras)

Para cada sección: indica qué datos necesito y qué estándares seguir
```

**Guardar**: `06_paper_outline.md`

---

### PASO 7: Escribe la Introduction

**🔧 Skill**: `SKILL_originalpaper.md`

**Comando**:
```
Escribe la INTRODUCTION siguiendo SKILL_originalpaper:

Outline: [sección Introduction del Paso 6]
Literatura: [del Paso 5]
Pregunta: [del Paso 1]

Estructura (embudo de problema a contribución):
1. Define el problema (enfermedad, política, mecanismo)
2. Cuantifica la carga (clínica, económica, equidad)
3. Mecanismo institucional que hace importante la pregunta
4. Evidencia cercana + qué permanece desconocido
5. Objetivo en una oración directa
6. Contribución o novedad

Tono: formal, analítico, no promocional
~800 palabras, APA 7
```

**Guardar**: `07_introduction.md`

---

### PASO 8: Escribe los Methods

**🔧 Skill**: `SKILL_originalpaper.md`

**Comando**:
```
Escribe la sección METHODS siguiendo SKILL_originalpaper:

Outline: [sección Methods del Paso 6]
Tipo de análisis: [CEA / CUA / cuasi-experimental / descriptivo]

Incluye en este orden:
1. Diseño y perspectiva analítica
2. Escenario y contexto institucional (SGSSS)
3. Período y fuentes de datos
4. Población y criterios de elegibilidad
5. Definición de intervenciones comparadas
6. Desenlaces y medición
7. Análisis principal (modelo económico)
8. Análisis de sensibilidad
9. Análisis de equidad (subgrupos)

CHEERS 2022 compliant, reproducible
~1500 palabras
```

**Guardar**: `08_methods.md`

---

### PASO 9: Escribe los Results

**🔧 Skill**: `SKILL_originalpaper.md`

**Comando**:
```
Escribe la sección RESULTS siguiendo SKILL_originalpaper:

Outline: [sección Results del Paso 6]
Mis datos: [pega tus resultados o datos disponibles]

Patrón por párrafo: hallazgo → comparación → explicación → implicación
Tono: neutral, reportar sin interpretar aún
Incluye: estimados centrales + intervalos de confianza
~1200 palabras
```

**Guardar**: `09_results.md`

---

### PASO 10: Escribe la Discussion

**🔧 Skill**: `SKILL_originalpaper.md`

**Comando**:
```
Escribe la DISCUSSION siguiendo SKILL_originalpaper:

Results: [resumen del Paso 9]
Literatura: [papers base del Paso 2]

Subsecciones:
1. Hallazgos principales vs literatura (sin repetir resultados)
2. Implicaciones para política (actor + mecanismo específico)
3. Equidad (¿quién se beneficia/excluye?)
4. Limitaciones (honestas y técnicamente específicas)
5. Investigación futura

Lenguaje causal: ajustado al diseño del estudio
~1200 palabras
```

**Guardar**: `10_discussion.md`

---

### PASO 11: Escribe las Conclusions

**🔧 Skill**: `SKILL_originalpaper.md`

**Comando**:
```
Escribe las CONCLUSIONS siguiendo SKILL_originalpaper:

Hallazgos: [del Paso 9]
Implicaciones: [del Paso 10]

Requisitos:
- 1-2 párrafos compactos
- Reitera respuesta central + magnitud
- Implicación para sistema de salud
- Nombra actor responsable o mecanismo
- Recomendación proporcionada (NO slogan)
- Sin nueva evidencia ni afirmaciones amplias
~300 palabras
```

**Guardar**: `11_conclusions.md`

---

### PASO 12: Escribe el Abstract

**🔧 Skill**: `SKILL_originalpaper.md`

**Comando**:
```
Escribe el ABSTRACT siguiendo SKILL_originalpaper:

Secciones completas: [Pasos 7-11]
Journal: [nombre del journal]

Estructura (250 palabras máximo):
- Background/problema: 1-2 oraciones
- Objetivo: 1 oración explícita
- Methods: diseño, escenario, población, datos, método
- Results: muestra, estimados centrales, incertidumbre
- Conclusion: respuesta directa + implicación acotada

Sin literatura de antecedentes salvo que sea esencial
Reporta magnitudes reales, no solo "significativo" o "sustancial"
```

**Guardar**: `12_abstract.md`

---

### PASO 13: Manuscrito Completo

**🔧 Skill**: `claude.md`

**Comando**:
```
Combina todas las secciones en manuscrito completo:

Abstract: [Paso 12]
Introduction: [Paso 7]
Methods: [Paso 8]
Results: [Paso 9]
Discussion: [Paso 10]
Conclusions: [Paso 11]

Formato Markdown
Verifica: transiciones suaves, acrónimos consistentes, tono uniforme
```

**Guardar**: `13_manuscript_complete.md`

---

### PASO 14: Peer Review Simulado

**🔧 Skill**: `claude.md` (Academic Paper Reviewer framework)

**Comando**:
```
Simula peer review completo:

Manuscript: [del Paso 13]
Journal: [tu journal objetivo]

5 revisores:
1. Methodology Specialist
2. Health Economics Expert
3. Public Health / Cross-disciplinary
4. Devil's Advocate
5. Editor-in-Chief (decisión final)

Output: fortalezas, debilidades, revisiones REQUERIDAS vs opcionales
```

**Guardar**: `14_peer_reviews.md`

---

### PASO 15: Aplica Revisiones

**🔧 Skill**: `SKILL_originalpaper.md`

**Comando**:
```
Crea roadmap de revisión y aplica cambios:

Manuscript: [Paso 13]
Reviews: [Paso 14]

Para cada revisión REQUERIDA:
- Ubicación exacta (sección + párrafo)
- Texto actual
- Texto revisado
- Justificación del cambio

Genera también: Response to Reviewers
```

**Guardar**: `15_manuscript_FINAL.md`

---

### PASO 16: CHEERS 2022 Checklist

**🔧 Skill**: `claude.md`

**Comando**:
```
Valida CHEERS 2022 completo:

Manuscript: [Paso 15]

Para cada uno de los 28 items:
- Número y recomendación
- Ubicación en mi manuscrito
- Status: ✓ Compliant / ✗ Missing / ⚠ Partial
- Si falta: qué agregar

% de compliance + acciones para llegar al 100%
```

**Guardar**: `16_CHEERS_checklist.md`

---

### PASO 17: Referencias APA 7

**🔧 Skill**: `claude.md`

**Comando**:
```
Valida y formatea todas las referencias en APA 7:

Manuscript: [Paso 15]

- Lista completa ordenada alfabéticamente
- Verifica coherencia in-text vs lista
- DOIs correctos y accesibles
- Formato consistente por tipo (journal, libro, reporte)
```

**Guardar**: `17_references_APA7.md`

---

## 📰 PARTE 2: COLUMNA DE OPINIÓN PÚBLICA

*Usa `SKILL_opinion.md` — Para publicar en prensa, medios o blogs*

---

### PASO A: Define el Tema y el Gancho

**🔧 Skill**: `SKILL_opinion.md`

**Comando**:
```
Quiero escribir una columna de opinión sobre [tema].

DATO MOTIVADOR: [hecho reciente, cifra o evento que motiva escribirla]
TESIS: [qué quieres defender, aunque sea preliminar]
AUDIENCIA: [periódico, medio o blog objetivo]

¿Con cuál de estos patrones encaja mejor mi tema?
A) Medida popular, efecto indeseado
B) Dato técnico, impacto ciudadano
C) Concepto abusado
D) Referente internacional

Dame una propuesta de estructura antes de escribir.
```

---

### PASO B: Escribe la Columna

**🔧 Skill**: `SKILL_opinion.md`

**Comando**:
```
Escribe la columna de opinión siguiendo SKILL_opinion:

TEMA: [tu tema]
PATRÓN: [A / B / C / D]
DATO MOTIVADOR: [hecho/cifra de apertura]
TESIS: [lo que quieres defender]

Requisitos:
- Título: 2-6 palabras
- 400-500 palabras
- Apertura con hecho concreto (no abstracción)
- Tesis antes del párrafo 3
- Mínimo 1 dato específico con fuente
- Cierre con juicio claro (no pregunta abierta)
- Tono sobrio, argumentativo, no panfletario
```

---

### PASO C: Revisa con Checklist

**🔧 Skill**: `SKILL_opinion.md`

**Comando**:
```
Revisa esta columna con el checklist de SKILL_opinion:

COLUMNA: [pega el texto]

Verifica:
- ¿Abre con hecho concreto?
- ¿Tesis antes del párrafo 3?
- ¿Hay al menos 1 dato con fuente?
- ¿Explica implicación no obvia?
- ¿Tiene matiz o concesión?
- ¿Cierra con juicio claro?
- ¿Entre 400-500 palabras?
- ¿No copia frases de textos de referencia?

Dame el texto corregido si hay problemas.
```

---

## 📊 RESUMEN: Qué Skill Usar en Cada Paso

### Para Artículo Científico:

| Paso | Tarea | Skill |
|------|-------|-------|
| 1 | Refinar pregunta | `claude.md` |
| 2 | Analizar papers | `claude.md` |
| 3 | Buscar literatura | `claude.md` |
| 4 | Estructurar lit review | `claude.md` |
| 5 | Escribir lit review | `SKILL_originalpaper.md` |
| 6 | Outline completo | `SKILL_originalpaper.md` |
| 7-11 | Drafting secciones | `SKILL_originalpaper.md` |
| 12 | Abstract | `SKILL_originalpaper.md` |
| 13 | Manuscrito completo | `claude.md` |
| 14 | Peer review | `claude.md` |
| 15 | Revisiones | `SKILL_originalpaper.md` |
| 16 | CHEERS checklist | `claude.md` |
| 17 | Referencias APA 7 | `claude.md` |

### Para Columna de Opinión:

| Paso | Tarea | Skill |
|------|-------|-------|
| A | Definir tema y patrón | `SKILL_opinion.md` |
| B | Escribir columna | `SKILL_opinion.md` |
| C | Revisar con checklist | `SKILL_opinion.md` |

---

## ⏱️ TIEMPO ESTIMADO

### Artículo Científico:
- Pasos 1-4 (Preparación): 2-3 horas
- Pasos 5-12 (Drafting): 4-6 horas
- Pasos 13-15 (Review + Revisión): 2-3 horas
- Pasos 16-17 (Validación): 1 hora
- **TOTAL: 10-14 horas** (vs 3-6 meses tradicional)

### Columna de Opinión:
- Pasos A-C: **30-60 minutos**

---

## ✅ CHECKLIST FINAL

### Artículo Científico:
- [ ] Manuscript completo (~6000 palabras)
- [ ] Abstract ≤ 250 palabras
- [ ] CHEERS 2022: 28/28 items ✓
- [ ] Referencias APA 7 correctas
- [ ] Peer review simulado completado
- [ ] Revisiones aplicadas
- [ ] Response to reviewers preparada
- [ ] Verbos causales ajustados al diseño
- [ ] Limitaciones honestas y específicas
- [ ] Recomendaciones con actor + mecanismo nombrado

### Columna de Opinión:
- [ ] Título 2-6 palabras
- [ ] Apertura con hecho concreto
- [ ] Tesis antes del párrafo 3
- [ ] Mínimo 1 dato con fuente
- [ ] Implicación no obvia explicada
- [ ] Cierre con juicio claro
- [ ] 400-500 palabras

---

## 💡 TIPS

✅ Sube los 3 archivos al Project Knowledge antes de empezar
✅ Claude detecta automáticamente qué skill usar
✅ Guarda cada output en archivo separado
✅ Revisa cada sección manualmente antes de continuar
✅ No saltes el peer review (Paso 14)

❌ No subas solo `claude.md` — necesitas los 3 archivos
❌ No copies texto exacto de papers
❌ No conviertas asociación en causalidad en el paper
❌ No envíes sin completar CHEERS checklist

---

**Versión**: 3.0
**Para**: Claude.ai Projects
**Audiencia**: Investigadores en economía de la salud
**Archivos requeridos**: `claude.md` + `SKILL_opinion.md` + `SKILL_originalpaper.md`
