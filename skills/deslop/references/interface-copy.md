# Interface copy

Read the copy in its screen or flow. When working in code, inspect where the string is rendered, which state shows it, what the control does, and what appears next. A localization key or component name may describe the implementation rather than the user-visible outcome.

## Decide what deserves a place on the screen

- State changes, conditions, costs, and consequences belong where they affect the next choice. Use names, units, and timing the user can connect to the product. In a game, a yield of two branches per trip differs from two branches per second or a one-time grant.
- A button should name the action or outcome. Add nearby help only for a distinct question the label and state leave open. A tooltip can give the condition for an unavailable action. A confirmation should make an important consequence clear before commitment.
- An error should say what failed or what needs correcting. Give a viable way forward if one exists. Include technical terms when the reader can use them to fix or diagnose the issue. Error identifiers can be useful in a details view or when support needs them.
- A status should communicate a meaningful change. An empty state needs an explanation or action only if the blank screen leaves a real question. Accessibility names and announcements can supply equivalent information that isn't visible to their audience. Check them in the context in which they are used.
- In a game, a line can establish mood or character without explaining a mechanic. A tutorial cue can teach an affordance the player cannot yet see. Match its timing and persistence to that need.

When the only job of a line is to explain a weak visual cue, consider strengthening that cue if the task includes design. In a copy-only edit, preserve discoverability and surface the design issue separately. When implementing, check the finished cluster in its actual state when available. Read it in display order with its title, label, helper text, and status. Verify localized strings against the action and surrounding labels. A screenshot shows what was visible in one state. Verify the action separately.

## River Village examples

**First forest.** The banner says «Лес на месте. Нажмите на него, чтобы собирать: ветки и ягоды.» If the forest's arrival is already clear, «Лес на месте» repeats the scene. The instruction may still help on the first encounter if the forest doesn't look clickable. If a click starts gathering, «Нажмите на лес, чтобы собрать ветки и ягоды» is a candidate. If it opens a choice, name that step. If the scene already exposes the interaction, a persistent instruction adds little.

**First camp.** The card shows «Первая стоянка», «Скиталец пришёл с поклажей. Место отмечено флажком», «Можно нажать и на само место с флажком» and the button «Разбить лагерь». The button already names the main action. Does learning the map shortcut help at this point? If it does, one contextual cue can teach it where the flag is. If the button is enough for this moment, the card can lose the click instructions. The line about the wanderer can stay if it sets the intended tone.

**Technical detail that earns space.** «Сработала проверка MAX_UPLOAD_SIZE» describes an implementation. If the confirmed limit is 20 MB and the file exceeds it, «Файл больше 20 МБ. Выберите файл поменьше» gives the user the constraint and the action. For an operator investigating a failing integration, the matching error code can belong in diagnostics.

The placement and restraint guidance draws on [GOV.UK's Writing for user interfaces](https://www.gov.uk/service-manual/design/writing-for-user-interfaces) and [Nielsen's usability heuristics](https://www.nngroup.com/articles/ten-usability-heuristics/).
