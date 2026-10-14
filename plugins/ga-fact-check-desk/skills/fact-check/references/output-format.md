# Output format

Use the user's language unless they request another language. For Spanish, use the labels below exactly. For English, translate the section labels but preserve the five-verdict logic.

## Single central claim

Use this order:

## VEREDICTO
One of:
- Correcto
- Correcto con matices
- Engañoso
- Incorrecto
- No verificable

## CONFIANZA
One of `Alta`, `Media`, `Baja`.
If not `Alta`, add one concise sentence explaining the limitation.

## AFIRMACIÓN ANALIZADA
Reproduce the central claim briefly and faithfully.

## RESULTADO
Explain the factual conclusion in 2–4 sentences. State what is supported, what is not, and the material context required to understand the verdict. If an incorrect or misleading claim contains a true component, identify that true component explicitly.

## PROBLEMAS DETECTADOS
List only material or critical issues. If none: `No se han detectado problemas materiales.`

## EVIDENCIA CLAVE
Use only the sources necessary to support the verdict. Prefer:
1. decisive primary source;
2. one or two genuinely independent corroborating or counter-evidence sources when useful.

For each source provide organisation/publisher, specific document/article/dataset, date and link. Explain its evidentiary role if not self-evident.

## REDACCIÓN RECOMENDADA
Give the minimum factual correction while preserving language, intent and register. If no change is needed: `No requiere cambios.`

## REQUIERE JUICIO HUMANO
Include only when necessary. Explain the exact unresolved judgement in 1–2 sentences.

## VERIFICADO A
Give the local date and time of verification when available.

## Multiple material claims

Start with:

`Veredicto general: [veredicto]`
`Confianza general: [nivel]`

Then use a compact table:

| Afirmación | Veredicto | Confianza | Problema principal |
|---|---|---|---|
| ... | ... | ... | ... |

Develop only claims that are `Incorrecto`, `Engañoso`, materially `Correcto con matices`, low-confidence, or require human judgement. Do not bury the user in detail for claims that are plainly correct.

## Verdict calibration

- **Correcto** — The material claim is supported and nothing significant is missing.
- **Correcto con matices** — The core claim is supported but requires clarification, qualification or limited contextual correction that does not reverse the main meaning.
- **Engañoso** — The statement contains true elements but wording, omitted context, denominator, comparison, status, causality or framing would reasonably lead to a materially wrong impression.
- **Incorrecto** — The central material proposition is contradicted by reliable evidence or contains a critical factual error.
- **No verificable** — Available evidence is insufficient to substantiate or refute the claim to the required standard.

## Confidence calibration

- **Alta** — Clear primary evidence or strong independent convergence; no material unresolved contradiction.
- **Media** — Good evidence but a material limitation remains, such as indirect sourcing, incomplete primary access or a bounded interpretive uncertainty.
- **Baja** — Single weak chain, significant unresolved contradiction, incomplete evidence or substantial inference.

Confidence measures the quality of verification, not how plausible the claim feels.
