# Contextual anti-patterns

Use this catalog to find unchosen defaults. A pattern is a problem when it is reflexive, repeated, irrelevant to the subject, unsupported by the design contract, or harmful to hierarchy and trust. A purposeful convention is not a failure merely because it appears here.

## Severity and evidence

- **P0 — template fingerprint or contract violation:** a generic generated-page pattern dominates the result, or the UI contradicts an authoritative project rule.
- **P1 — structural or interaction weakness:** repetition, weak hierarchy, incomplete states, or poor product fit impairs use or trust.
- **P2 — craft gap:** rhythm, copy, crop, motion, or browser-surface details remain unfinished.

Label each finding as `code-certain`, `rendered`, or `inferred`. Without a render, palette dominance, spacing rhythm, visual hierarchy, crop, and motion remain inferred.

## Typography

- One unexamined default font for every role.
- A novelty serif, italic, or monospace added only as an AI-design costume.
- Display type repeated at hero scale throughout the page.
- Arbitrary sizes, weights, tracking, or hard line breaks without a role system.
- Uncomfortable measure, weak line height, clipped glyphs, or brittle localization.

Correct by following the project contract, defining the fewest roles that create real hierarchy, and using scale, weight, measure, rhythm, placement, and spacing before adding families.

## Color and material

- An unchosen purple-to-blue gradient, gradient headline, aurora blob, or generic neon glow.
- Framework defaults presented as a finished visual identity.
- One-off colors added per component instead of semantic reuse.
- Equal amounts of many timid accents with no dominant relationship.
- Glass, blur, shadow, grain, or texture without a material or layering reason.
- Decorative color competing with the primary action or semantic state signal.
- Insufficient contrast in text, borders, controls, or focus feedback.

Correct by mapping a small palette to stable roles: canvas, surface, primary and secondary text, rule, action, focus, and semantic states. Each material effect must encode grouping, hierarchy, state, or atmosphere.

## Structure and layout

- Centered hero → three equal feature cards → stats → testimonials → CTA → multi-column footer.
- Three cards created because the brief happened to contain three bullets.
- Every section wrapped in the same rounded rectangle.
- Cards nested inside cards or used to compensate for weak grouping.
- Alternating left/right split sections with no narrative reason.
- Big-number heroes, metric strips, pricing trios, or social proof unsupported by real content.
- Decorative eyebrows, section numbers, or labels that encode no genuine order.
- Centering everything when reading or task priority calls for alignment.
- Large empty areas that create neither focus nor transition.
- Desktop composition merely shrunk or stacked on mobile.

Correct by choosing a subject-specific macrostructure and varying alignment, density, media ratio, containment, and section rhythm according to each region's job.

## Components and chrome

- Untouched component-library styling presented as a brand.
- The same large radius and soft shadow on every surface.
- Repeated icon-in-rounded-square feature tiles or colored side-stripe cards.
- Fake browser, phone, terminal, IDE, or macOS traffic-light chrome.
- Emoji or unrelated glyphs standing in for a coherent icon system.
- Raw arrows appended to every link and button.
- A modal used for a task that needs neither interruption nor protected focus.
- Missing hover, focus-visible, active, disabled, loading, empty, error, success, or recovery states.

Correct by inheriting project primitives, using containment only when it communicates grouping or state, and implementing the actual interaction contract.

## Motion

- The same fade-up reveal on every section.
- `transition: all` or universal hover scaling.
- Endless ambient motion that competes with reading or input.
- Bounce, overshoot, cursor followers, particles, or glow loops substituting for a central idea.
- Reduced-motion handling that removes essential state feedback.

Correct by choosing one authored motion idea and at most two quiet support layers. Use motion for state, hierarchy, causality, or spatial relationship and provide a direct reduced alternative.

## Copy and content

- Brand-agnostic headlines such as “Elevate your workflow,” “Seamless,” “Unleash,” or “Next generation.”
- Generic names, filler testimonials, fabricated logos, invented metrics, fake urgency, or round proof numbers.
- UI copy that describes the prompt, hero, layout, or generation process.
- “Submit” or “Get started” where a concrete action verb exists.
- Excess explanations, redundant labels, and decorative microcopy.
- Placeholder imagery presented as authentic evidence.

Correct with real product language, concrete verbs, minimal copy, source-backed content, and honest labels for concepts or placeholders.

## Imagery and visual carrier

- A gradient blob standing in for a real product, person, place, object, output, or process.
- Generic team-at-a-laptop stock photography.
- Plastic abstract 3D forms unrelated to the subject.
- Tiny product mockups floating inside several nested frames.
- Crops that remove faces, product details, text, or critical silhouettes.
- Decorative media that cannot explain or support the product thesis.

Prefer supplied authentic assets, real screenshots or data, appropriate sourced or generated media, and code-native diagrams of the actual mechanism. If the correct asset is unavailable, keep the composition media-ready and state the limitation.

## Audit format

```text
[P0/P1/P2] Finding
Location: file:line, component, or rendered region
Evidence: code-certain | rendered | inferred
Why: impact on product fit, hierarchy, behavior, or trust
Contract: relevant user, DESIGN.md, or implementation constraint
Fix: smallest concrete correction
```

A clean catalog pass does not prove good design. Also test specificity, coherence, restraint, factual integrity, and faithfulness to the product.
