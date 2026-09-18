---
name: detector-falacias
description: Detecta falacias lógicas en un argumento dado, las ubica con precisión, explica por qué fallan, muestra cómo refutarlas y distingue casos falaces de usos legítimos similares. Se activa SOLO cuando el usuario lo pide explícitamente, con frases como "detecta falacias", "detectar falacia", "analiza este argumento" o "revisa esta lógica". No se activa automáticamente solo porque el usuario pegue un argumento o esté argumentando en la conversación.
---

# Detector de falacias

Cuando el usuario pida explícitamente análisis de falacias (por ejemplo con "detecta falacias" o "detectar falacia") sobre un argumento que proporcione, pegado, citado o descrito, sigue este procedimiento para cada falacia que identifiques:

## Procedimiento

1. **Lee el argumento completo antes de señalar nada.** No reacciones a la primera premisa sospechosa sin ver la conclusión completa — una falacia aparente a veces se resuelve más adelante en el mismo argumento.

2. **Antes de nombrar una falacia, verifica que no sea un uso legítimo que se le parece.** Esta es la regla más importante del Skill. Muchas falacias tienen una versión válida casi idéntica en superficie:
   - Atacar la credibilidad de una fuente (legítimo) vs. *ad hominem* (descalificar el argumento por la persona)
   - Resumir la posición contraria de forma desfavorable pero fiel (legítimo) vs. *hombre de paja* (distorsionarla)
   - Argumento de autoridad calificada y relevante (legítimo) vs. apelación a autoridad falaz (autoridad irrelevante o no calificada)
   - Generalizar a partir de evidencia suficiente (legítimo) vs. generalización apresurada
   
   Si hay ambigüedad genuina entre las dos lecturas, dilo explícitamente en vez de forzar el veredicto de "falacia".

3. **Para cada falacia real que identifiques, entrega las seis partes:**
   - **Nombre y clasificación** — el nombre de la falacia y su familia (formal / de relevancia / de ambigüedad / de presunción).
   - **Ubicación exacta** — cita el fragmento textual preciso donde ocurre. No generalices sobre "el argumento"; señala la frase.
   - **Por qué falla** — explica la mecánica: qué conexión lógica pretende establecer y por qué no se sostiene.
   - **Cómo se desbarata** — una refutación concreta, construida para *este* argumento específico, no una genérica de manual.
   - **El caso legítimo cercano** — nombra la versión válida que se le parece (ver paso 2), para que quede clara la línea.
   - **Ejemplo gemelo** — un caso paralelo, de otro dominio, que ilustre la misma estructura falaz, para afianzar el reconocimiento futuro.

4. **Modo constructivo (siempre, al final).** Después de desbaratar, ofrece cómo se repararía el argumento: si el autor quería sostener genuinamente su conclusión, ¿cuál sería la forma no-falaz de argumentarlo? Esto convierte el análisis en herramienta de construcción, no solo de demolición.

5. **Si no hay falacias**, dilo directamente y explica brevemente por qué el argumento es válido o al menos no-falaz, sin forzar un hallazgo.

## Formato de salida

Usa encabezados claros por cada falacia encontrada. Sé denso pero no exhaustivo — prioriza precisión sobre extensión.
