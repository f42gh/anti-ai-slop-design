# Product UI and states

Use this reference for dashboards, application shells, forms, settings, onboarding, commerce, data views, and components. Operational clarity outranks novelty.

## Identify the user posture

- **Persuade:** help a visitor decide and act; brand and evidence lead.
- **Operate:** help a user complete a task; scanability, consistency, and stable behavior lead.
- **Read:** help a user understand; structure, measure, and continuation lead.
- **Experience:** let the work itself lead; interface chrome recedes.

A marketing page and its signed-in dashboard can require different postures. Do not style every route as the product's most expressive surface.

## Preserve the component contract

For component work:

1. Read the containing system and representative neighbors.
2. Preserve props, events, semantics, size contract, and ownership.
3. Inherit type, color, spacing, shape, icons, and motion.
4. Implement only states the component can reach.
5. Verify long labels, narrow containers, keyboard and touch input, zoom, and disabled or error conditions.

Do not invent page navigation, a hero, a new palette, or unrelated layout for a component.

## Interaction states

Cover the relevant matrix:

- default;
- hover for pointer devices;
- `:focus-visible` with immediate visible feedback;
- active or pressed;
- selected or current;
- disabled, including the reason when needed;
- loading without unstable layout;
- empty with a clear next action;
- error naming the problem and recovery;
- success with restrained confirmation;
- optimistic update with recovery or undo when appropriate.

When a state changes the background, verify foreground, icon, border, and focus contrast. Never rely on color alone.

## Forms

- Use persistent labels; placeholders are examples, not labels.
- Place instructions before the action they affect and errors beside the field or group they describe.
- Preserve entered values after recoverable errors.
- Move focus only when the interaction genuinely changes context.
- Use native elements and browser behavior as the baseline.
- Keep the same concrete action verb through button, progress, success, and error copy.
- Prefer undo over confirmation for safe, reversible actions.

## Data and dashboards

- Choose density from task frequency, comparison needs, and decision complexity.
- Use tables when row/column comparison matters. Preserve comparison on mobile through controlled scroll, prioritization, disclosure, or a purpose-built alternate view.
- Align comparable values and expose units, freshness, filters, sort, time range, empty states, and errors.
- Encode meaning with labels, position, shape, or pattern in addition to color.
- Reserve cards for bounded entities, selected options, or framed tools. Use rows, dividers, whitespace, and grouped regions for continuous information.
- Keep primary, comparison, and detail paths obvious without turning every metric into a climax.

## App shells and commerce

- Persistent chrome is justified by frequent switching and stable tasks, not category habit.
- Keep the primary canvas dominant and secondary regions contextual.
- Bound sticky regions so they do not hide focused content, headings, anchors, or errors.
- Show believable product states with real labels and data, not fake browser chrome.
- In commerce, reveal the product, price, options, availability, and purchase path early.
- Do not fabricate scarcity, countdowns, reviews, discounts, or savings.
- Add sticky buying controls only when they restore an action that has scrolled away.

## Responsive behavior

Recompose rather than shrink:

- preserve DOM, reading, and focus order;
- move contextual panels after the primary task or into labeled disclosure;
- keep touch targets usable and essential controls reachable;
- change crops deliberately to preserve the subject;
- retain comparison meaning;
- allow horizontal scrolling only for intentional, accessible data or media regions;
- account for virtual keyboards, safe areas, dynamic viewport height, and sticky chrome.

## Motion

Use motion to communicate state, causality, spatial transition, or direct manipulation. Keep feedback fast and predictable and use one shared timing language. Avoid layout jank, blocking motion, unpausable autoplay, and perpetual effects in dense operational surfaces. Under reduced motion, preserve state change and hierarchy with direct transitions.
