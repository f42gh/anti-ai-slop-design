---
name: anti-ai-slop-design
description: Design, build, redesign, audit, or polish distinctive frontend interfaces without generic AI-generated defaults. Use for web pages, landing pages, product UI, dashboards, components, and design systems; do not use for backend-only or purely textual work.
---

# Anti-AI Slop Design

Create interfaces that look deliberately made for their subject. Replace unexamined defaults with decisions grounded in the product, audience, content, and use scene. Preserve product truth, behavior, accessibility, and the project's existing visual contract.

## Resolve authority first

Apply constraints in this order:

1. The user's explicit request and supplied references.
2. A project-root `DESIGN.md` or `design.md`, read in full.
3. Repository instructions, existing design tokens, brand assets, and component contracts.
4. Functional correctness, semantics, data integrity, accessibility, and input modality.
5. Product, audience, platform, content, and viewport needs.
6. The selected art direction.
7. Anti-slop heuristics.

Never let a lower-ranked aesthetic preference override a higher-ranked contract. Do not edit or regenerate an existing `DESIGN.md` unless the user explicitly asks. If no design contract exists, form a provisional internal brief; persist one only when requested. Use [DESIGN.template.md](assets/DESIGN.template.md) when a project-specific contract is part of the task.

## Choose the task mode

- **Greenfield:** define a compact visual system and build the real primary experience.
- **Existing implementation:** inspect first, then make scoped changes without breaking public behavior.
- **Redesign / de-slop:** preserve product truth, identify the layers causing genericness, and replace only those layers.
- **Audit:** report evidence and prioritized corrections; do not edit.
- **Component:** inherit the surrounding system and skip page-level identity work.

Do not turn a build request into an audit report or an audit request into an unapproved redesign.

## Inspect before deciding

Read the relevant routes, components, styles, tokens, assets, fonts, icons, state models, and project checks. Identify the exact files in scope and the behavior, content, props, routes, analytics, and data flow that must remain compatible. Render the current interface when practical; source alone cannot establish visual hierarchy, crop quality, density, or motion.

Do not install a package, replace a framework, or introduce a parallel design system merely to imitate a trend.

## Ground the direction

Before detailed design, write a compact internal brief:

```text
Surface and task mode:
Audience and primary outcome:
Product thesis:
Use scene and desired feeling:
Content spine and factual evidence:
Available subject-specific artifacts and media:
Authoritative design constraints:
Behavioral, responsive, accessibility, and performance constraints:
```

For a substantial public, editorial, portfolio, commerce, or branded surface, consider three materially different directions. Vary the visual carrier, silhouette, type treatment, material logic, section rhythm, and motion—not merely color. Include one restrained direction. Select the option that is most specific to the subject and feasible in the repository.

For a component, operational screen, or narrow edit, inherit one quiet direction from the surrounding product. Do not invent a new identity.

Read [aesthetic-directions.md](references/aesthetic-directions.md) when establishing page composition or art direction.

## Build from structure, not decoration

1. Define the primary reading or task path.
2. Choose a macrostructure that follows the content and user outcome.
3. Make the first viewport express the product thesis through a real subject, artifact, action, or typographic idea.
4. Establish the smallest useful semantic token set from the existing contract.
5. Use proximity, hierarchy, rhythm, and whitespace before cards, borders, shadows, blur, or gradients.
6. Spend distinctiveness on one memorable, justified move; keep supporting regions disciplined.
7. Use real content and assets. Label concepts honestly; never invent testimonials, metrics, logos, awards, scarcity, or product evidence.
8. Implement the primary path and every reachable state required by the feature.

Read [anti-patterns.md](references/anti-patterns.md) before generating, redesigning, or auditing an interface. Treat the catalog as a detector of unchosen defaults, not a list of absolute style bans.

For dashboards, forms, application shells, settings, commerce, data views, or interactive components, also read [product-ui.md](references/product-ui.md).

## Preserve implementation integrity

- Preserve routes, exports, props, state transitions, data flow, content meaning, and accessibility unless the user changes their scope.
- Prefer scoped, recoverable edits. Do not delete production files or restructure ownership merely for a new look.
- Use semantic HTML and native controls where possible. ARIA supplements semantics; it does not replace them.
- Cover relevant states: default, hover where applicable, focus-visible, active, selected, disabled, loading, empty, error, success, and recovery.
- Name actions concretely. Keep copy short, factual, and consistent with the product voice.
- Use motion to explain state, hierarchy, causality, or spatial relationships. Respect reduced motion and keep state feedback intact.

## Verify in bounded passes

After implementation:

1. Run the relevant project checks.
2. Inspect one narrow mobile and one desktop viewport together; add other states and viewports only when risk requires them.
3. Fix observed defects in one batch.
4. Confirm once more, then stop open-ended polishing.
5. Re-run the anti-pattern scan and test whether the result is justified, coherent, specific, restrained, and complete.

Read [verification.md](references/verification.md) before handoff. State what changed, what was checked, what the evidence proves, and what remains unverified.

## Reference map

- [anti-patterns.md](references/anti-patterns.md): contextual AI-tell catalog and audit format.
- [aesthetic-directions.md](references/aesthetic-directions.md): subject grounding, direction exploration, and macrostructure.
- [product-ui.md](references/product-ui.md): operational UI, interaction states, forms, data, and responsive behavior.
- [verification.md](references/verification.md): bounded visual, accessibility, responsive, and implementation validation.
- [provenance.md](references/provenance.md): conceptual sources and synthesis boundaries.
- [DESIGN.template.md](assets/DESIGN.template.md): optional project-specific design contract template.
