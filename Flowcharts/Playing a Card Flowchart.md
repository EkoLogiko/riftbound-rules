---
title: "Playing a Card Flowchart"
type: flowchart
rules_document: Core Rules
source_version: "2026-10-09"
aliases: ["Card Play Flowchart", "Playing a Card Process"]
cssclasses:
  - riftbound-rules
---

# Playing a Card Flowchart

[[General Index|General index]] · [[Core Rules Index#Playing cards and making choices|Playing cards and making choices]] · [[Playing or Activating Abilities Flowchart|Related flowchart]]

This chart summarizes the six stages of playing a card, followed by the different resolution paths for Units, Gear, and Spells.

## Playing a card

```mermaid
flowchart TD
    A["1. Move card to the Chain<br/>It becomes Pending; state becomes Closed<br/>Then finish any current resolution<br/>and outstanding Tasks"]
    C["2. Make relevant choices<br/>Targets, modes, destinations,<br/>optional additional costs"]
    D["3. Determine Total Cost, in order<br/>Base-cost modifications → additional costs<br/>→ increases → discounts<br/>→ Total Cost modifications"]
    E["4. Pay costs<br/>Energy, Power, and nonstandard costs"]
    F{"5. Legal choices and timing,<br/>all costs paid, and no illegal state?"}
    X["Undo the playing process<br/>and cancel the action"]
    G["6. Finish finalizing<br/>Card is no longer Pending"]
    H{"Card category?"}
    U["Unit: resolve immediately<br/>Enter chosen Location exhausted"]
    J["Non-Unit Gear: resolve immediately<br/>Enter your Base Ready"]
    S["Spell: remain on the Chain<br/>as a Finalized item"]
    P["Finalize other Pending items first"]
    R["Reaction window<br/>Process Reactions and resulting items"]
    W["When this spell is next to resolve<br/>and all players pass consecutively"]
    V["Resolve instructions top to bottom<br/>Ignore instructions for illegal targets;<br/>do as much as possible"]
    T["Put the spell in its owner's Trash"]
    A --> C --> D --> E --> F
    F -->|No| X
    F -->|Yes| G --> H
    H -->|Unit| U
    H -->|Non-Unit Gear| J
    H -->|Spell| S --> P --> R --> W --> V --> T
```

Units and Gear resolve immediately without a Reaction window between finalization and resolution. Their passive abilities become active, and their rules text is processed; any resulting triggered abilities follow their own process. See [[Trigger Timing Flowchart]] and [[Playing or Activating Abilities Flowchart]].

For costs, component-specific discounts apply when that component is added, before discounts on the total. Energy and Power costs cannot fall below zero.

## Read the full rules

- [[Playing Cards]]
- [[Process of Playing a Card]]
- [[Costs]]
- [[Targeting]]
- [[Unit]]
- [[Gear]]
- [[Spell]]
- [[Handling Tasks and Resolving Chain Items]]

This chart is a reading aid. The linked rule notes contain the full conditions, exceptions, and procedures.

## Source references

<details class="rule-ref"><summary title="Core rules 334, 337, 340, 354, 355, 356, 357, 358, 359; PDF pages 43, 44, 46, 47, 52, 54, 55" aria-label="Show source rules">ⓘ</summary><div class="rule-tooltip">Core rules 334, 337, 340, 354, 355, 356, 357, 358, 359; PDF pages 43, 44, 46, 47, 52, 54, 55</div></details>
