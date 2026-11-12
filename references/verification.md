# Verification and handoff

Verify the built result, not the intention. Keep the process bounded: one batched inspection, one batched correction, one confirmation.

## Evidence ladder

Use the strongest practical evidence:

1. UI/UX review of hierarchy, task flow, copy, states, density, product fit, and design-contract fidelity.
2. Static inspection of semantics, styles, source paths, tokens, and component contracts.
3. Existing project checks such as typecheck, lint, unit tests, and build.
4. Rendered inspection at representative states and viewports.
5. Existing browser or end-to-end tests when the project owns them or the task requires them.
6. Reasoned inference, explicitly labeled unverified.

Never claim a viewport, contrast, keyboard, performance, screen-reader, or interaction pass from prose or source review alone.

## Batched visual review

Inspect at minimum:

- one narrow mobile viewport with long real content;
- one desktop viewport;
- the primary path and the most consequential alternate state.

Add tablet, breakpoint-adjacent, short-height, landscape, zoom, localization, dark theme, reduced motion, or data-extreme states only when risk justifies them. Review mobile and desktop together before editing so corrections address the system.

## Design-system fidelity

- An existing `DESIGN.md` remains unchanged unless explicitly in scope.
- Any value changed because the contract would break the accessibility floor is listed with its ratio and a suggested amendment.
- Fonts, colors, spacing, borders, shape, motion, and copy follow the authoritative system.
- No parallel token system or one-off palette has appeared.
- Every new surface, line, radius, effect, and animation has a reason.
- A refinement remains recognizably the same product.

## Accessibility and input

- Semantic structure and heading order match the reading route.
- Controls have accessible names, states, and relationships.
- Keyboard order matches visual order; no traps exist.
- Focus-visible feedback is immediate, unclipped, distinct, and at least 3:1 against adjacent colors; nothing removes it with `outline: none`.
- Computed contrast meets the target for every color pair actually used, in every state and theme: text 4.5:1, large text (≥24px, or ≥18.66px bold) 3:1, component boundaries and meaningful non-text marks 3:1. Disabled controls, logos, and pure decoration are exempt. List the pairs and ratios in the completion report; do not round.
- Touch targets are at least 24×24 CSS pixels (WCAG 2.5.8) or meet a larger project minimum; prefer about 44×44 when space allows, enlarging the hit area with padding.
- Content survives zoom and text resizing without loss or overlap.
- Reduced-motion users retain state feedback and hierarchy.
- Color is not the only carrier of meaning.
- Errors identify the problem and recovery; focus management is intentional.

## Responsive and layout

- No unintended horizontal overflow exists.
- The primary action and orientation remain reachable at short heights.
- Long Japanese and English text wraps without clipping or pathological columns.
- Fixed and sticky elements do not cover anchors, headings, fields, errors, focused controls, or final content.
- Background bleed and content containment remain aligned.
- Bounded surfaces retain inset and wrapped siblings retain deliberate gaps.
- Real images preserve their focal subject under actual crops.
- Scroll snapping, if used, does not trap keyboard, touch, trackpad, or reduced-motion users.

## Functional integrity

- Routes, exports, props, state, data fetching, analytics, and content meaning remain compatible.
- Primary controls work and relevant loading, empty, error, disabled, success, and recovery paths are reachable.
- No fabricated claims, identities, ratings, testimonials, or metrics were introduced.
- No new dependency was added without necessity.
- Project checks pass, or introduced failures are separated from pre-existing ones.

## Anti-slop judgment

Answer these questions after the catalog scan:

1. **Justified:** Can each major decision be traced to the subject, user, task, design contract, or real content?
2. **Coherent:** Do type, palette, layout, carrier, states, and motion reinforce one direction?
3. **Specific:** Would the interface still identify this product if its logo disappeared?
4. **Restrained:** Is there one memorable move with disciplined support rather than several competing tricks?
5. **Structurally distinct:** Does the macrostructure follow the content rather than a familiar generated sequence?
6. **Complete:** Are the primary path, responsive behavior, real content, and reachable states finished?

Fix failed answers before handoff.

## Completion report

Report concisely:

- files and meaningful design changes;
- how the existing design contract was preserved;
- checks run and their results;
- rendered viewports and states inspected;
- accessibility and responsive evidence;
- remaining unverified risk.

Do not hide skipped checks behind “looks good.”
