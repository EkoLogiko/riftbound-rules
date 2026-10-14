---
title: "Turn Phases Flowchart"
type: flowchart
rules_document: Core Rules
source_version: "2026-10-09"
aliases: ["Turn Flowchart", "Turn Sequence Flowchart"]
cssclasses:
  - riftbound-rules
---

# Turn Phases Flowchart

[[General Index|General index]] · [[Core Rules Index#Turns and timing|Turns and timing]] · [[Trigger Timing Flowchart|Related flowchart]]

This chart shows the default turn. Finish the current phase or step's outstanding tasks and required chain processing before advancing. Card effects and game-mode rules can modify the default turn.

**⚡ marks when a trigger condition can become satisfied.** See [[Trigger Timing Flowchart]] for how those conditions are checked and processed.

## Turn sequence

**Before the first turn:** [[Game Setup Flowchart#Game setup sequence|Set up the game and check mode-specific first-turn changes]].

```mermaid
flowchart TD
    subgraph START["Start of Turn"]
        A["Awaken Phase<br/>Ready eligible game objects you control"]
        B["Beginning Phase — Beginning Step<br/>⚡ At start of Beginning Phase"]
        C["Beginning Phase — Scoring Step<br/>Hold battlefields you control<br/>⚡ Hold triggers"]
        D["Channel Phase<br/>Channel 2 runes, or as many as remain"]
        E["Draw Phase<br/>Draw 1<br/>Handle Burn Out if necessary"]
        A --> B --> C --> D --> E
    end

    subgraph MAIN["Main Phase"]
        F["Main Phase entry<br/>Empty every player's Rune Pool<br/>Then ⚡ at start of Main Phase<br/>Complete tasks and chain processing"]
        G["Take actions; handle chains,<br/>showdowns, and combat<br/>⚡ Matching event triggers throughout"]
        H{"Ready to end Main Phase?"}
        F --> G --> H
        H -->|No| G
    end

    subgraph ENDING["Ending Phase"]
        I["Ending Step<br/>⚡ At end of turn<br/>Process resulting abilities"]
        J["Expiration Step<br/>Ending Special Cleanup includes:<br/>heal all Units → expire 'this turn' effects<br/>→ empty every Rune Pool"]
        K["Finish outstanding tasks<br/>and required chain processing"]
        L{"Did any item undergo<br/>the FEPR process?"}
        I --> J --> K --> L
        L -->|Yes: repeat Expiration| J
    end

    E --> F
    H -->|Yes| I
    L -->|No| N["Next queued turn begins"]
    N --> A
```

**Beginning Step abilities are processed before holding.** The **Expiration Step** can repeat without repeating the **Ending Step**.

## Read the full rules

- [[Start of Turn]]
- [[Main Phase]]
- [[Ending Phase]]
- [[Turn Phases]]
- [[Beginning Step]]
- [[Scoring Step]]
- [[Ending Step]]
- [[Expiration Step]]
- [[Handling Tasks and Resolving Chain Items]]
- [[HOT FEPR]]
- [[Cleanups]]

This chart is a reading aid. The linked rule notes contain the full conditions, exceptions, and procedures.

## Source references

<details class="rule-ref"><summary title="Core rules 315, 316, 317, 334, 335; PDF pages 37, 38, 40, 43" aria-label="Show source rules">ⓘ</summary><div class="rule-tooltip">Core rules 315, 316, 317, 334, 335; PDF pages 37, 38, 40, 43</div></details>
