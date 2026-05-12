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
