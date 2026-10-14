---
title: "Playing or Activating Abilities Flowchart"
type: flowchart
rules_document: Core Rules
source_version: "2026-10-09"
aliases: ["Ability Play Flowchart", "Activating Abilities Flowchart"]
cssclasses:
  - riftbound-rules
---

# Playing or Activating Abilities Flowchart

[[General Index|General index]] · [[Core Rules Index#Abilities and effects|Abilities and effects]] · [[Playing a Card Flowchart|Related flowchart]]

This chart summarizes the process for activated and triggered abilities. See [[Trigger Timing Flowchart]] for when trigger conditions are checked and [[Playing a Card Flowchart]] for the shared playing procedure.

## Playing or activating abilities

```mermaid
flowchart TD
    A["1. Activate an ability or its trigger condition is met<br/>Then add a Pending ability to the Chain<br/>State becomes Closed<br/>Then finish any current resolution<br/>and outstanding Tasks"]
    C["2. Make relevant choices<br/>If a triggered effect starts with<br/>'you may' or 'they may', decide now"]
    D["Choose targets, modes,<br/>and other required options"]
    Q{"Enough legal choices?"}
    X["Remove triggered ability from Chain<br/>Never Finalized; not countered"]
    I["Process is illegal<br/>Cancel and undo it"]
    E["3. Determine Total Cost<br/>Base cost and applicable modifications"]
    F["4. Pay costs"]
    L{"5. Targets still legal,<br/>costs paid, permissions met,<br/>and no illegal state?"}
    G["6. Finalize the ability<br/>It is no longer Pending"]
    H{"Does the ability Add resources?"}
    M["Resolve immediately<br/>Then remove the Chain item"]
    P["Finalize other Pending items first"]
    R["Reaction window<br/>Process Reactions and resulting items"]
    N["When this ability is next to resolve<br/>and all players pass consecutively"]
    V["Resolve like a spell, top to bottom<br/>Ignore instructions for illegal targets;<br/>do as much as possible"]
    T["Remove the ability's Chain item"]
    A --> C
    C -->|Decline initial may| X
    C -->|Continue| D --> Q
    Q -->|No: triggered| X
    Q -->|No: activated| I
    Q -->|Yes| E --> F
    F -->|Triggered: decline payment| X
    F -->|Costs paid| L
    L -->|No| I
    L -->|Yes| G --> H
    H -->|Yes| M
    H -->|No| P --> R --> N --> V --> T
```

An activated ability’s base cost appears before `:`. A triggered ability usually has no base cost; a cost within instructions at the beginning of its effect—or immediately after its initial “may”—is paid during finalization.

A “may” appearing later in the effect is decided **during resolution**.

## Read the full rules

- [[Playing or Activating an Ability]]
- [[Activated Ability]]
- [[Triggered Ability]]
- [[Costs within Instructions]]
- [[Add]]
- [[Targeting]]
- [[Handling Tasks and Resolving Chain Items]]

This chart is a reading aid. The linked rule notes contain the full conditions, exceptions, and procedures.

## Source references

<details class="rule-ref"><summary title="Core rules 334, 337, 340, 383.3.a, 383.3.b, 400, 401, 402, 403, 404, 405, 406, 407; PDF pages 43, 44, 69, 75, 76" aria-label="Show source rules">ⓘ</summary><div class="rule-tooltip">Core rules 334, 337, 340, 383.3.a, 383.3.b, 400, 401, 402, 403, 404, 405, 406, 407; PDF pages 43, 44, 69, 75, 76</div></details>
