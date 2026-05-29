Te lo voy a explicar usando una analogía sencilla porque OpenClaw puede parecer más complejo de lo que realmente es.

# Imagina que OpenClaw es una empresa

```text
CEO                → Agent
Personalidad       → soul.md
Empleado           → user.md
Reglamento         → agent.md
Agenda diaria      → heartbeat.md
Herramientas       → Skills
Memoria            → Memory
```

---

# 1. agent.md = EL REGLAMENTO DEL AGENTE

Es el archivo más importante.

Le dice al agente:

```text
Quién eres
Qué haces
Qué no haces
Qué prioridad tienes
Cómo tomar decisiones
```

Ejemplo:

```md
You are MarketMirror Observer.

Primary goal:
Detect trend changes in options markets.

Never:
Execute trades.
Modify production systems.

Always:
Provide evidence.
Show confidence score.
```

OpenClaw leerá esto constantemente.

Piensa en él como:

```text
La descripción del cargo
```

---

# 2. soul.md = LA PERSONALIDAD

No define el trabajo.

Define la forma de pensar.

Ejemplo:

```md
Be skeptical.

Never assume.

Prefer evidence over opinion.

Think like a quantitative analyst.
```

o

```md
Think like Warren Buffett.

Prefer long-term reasoning.
```

o

```md
Think like a risk manager.
```

Es el equivalente a:

```text
La personalidad del empleado
```

---

# 3. user.md = EL JEFE

Describe quién eres tú.

Ejemplo:

```md
The user is building MarketMirrorAI.

The user prefers:
- AWS
- Evidence based reasoning
- Cost efficient solutions

The user is interested in:
- Options
- Trend detection
- AI agents
```

Esto ayuda a OpenClaw a entender:

```text
Qué le importa a Iván
```

---

# 4. heartbeat.md = EL LATIDO

Este archivo define:

```text
Qué hacer periódicamente
```

Ejemplo:

```md
Every 15 minutes:
Check news.

Every 30 minutes:
Check options flow.

Every 60 minutes:
Generate report.
```

Piensa en:

```text
La agenda automática del agente
```

---

# 5. Skills = HERRAMIENTAS

Los Skills son superpoderes.

Sin Skills:

```text
OpenClaw puede pensar.
```

Con Skills:

```text
OpenClaw puede actuar.
```

Ejemplos:

### Skill Web

```text
Buscar noticias
```

### Skill Files

```text
Leer PDFs
```

### Skill Email

```text
Enviar correos
```

### Skill Telegram

```text
Enviar alertas
```

### Skill Database

```text
Guardar memoria
```

---

# Cómo interactúan

Supongamos tu proyecto.

```text
Noticias
      ↓
Skill Web
      ↓
OpenClaw
      ↓
agent.md
      ↓
soul.md
      ↓
heartbeat.md
      ↓
Telegram Skill
      ↓
Alerta
```

---

# Lo que yo haría para MarketMirrorAI

## agent.md

```text
Objetivo:
Detectar cambios de tendencia.

Nunca:
Ejecutar operaciones.

Siempre:
Generar evidencia.
```

---

## soul.md

```text
Actúa como un analista cuantitativo.

Sé conservador.

Evita falsas alarmas.
```

---

## heartbeat.md

```text
Cada 15 minutos:
Revisar noticias.

Cada 30 minutos:
Revisar opciones.

Cada 60 minutos:
Comparar señales.
```

---

## user.md

```text
El usuario es Iván.

Construye MarketMirrorAI.

Prefiere:
AWS
Bedrock
Análisis verificable

No quiere:
Operaciones automáticas.
```

---

# La clave conceptual

Mucha gente piensa que OpenClaw es:

```text
LLM + Tools
```

Pero realmente es más parecido a:

```text
LLM
+
Personalidad (soul.md)
+
Misión (agent.md)
+
Usuario (user.md)
+
Agenda (heartbeat.md)
+
Skills
+
Memoria
```

Por eso OpenClaw se siente más como un "empleado digital" que como un chatbot tradicional.

Para tu caso, yo construiría primero un único agente:

```text
MarketMirror Observer
```

que solo observe, aprenda tu metodología desde PDFs y genere alertas, sin permisos para ejecutar ninguna operación. Ese sería el mejor laboratorio para comparar OpenClaw contra el workflow principal de MarketMirrorAI.
