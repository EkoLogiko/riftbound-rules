---
title: "Trigger Timing Flowchart"
type: flowchart
rules_document: Core Rules
source_version: "2026-10-09"
aliases: ["Trigger Condition Flowchart", "Trigger Timing"]
cssclasses:
  - riftbound-rules
---

# Trigger Timing Flowchart

[[General Index|General index]] · [[Core Rules Index#Abilities and effects|Abilities and effects]] · [[Turn Phases Flowchart|Related flowchart]]

**Event triggers can happen in any phase**, including during readying, holding, channeling, drawing, or cleanup. A satisfied condition places the ability on the chain as a Pending Item; its effect is processed through the chain. See [[Turn Phases Flowchart]] to locate the turn phases.

**Ability finalization:** [[Playing or Activating Abilities Flowchart]].

**Showdown and combat:** [[Combat Flowchart#Combat sequence|Combat trigger sequence]] · [[Showdown Flowchart#Showdown loop|Showdown loop]] · [[Combat Flowchart#Keyword timing side notes|Keyword timing]].

## Trigger condition check

```mermaid
flowchart TD
    A["An event or specified timing occurs"]
    B["Apply relevant replacement effects"]
    C{"Does this ability trigger<br/>from its own source leaving the board?"}

    A --> B --> C
    C -->|Yes| D["Check immediately before departure<br/>using the actual event after replacements"]
    C -->|No| E["Process the event<br/>then check the resulting game state"]

    D --> F{"Trigger condition fulfilled,<br/>including any immediate 'if' clause,<br/>and ability eligible to trigger?"}
    E --> F

    F -->|No| G["Continue the current process"]
    F -->|Yes| H["Add the ability to the chain<br/>as a Pending Item"]
    H --> I["Order simultaneous triggers:<br/>players in turn order;<br/>each orders their own abilities"]
    I --> G

    G --> J["Finish the current action, task,<br/>or resolving chain item as required"]
    J --> K["Handle Outstanding Tasks"]
    K --> L["Process the chain through FEPR<br/>Finalization applies choices,<br/>costs, and legality checks"]
```

## Read the full rules

- [[Triggered Ability]]
- [[Replacement Effect]]
- [[Chain]]
- [[Pending Chain Item]]
- [[Handling Tasks and Resolving Chain Items]]
- [[HOT FEPR]]
- [[Cleanups]]

This chart is a reading aid. The linked rule notes contain the full conditions, exceptions, and procedures.

## Source references

<details class="rule-ref"><summary title="Core rules 367, 383.2.a.1, 383.2.c, 383.3, 383.3.d, 334, 337, 340; PDF pages 43, 44, 62, 67, 68, 69" aria-label="Show source rules">ⓘ</summary><div class="rule-tooltip">Core rules 367, 383.2.a.1, 383.2.c, 383.3, 383.3.d, 334, 337, 340; PDF pages 43, 44, 62, 67, 68, 69</div></details>
