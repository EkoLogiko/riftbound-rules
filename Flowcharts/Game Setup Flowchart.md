---
title: "Game Setup Flowchart"
type: flowchart
rules_document: Core Rules
related_rules_document: Tournament Rules
source_version: "2026-10-09"
aliases: ["Setup Flowchart", "All Modes Setup", "Game Setup", "Mulligan Sequence", "Opening Hand Setup"]
cssclasses:
  - riftbound-rules
---

# Game Setup Flowchart

[[General Index|General index]] · [[Core Rules Index#Deck construction and setup|Core setup rules]] · [[Tournament Rules Index#Matches and tournament procedures|Tournament procedures]] · [[Turn Phases Flowchart|Turn sequence]]

All five Core Rules modes share one path until their setup procedures diverge. Battlefield selection is shown after determining the First Player because FFA4 and 2v2 depend on that result. See [[Game Setup Flowchart#Tournament adjustments|Tournament adjustments]] for competition-specific changes.

## Game setup sequence

```mermaid
flowchart TD
    START["Choose mode<br/>1v1 Duel · 1v1 Match · FFA3 · FFA4 · 2v2"]
    TEAM{"2v2?"}
    TEAMYES["4 players: two teams of two<br/>Victory Score: 11 shared points<br/>Teammates use different Legends and Battlefields"]
    TEAMNO["No teams; Victory Score: 8<br/>1v1: 2 players · FFA3: 3 · FFA4: 4"]
    START --> TEAM
    TEAM -->|Yes| TEAMYES
    TEAM -->|No| TEAMNO

    subgraph PREP["Prepare cards"]
        P["Each player places their Legend in the Legend Zone<br/>Then their Chosen Champion in the Champion Zone<br/>Set aside their 3 Battlefields"]
        SHUFFLE["Shuffle Main and Rune Decks separately<br/>Place each deck in its own Zone"]
        P --> SHUFFLE
    end

    subgraph ORDER["Determine turn order"]
        FIRST["Determine First Player<br/>Use an agreed fair random method"]
        T{"2v2?"}
        SOLO["1v1 / FFA<br/>Clockwise from First Player"]
        TEAMS["2v2: alternate teams<br/>First Player → opponent → teammate → other opponent"]
        FIRST --> T
        T -->|No| SOLO
        T -->|Yes| TEAMS
    end

    subgraph FIELDS["Select and place Battlefields"]
        BF{"Mode?"}
        DUEL["1v1 Duel<br/>Each player randomly selects 1 of their 3"]
        MATCH["1v1 Match<br/>Each player chooses 1 available Battlefield<br/>Keep the others for later games"]
        FFA3["FFA3<br/>Each player randomly selects 1 of their 3"]
        FOUR["FFA4 / 2v2<br/>First Player's Battlefields are not used<br/>Each other player randomly selects 1 of their 3"]
        PLACE["Place selected Battlefields simultaneously<br/>1v1: 2 total · FFA3 / FFA4 / 2v2: 3 total"]
        BF -->|Duel| DUEL --> PLACE
        BF -->|Match| MATCH --> PLACE
        BF -->|FFA3| FFA3 --> PLACE
        BF -->|FFA4 / 2v2| FOUR --> PLACE
    end

    subgraph HAND["Opening hands"]
        DRAW["Everyone draws 4"]
        MULL["Mulligan, in turn order<br/>Set aside up to 2 → draw replacements<br/>→ recycle to Main Deck bottom<br/>Random order if recycling 2"]
        BEGIN["First Player begins their turn"]
        DRAW --> MULL --> BEGIN
    end

    subgraph BONUSES["Each player's FIRST turn only"]
        BONUS{"Mode?"}
        ONE["1v1 Duel / Match<br/>Second Player: channel +1 Rune<br/>during their first Channel Phase"]
        MANY["FFA3 / FFA4 / 2v2<br/>First Player: no card from their first Draw Phase<br/>Last Player: channel +1 Rune<br/>during their first Channel Phase"]
        BONUS -->|1v1| ONE
        BONUS -->|FFA / 2v2| MANY
    end

    TEAMYES --> P
    TEAMNO --> P
    SHUFFLE --> FIRST
    SOLO --> BF
    TEAMS --> BF
    PLACE --> DRAW
    BEGIN --> BONUS
```

## Between games of 1v1 Match

- [[1v1 (Match)|1v1 Match]] is best of 3 by default; optionally best of 5. Other modes are best of 1.
- After a won game, both players use different Battlefields next game.
- Best-of-5 games 4–5 permit reuse after all three were presented, with no Battlefield presented more than twice.

## Tournament adjustments

- The [[Play First Rule]] gives a designated player the first/last choice. Later games use the previous loser’s choice; draws retain the starting order.
- [[2v2 (Tournament)|Tournament 2v2]] uses the repeating order **Team 1 A → Team 2 A → Team 1 B → Team 2 B**; the deciding team chooses the starting position.
- Draws require the same Battlefields next game. Deck presentation, opponent shuffling, sideboarding and the optional altered best-of-1 sequence follow [[Start of Game Procedure]].

## Read the full rules

- [[Setup Process]]
- [[1v1 (Duel)]]
- [[1v1 (Match)]]
- [[FFA3 (Skirmish)]]
- [[FFA4 (War)]]
- [[2v2 (Magma Chamber)]]
- [[Recycle]]
- [[Start of Game Procedure]]
- [[Play First Rule]]
- [[2v2 (Tournament)]]
- [[Sideboard]]
- [[Shuffling]]

This chart is a reading aid. The linked rule notes contain the full conditions, exceptions, and procedures.

## Source references

<details class="rule-ref"><summary title="Core rules 110, 111, 112, 113, 114, 115, 116, 117, 118, 417, 487, 488, 489, 490, 491; PDF pages 7, 8, 79, 111, 112, 113" aria-label="Show source rules">ⓘ</summary><div class="rule-tooltip">Core rules 110, 111, 112, 113, 114, 115, 116, 117, 118, 417, 487, 488, 489, 490, 491; PDF pages 7, 8, 79, 111, 112, 113</div></details>

<details class="rule-ref"><summary title="Tournament rules 403, 406, 407, 603.7; PDF pages 8, 9, 10, 31" aria-label="Show source rules">ⓘ</summary><div class="rule-tooltip">Tournament rules 403, 406, 407, 603.7; PDF pages 8, 9, 10, 31</div></details>
