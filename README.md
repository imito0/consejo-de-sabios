# consejo-de-sabios

> Consejo de Sabios para tu asistente de IA: 5 expertos analizan tu negociación por separado y un Moderador integra todo en una recomendación con guion de conversación.

## Qué hace

Cuando le planteas una negociación (salario, precio, contrato, alquiler, condiciones...), el plugin convoca a un **Consejo de Sabios**:

| Asesor | Rol |
|---|---|
| **El Estratega** | BATNA, ZOPA, anclaje y plan de concesiones |
| **El Abogado del Diablo** | Riesgos, puntos débiles y tácticas que usará la contraparte |
| **El Psicólogo** | Motivaciones reales, tono y manejo de la relación |
| **El Externo** | Opinión objetiva, sin apego a tu contexto |
| **El Ejecutor** | 3 pasos concretos para mañana + guion con frases literales |
| **El Moderador** | Consenso, tensiones y recomendación final (plan A/B y línea roja) |

Incluye un **modo simulacro**: el asistente hace de contraparte para que ensayes la conversación antes de la cita real.

## Instalación

### Claude Code (como plugin de este repo)

```
/plugin marketplace add <tu-usuario>/consejo-de-sabios
/plugin install consejo-de-sabios@consejo-de-sabios-plugins
```

### Claude Code (manual, solo la skill)

```
ln -s "$PWD/skills/consejo-de-sabios" ~/.claude/skills/consejo-de-sabios
```

La carpeta `skills/consejo-de-sabios/` es markdown puro y funciona también en otros agentes compatibles con el formato SKILL.md.

## Uso

Describe tu situación con todo el detalle que puedas. Por ejemplo:

> Tengo una oferta de 45.000 € como desarrollador backend en Madrid. Llevo 4 años en mi empresa actual ganando 38.000. La empresa nueva me gusta pero me gustaría llegar a 50.000. Tengo una semana para responder.

Si falta información clave, el Consejo te hará solo las preguntas imprescindibles antes de deliberar. Tras la deliberación puedes:

- preguntar a un asesor concreto ("¿qué diría el Abogado del Diablo sobre...?"),
- pedir el guion literal de la conversación,
- o simular la negociación con el modo simulacro.

## Licencia

MIT
