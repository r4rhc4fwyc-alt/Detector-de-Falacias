# Contexto del proyecto

Detector-de-Falacias es, ante todo, un **repo de aprendizaje**. El contenido (falacias lógicas) ya lo domina el usuario — el objetivo real de este repo es que use el tema como excusa de bajo riesgo para aprender Claude Code y Git con un caso concreto, no abstracto.

## Quién es el usuario

Roberto. Aprendiendo Claude Code desde cero, sin PC — trabaja desde iPad (navegador y la app de Claude). Prefiere explicación directa primero; aterriza mejor los conceptos después de hacer el gesto con las manos. Piensa en voz alta y razona por contraste. Antes de ejecutar cualquier acción no trivial, explícale primero qué vas a hacer y por qué.

## Estado actual del Skill

- `detector-falacias` (`.claude/skills/detector-falacias/SKILL.md`) está terminado y funcionando.
- Activación: **manual únicamente** — requiere frases explícitas ("detecta falacias", "detectar falacia", "analiza este argumento", "revisa esta lógica"). Se ajustó a propósito para que no se dispare solo con cualquier argumento pegado en el chat.
- También está empaquetado y subido a Claude.ai (Customize > Skills) como `anthropic-skills:detector-falacias`, para usarlo en cualquier conversación fuera de este repo. **Las dos copias son independientes**: si se edita el Skill acá, hay que volver a exportarlo (zip) y resubirlo a Claude.ai para que se actualice allá también.

## Qué ya aprendió Roberto (no reexplicar desde cero)

- Qué es un commit ("foto" con mensaje), un branch, un merge, un pull request.
- Diferencia entre `git add` (preparar), `git commit` (fotografiar) y `git push` (sincronizar con GitHub).
- El mismo ciclo editar → add → commit → push, hecho tanto desde la terminal como desde el editor web de GitHub.
- Diferencia entre borrar una rama local (`git branch -d`) y una remota (`git push origin --delete`).
- Por qué GitHub y una copia local se desincronizan (dos copias mirando "fotos" distintas de la misma historia) y cómo se resuelve con `pull`/`fetch`.
- Cómo se decide la activación automática vs. manual de un Skill: el campo `description` del frontmatter en `SKILL.md` es la única señal que usa Claude para decidir cuándo dispararlo solo.

## Cómo ayudarlo

- Explicar antes de ejecutar, especialmente en cambios visibles hacia afuera (push, borrar ramas remotas).
- Aterrizar los conceptos con ejemplos reales de este repo (sus propios commits, ramas, archivos) en vez de teoría abstracta o genérica.
- Confirmar antes de acciones destructivas o difíciles de revertir.
