Viendo tu repositorio, el problema principal no es el contenido.

El problema es que estás mezclando:

```text
Conceptos
Arquitectura
Instalación
Hardware
Prompts
Metodología
AWS
OpenClaw
MarketMirrorAI
```

en el mismo nivel.

Por eso GitHub no puede ayudarte a encontrar las cosas rápidamente.

---

# Mi recomendación

Usa el sistema que utilizan los arquitectos de software:

## Nivel 1: Carpetas

```text
MarketMirrorAI/
│
├── 00-README
│
├── 01-VISION
│
├── 02-METHODOLOGY
│
├── 03-OPENCLAW
│
├── 04-AWS
│
├── 05-DATA-SOURCES
│
├── 06-HARDWARE
│
├── 07-PROMPTS
│
├── 08-AGENTS
│
├── 09-IMPLEMENTATION
│
└── 10-REFERENCE
```

---

# Dentro de OPENCLAW

```text
03-OPENCLAW
│
├── 01-Concepts.md
├── 02-Skills.md
├── 03-Memory.md
├── 04-Agent.md
├── 05-Soul.md
├── 06-Heartbeat.md
├── 07-Learning-Mode.md
├── 08-Shadow-Agent.md
└── 09-Bedrock-Integration.md
```

---

# Dentro de AWS

```text
04-AWS
│
├── 01-Lightsail.md
├── 02-EC2.md
├── 03-Bedrock.md
├── 04-S3.md
├── 05-IAM.md
├── 06-Networking.md
└── 07-Costs.md
```

---

# Dentro de Hardware

```text
06-HARDWARE
│
├── 01-Raspberry-Pi.md
├── 02-Jetson-Orin.md
├── 03-Cameras.md
├── 04-PIR-Sensors.md
└── 05-Comparisons.md
```

---

# Convención de nombres

Evitar:

```text
** SYSTEM PROMPT v2.md
* market API to Jetson.md
mirror: pasado interpreta presente.md
```

Porque:

* símbolos especiales desordenan GitHub
* los espacios dificultan enlaces
* las búsquedas son menos limpias

---

Usar:

```text
01-system-prompt-v1.md
02-system-prompt-v2.md

01-market-api-jetson.md

01-past-interprets-present.md
```

---

# Para MarketMirrorAI

Yo usaría una numeración de tres niveles:

```text
01.00-vision.md
01.01-problem.md
01.02-solution.md

02.00-methodology.md
02.01-trend-change.md
02.02-trend-continuation.md

03.00-openclaw.md
03.01-skills.md
03.02-agent.md
03.03-soul.md
```

Ventaja:

GitHub siempre mostrará:

```text
01
02
03
04
05
```

en orden lógico.

---

# Lo que haría inmediatamente

Renombraría:

```text
OpenClaw.md
OpenClaw concepts.md
OpenClaw's features.md
AWS - OpenClaw.md
```

a:

```text
03.00-openclaw-overview.md
03.01-openclaw-concepts.md
03.02-openclaw-features.md
03.03-openclaw-aws-deployment.md
```

y crearía una carpeta:

```text
03-OPENCLAW
```

porque sospecho que OpenClaw se convertirá en una parte muy importante de MarketMirrorAI y terminarás con decenas o cientos de documentos relacionados con él.

La regla que sigo en proyectos grandes es:

> Si un tema tendrá más de 10 documentos, merece su propia carpeta.
> Si tendrá más de 50 documentos, merece además numeración jerárquica (01.00, 01.01, 01.02...).

Para MarketMirrorAI, ya estás entrando claramente en esa segunda categoría.
