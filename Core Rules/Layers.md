---
title: "Layers"
type: core-topic
rules_document: Core Rules
source_version: "2026-10-09"
cssclasses:
  - riftbound-rules
---

# Layers

[[Start Here|Home]] · [[Concept Index|Find a concept]] · [[Core Rules Index|Core rules]]

<span title="Core rule 475"></span> ^cr-475

<details class="rule-ref"><summary title="Core rule 475 · PDF page 106" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 475 · PDF page 106</div></details>

Layers are the mechanism in which [[Game Effect|Game Effects]] alter the Traits, Intrinsic [[Ability|Abilities]], or other properties of [[Game Object|Game Objects]]. ^cr-476

<details class="rule-ref"><summary title="Core rule 476 · PDF page 106" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 476 · PDF page 106</div></details>

Layers are an organizational structure. ^cr-477

<details class="rule-ref"><summary title="Core rule 477 · PDF page 106" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 477 · PDF page 106</div></details>

Layers only serve to structure the application and order that [[Game Effect|Game Effects]] apply to [[Game Object|Game Objects]] to maintain consistency. ^cr-477-1

<details class="rule-ref"><summary title="Core rule 477.1 · PDF page 106" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 477.1 · PDF page 106</div></details>

The layers are applied repeatedly until all effects operating on an object have been applied once and no changes have been processed. ^cr-478

<details class="rule-ref"><summary title="Core rule 478 · PDF page 106" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 478 · PDF page 106</div></details>

Layers are applied and evaluated continuously. All [[Game Object|Game Objects]] have their layers updated in the same instant, but each Game Object is treated separately and individually when evaluating layers. ^cr-478-1

<details class="rule-ref"><summary title="Core rule 478.1 · PDF page 106" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 478.1 · PDF page 106</div></details>

If evaluating a [[Game Effect]]’s applicability depends on information from one or more other [[Game Object|Game Objects]], that Game Effect has an object [[Level|level]] [[Dependency]]. Pause evaluating the layers of the dependent Game Object and evaluate the layer effects of those Game Objects whose information is referenced. Continue once the applicability of that Game Effect has been established or disqualified. ^cr-478-1-a

**Example:** A 4 &#91;M&#93; [[Unit|unit]] reads in part “While I’m &#91;[[Mighty]]&#93;, I’m a Yeti.” Another unit reads in part “I have all tags of units you [[Control|control]].” When the 4 &#91;M&#93; unit is [[Buffs|buffed]], the layers for all [[Game Object|game objects]] are evaluated. While evaluating the layers for the second unit, it requires us to pause and evaluate the layers for all other units. When we’re evaluating the layers for the 4 &#91;M&#93; unit, after all is said and done, the unit has the Yeti [[Tag|tag]]. Once we’ve evaluated all units, we go back to evaluating the second unit, and at that time it has the Yeti tag as well.

<details class="rule-ref"><summary title="Core rule 478.1.a · PDF page 106" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 478.1.a · PDF page 106</div></details>

If a [[Game Object]] has an object [[Level|level]] [[Dependency|dependency]] with a Game Object that itself has an object level dependency with a third Game Object and so on, determine the final point of the dependency [[Chain|chain]] and evaluate the layer effects of that Game Object first, continuing up the dependency chain until all Game Objects have had their layer effects evaluated. ^cr-478-1-b

<details class="rule-ref"><summary title="Core rule 478.1.b · PDF page 106" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 478.1.b · PDF page 106</div></details>

If a [[Dependency|dependency]] [[Chain|chain]] loops back around on itself, identify the minimum set of [[Game Object|Game Objects]] in the loop and evaluate their layer effects simultaneously, layer by layer. If any of them have [[Game Effect|Game Effects]] that reference Game Objects from outside the set, pause and evaluate those Game Objects first before continuing with the set. ^cr-478-1-c

**Example:** A 4 &#91;M&#93; [[Unit|unit]] reads “If there is a &#91;[[Mighty]]&#93; [[Enemy|enemy]] unit here, I have +5 &#91;M&#93;.” Both players [[Control|control]] one of these units at a [[Battlefield|battlefield]] during [[Combat|combat]]. Each one is [[Buffs|buffed]]. A third player plays Siphon [[Power]], which reads “Choose a battlefield. Give [[Friendly|friendly]] units there +1 &#91;M&#93; this [[Turn|turn]], and enemy units there -1 &#91;M&#93; this turn, to a minimum of 1 &#91;M&#93;.” Both of the units there are given -1 &#91;M&#93;. Because they have effects that reference each other, they have a [[Dependency|dependency]] [[Chain|chain]]. After evaluating their layers simultaneously, layer by layer, both units will be 4 &#91;M&#93;.

<details class="rule-ref"><summary title="Core rule 478.1.c · PDF page 106-107" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 478.1.c · PDF page 106-107</div></details>

Layers are applied in sequence. Each effect in them is applied as soon as able, and only a single time across all sequences. ^cr-478-2

<details class="rule-ref"><summary title="Core rule 478.2 · PDF page 107" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 478.2 · PDF page 107</div></details>

When a sequence of applications completes, recur the process, and evaluate each layer again applying any effects that may now be applicable. ^cr-478-3

<details class="rule-ref"><summary title="Core rule 478.3 · PDF page 107" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 478.3 · PDF page 107</div></details>

The removal or disqualification of an effect is separate from the application of the effect, but still can only be applied once. ^cr-478-4

**Example:** Fiora, Victorious has [[Printed Might|printed Might]] 4 and says “While I'm [[Mighty]], I have [[Deflect]], [[Ganking]], and [[Shield]].” If a player places a [[Buffs|buff]] on Fiora, her [[Might]] is increased in the Arithmetic layer, after the layer for [[Ability-Altering Effects]]. The Ability-Altering Effect layer is then re-checked and the [[Ability|abilities]] Deflect, Ganking, and Shield applied. Since each effect has been applied once and there are no other effects to apply, Fiora’s characteristics are finalized as 5 Might with Deflect, Ganking, and Shield. While a buffed Fiora, Victorious is [[In Combat|in combat]] as a [[Defender|defender]], an additional +1 Might will be applied in the Arithmetic layer, giving her 6 Might and the 3 [[Keywords|keywords]].

**Example:** A [[Buffs|buffed]] Fiora, Victorious is [[In Combat|in combat]] as a [[Defender|defender]] when her buff is removed. Reevaluating the layers in sequence, she no longer gains [[Deflect]], [[Ganking]], and [[Shield]] during the Ability-Altering Effect layer, so when the Arithmetic layer is evaluated, neither the buff (which is gone) nor Shield (which she no longer has) apply. She goes directly from 6 [[Might]] with three [[Keywords|keywords]] to 4 Might with no keywords.

<details class="rule-ref"><summary title="Core rule 478.4 · PDF page 107" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 478.4 · PDF page 107</div></details>

Layers are applied in the following order: ^cr-479

<details class="rule-ref"><summary title="Core rule 479 · PDF page 107" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479 · PDF page 107</div></details>

### 1. Copy Effects

^cr-479-1

<details class="rule-ref"><summary title="Core rule 479.1 · PDF page 107" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.1 · PDF page 107</div></details>

This layer deals with all [[Copy Effects|copy effects]]. ^cr-479-1-a

<details class="rule-ref"><summary title="Core rule 479.1.a · PDF page 107" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.1.a · PDF page 107</div></details>

When a [[Copy]] effect is applied to a [[Game Object]], the traits specified by the Copy Effect replace or are added to the Copyable Traits of the Game Object being Copied as specified by the effect. If no traits are specified by a Copy Effect, all traits of the Game Object are replaced with those of the Copied Game Object. ^cr-479-1-b

**Example:** A player triggers Leblanc, Deceiver’s [[Hold Effect|hold effect]] and plays a Reflection [[Token|token]], making it a [[Copy|copy]] of Honest Broker. That player then plays Mirror Image, [[Targeting|targeting]] the Reflection token. When the Mirror Image Reflection token is played, it copies all of the copyable traits of the original Reflection token - which are currently those of Honest Broker which it is a copy of. That player will have three [[Unit|units]] named Honest Broker in [[Play|play]], two of which are token Copies with [[Temporary]].

<details class="rule-ref"><summary title="Core rule 479.1.b · PDF page 107" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.1.b · PDF page 107</div></details>

The copyable traits of a [[Game Object]] are all of the printed—or if a [[Copy|copy]] effect is applied, copied—traits of that Game Object. In the case of a [[Token]], they are the traits the token had when it was Created. ^cr-479-1-b-1

**Example:** The copyable traits include the printed versions of the following traits: [[Card Name|Name]], [[Supertype]], Type, Tags, [[Costs|Cost]], [[Domain]], [[Rules Text]], [[Effect Text]], [[Might]], [[Might Bonus]], [[Flavor Text]], Art

<details class="rule-ref"><summary title="Core rule 479.1.b.1 · PDF page 107" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.1.b.1 · PDF page 107</div></details>

Copyable traits of a [[Game Object]] are distinct from the actual traits of that Game Object, which may be modified by subsequent applied Layer effects. ^cr-479-1-c

<details class="rule-ref"><summary title="Core rule 479.1.c · PDF page 107" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.1.c · PDF page 107</div></details>

Effects for this layer can be identified by the phrase "[[Copy|copy]]" in the text. ^cr-479-1-d

**Example:** Svellsongur is an [[Equipment]] that reads in part “As this is [[Attached|attached]] to a [[Unit|unit]], [[Copy|copy]] that unit's text to this Equipment's [[Effect Text|effect text]] for as long as this is attached to it.” This is a copy effect that is applied in this layer.

<details class="rule-ref"><summary title="Core rule 479.1.d · PDF page 107-108" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.1.d · PDF page 107-108</div></details>

### 2. Trait-Altering Effects

^cr-479-2

<details class="rule-ref"><summary title="Core rule 479.2 · PDF page 108" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.2 · PDF page 108</div></details>

This layer deals with effects that grant, remove, or replace inherent traits of [[Game Object|Game Objects]]. [[Card Name|Name]] [[Supertype]] Type Tags Controller [[Costs|Cost]] [[Domain]] [[Base Might]] Base Might Bonus ^cr-479-2-a

<details class="rule-ref"><summary title="Core rule 479.2.a · PDF page 108" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.2.a · PDF page 108</div></details>

Effects for this layer can be identified by the phrase "become(s)", "give," "is," or "are" in the text. ^cr-479-2-b

**Example:** A [[Permanent|permanent]] has the [[Ability|ability]] "Other [[Friendly|friendly]] [[Unit|units]] are Yordles." Other friendly units gain the Yordle [[Tag|tag]] in this layer.

<details class="rule-ref"><summary title="Core rule 479.2.b · PDF page 108" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.2.b · PDF page 108</div></details>

### 3. Ability-Altering Effects

^cr-479-3

<details class="rule-ref"><summary title="Core rule 479.3 · PDF page 108" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.3 · PDF page 108</div></details>

This layer deals with non-Copy effects that grant, remove, or replace the [[Ability|abilities]] or [[Rules Text|rules text]] of [[Game Object|Game Objects]]. [[Keywords]] [[Passive Ability|Passive Abilities]] Appending rules text Removing rules text [[Effect Text]] ^cr-479-3-a

<details class="rule-ref"><summary title="Core rule 479.3.a · PDF page 108" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.3.a · PDF page 108</div></details>

Effects for this layer can be identified by the phrase "become(s)," "give," "lose(s)," "have," "has," "is," or "are" in the text. ^cr-479-3-b

**Example:** A [[Permanent|permanent]] has the [[Ability|ability]] "Other [[Friendly|friendly]] [[Unit|units]] have &#91;[[Vision]]&#93;." Other friendly units gain the Vision [[Keywords|keyword]] in this layer.

<details class="rule-ref"><summary title="Core rule 479.3.b · PDF page 108" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.3.b · PDF page 108</div></details>

[[Ability|Abilities]] of [[Effect Text]] of [[Attached]] [[Card|cards]] are appended in this layer. ^cr-479-3-c

<details class="rule-ref"><summary title="Core rule 479.3.c · PDF page 108" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.3.c · PDF page 108</div></details>

### 4. Arithmetic Effects

^cr-479-4

<details class="rule-ref"><summary title="Core rule 479.4 · PDF page 108" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.4 · PDF page 108</div></details>

This layer deals with the mathematics of increasing and decreasing the numeric values of the traits of [[Game Object|Game Objects]]. [[Might]] [[Energy Cost]] [[Power Cost]] ^cr-479-4-a

<details class="rule-ref"><summary title="Core rule 479.4.a · PDF page 108" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.4.a · PDF page 108</div></details>

When an arithmetic effect from a source that is not a [[Passive Ability|passive ability]] has a limitation that applies, it is limited at the time of its application, and is “remembered” at that limited [[Level|level]] for the duration of its effect. This process is called “snapshotting.” ^cr-479-4-b

**Example:** If an effect gives a [[Unit|unit]] “-4 &#91;M&#93; to a min of 1 this [[Turn|turn]]” choosing a unit with 2 &#91;M&#93;, then the effect will generate -1 &#91;M&#93; this turn.

**Example:** A [[Unit|unit]] reads “Units you [[Control|control]] here have their [[Might]] increased to 5 &#91;M&#93;.” This is a [[Passive Ability|passive ability]], so it will not snapshot.

**Example:** A [[Spell|spell]] reads “Increase a [[Friendly|friendly]] [[Unit|unit]]’s [[Might]] to 5 &#91;M&#93;.” This effect is applied once, with an unlimited duration. Because it isn’t from a [[Passive Ability|passive ability]], it will snapshot.

<details class="rule-ref"><summary title="Core rule 479.4.b · PDF page 108" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.4.b · PDF page 108</div></details>

Players cannot increase a numeric attribute by a negative amount. If an effect would instruct a player to do so, they increase it by 0 instead. ^cr-479-4-c

**Example:** A player plays Last Stand, which reads “Double a [[Friendly|friendly]] [[Unit|unit]]'s [[Might]] this [[Turn|turn]]. Give it [[Temporary]].” The player declares a 2 &#91;M&#93; unit as the target during finalization. In reaction to Last Stand, an opponent plays Eclipse [[Targeting|targeting]] the 2 &#91;M&#93; unit. When Last Stand resolves, the unit is -2 &#91;M&#93;. Last Stand instructs its controller to increase the unit’s Might by its current amount, -2, when the double action is performed. This is not possible, so the unit’s Might is increased by 0 instead.

<details class="rule-ref"><summary title="Core rule 479.4.c · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.4.c · PDF page 109</div></details>

[[Might Bonus|Might Bonuses]] of [[Attached]] [[Card|cards]] are applied in this layer. ^cr-479-4-d

<details class="rule-ref"><summary title="Core rule 479.4.d · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.4.d · PDF page 109</div></details>

This layer applies arithmetic in the following way. ^cr-479-4-e

<details class="rule-ref"><summary title="Core rule 479.4.e · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.4.e · PDF page 109</div></details>

1. Increases ^cr-479-4-e-1

<details class="rule-ref"><summary title="Core rule 479.4.e.1 · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.4.e.1 · PDF page 109</div></details>

Positive values, or increases, to [[Might]] are applied first. ^cr-479-4-e-1-a

<details class="rule-ref"><summary title="Core rule 479.4.e.1.a · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.4.e.1.a · PDF page 109</div></details>

If there is a restriction or limitation to this increase and it isn’t from a [[Passive Ability|passive ability]], the limitation is “snapshotted” for the duration of the effect. ^cr-479-4-e-1-b

<details class="rule-ref"><summary title="Core rule 479.4.e.1.b · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.4.e.1.b · PDF page 109</div></details>

2. Decreases ^cr-479-4-e-2

<details class="rule-ref"><summary title="Core rule 479.4.e.2 · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.4.e.2 · PDF page 109</div></details>

Negative values, or decreases, to [[Might]] are applied last. ^cr-479-4-e-2-a

<details class="rule-ref"><summary title="Core rule 479.4.e.2.a · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.4.e.2.a · PDF page 109</div></details>

If there is a restriction or limitation to this decrease and it isn’t from a [[Passive Ability|passive ability]], the limitation is “snapshotted” for the duration of the effect. ^cr-479-4-e-2-b

<details class="rule-ref"><summary title="Core rule 479.4.e.2.b · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.4.e.2.b · PDF page 109</div></details>

Effects for this layer can be identified by the phrase "give,” “[[Swap|swap]],” "increase," "decrease," "[[Costs|cost]] … less," "cost … more," "-X,” or “+X,” in the text. ^cr-479-4-f

**Example:** An effect says “I [[Costs|cost]] &#91;1&#93; less for each [[Card|card]] you've played this [[Turn|turn]], to a minimum of &#91;1&#93;.” The cost is modified in this layer.

<details class="rule-ref"><summary title="Core rule 479.4.f · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 479.4.f · PDF page 109</div></details>

If more than one effect applies to the same [[Game Object]] in the Same Layer, or to each other in the same layer, then both effects will apply but their order may be determined by [[Dependency]]. ^cr-480

<details class="rule-ref"><summary title="Core rule 480 · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 480 · PDF page 109</div></details>

A [[Dependency]] is established if: ^cr-480-1

<details class="rule-ref"><summary title="Core rule 480.1 · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 480.1 · PDF page 109</div></details>

Applying one of the effects alters the existence of the other; or ^cr-480-1-a

<details class="rule-ref"><summary title="Core rule 480.1.a · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 480.1.a · PDF page 109</div></details>

Applying one of the effects alters the number of objects the other effect can influence; or ^cr-480-1-b

<details class="rule-ref"><summary title="Core rule 480.1.b · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 480.1.b · PDF page 109</div></details>

Applying one of the effects alters the outcome when applying the other. ^cr-480-1-c

<details class="rule-ref"><summary title="Core rule 480.1.c · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 480.1.c · PDF page 109</div></details>

To determine which effect Depends on another, determine which of the prior criteria applies, and then also which effect’s evaluation is altered by the sequence of applications. That effect is said to Depend on the other. ^cr-481

**Example:** A [[Unit|unit]] with 4 &#91;M&#93; is under the effects of a [[Passive Ability|passive ability]] that reads “Units you [[Control|control]] here have their [[Might]] increased to 5 &#91;M&#93;.” Its controller plays Discipline on the unit, giving it +2 &#91;M&#93;. When applying Layer alterations, both effects are applied in the same layer. If we apply the passive ability first, the passive ability will give +1 &#91;M&#93; while the Discipline effect will give +2 &#91;M&#93;. If we apply them in the other order, the Discipline effect will give +2 &#91;M&#93;, and the passive ability will give +0 &#91;M&#93;. The passive ability is altered by the sequence of applications, so it depends on the Discipline effect.

<details class="rule-ref"><summary title="Core rule 481 · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 481 · PDF page 109</div></details>

If both effects are altered by the application of the other, no [[Dependency]] can be established. ^cr-481-1

**Example:** A [[Unit|unit]] with 4 &#91;M&#93; is under the effects of a [[Passive Ability|passive ability]] that reads “Units you [[Control|control]] here have their [[Might]] increased to 5 &#91;M&#93;.” Its controller plays a [[Spell|spell]] that reads “Give a unit +2 &#91;M&#93;, to a maximum of 5 &#91;M&#93;.” If we apply the passive ability first, the passive ability will apply +1 &#91;M&#93; and the spell effect will apply +0 &#91;M&#93;. If we apply the spell effect first, it will apply +1 &#91;M&#93; while the passive ability applies +0 &#91;M&#93;. Both effects are altered by the sequence of applications, so we can’t establish a [[Dependency|dependency]].

<details class="rule-ref"><summary title="Core rule 481.1 · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 481.1 · PDF page 109</div></details>

To resolve a [[Dependency|dependency]], the effects within the same layer that created the dependency must be applied such that: 1. Identify which effect Depends on the other within the Layer. 2. Apply the effect that is depended on first. 3. Immediately apply the effect that Depends on the first effect next. ^cr-481-2

**Example:** A [[Unit|unit]] with 4&#91;M&#93; is under the effects of a [[Passive Ability|passive ability]] that reads “Units you [[Control|control]] here have their [[Might]] increased to 5 &#91;M&#93;.” Its controller plays Discipline on the unit. As previously established, the passive ability depends on the Discipline effect. We apply the Discipline effect first, giving the unit +2 &#91;M&#93;, and then immediately apply the passive ability that depends on it. The unit’s final Might is 6 &#91;M&#93;.

<details class="rule-ref"><summary title="Core rule 481.2 · PDF page 110" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 481.2 · PDF page 110</div></details>

If more than one effect applies to the same [[Game Object]] in the same layer but no [[Dependency|dependency]] is established, then Timestamp order is applied to the effects within that layer and sublayer ^cr-482

<details class="rule-ref"><summary title="Core rule 482 · PDF page 110" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 482 · PDF page 110</div></details>

When an effect begins applying, it establishes a time for which it is compared against other [[Game Effect|Game Effects]] for purposes of resolving Layered effects as its Timestamp. ^cr-482-1

<details class="rule-ref"><summary title="Core rule 482.1 · PDF page 110" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 482.1 · PDF page 110</div></details>

Timestamps are not rote values. ^cr-482-1-a

<details class="rule-ref"><summary title="Core rule 482.1.a · PDF page 110" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 482.1.a · PDF page 110</div></details>

Timestamps are relative comparisons between effects and when they began applying to the game. ^cr-482-1-b

<details class="rule-ref"><summary title="Core rule 482.1.b · PDF page 110" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 482.1.b · PDF page 110</div></details>

Timestamps are not referenced by [[Game Effect|Game Effects]] in any way. They are only used to finalize layered effects. ^cr-482-1-c

<details class="rule-ref"><summary title="Core rule 482.1.c · PDF page 110" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 482.1.c · PDF page 110</div></details>

When [[Rules Text]] becomes [[Inactive]] for any reason, it loses its Timestamp. When it ceases to be Inactive, a new Timestamp is established. ^cr-482-2

<details class="rule-ref"><summary title="Core rule 482.2 · PDF page 110" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 482.2 · PDF page 110</div></details>

Effects are applied such that the earliest Timestamp within each Layer and Sublayer applies first, followed by other Effects in that Layer and Sublayer in chronological order. ^cr-482-3

<details class="rule-ref"><summary title="Core rule 482.3 · PDF page 110" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 482.3 · PDF page 110</div></details>

## Related concepts

[[Ability]] · [[Ability-Altering Effects]] · [[Attached]] · [[Base Might]] · [[Battlefield]] · [[Buffs]] · [[Card]] · [[Card Name]] · [[Chain]] · [[Combat]] · [[Control]] · [[Copy]] · [[Copy Effects]] · [[Costs]] · [[Defender]] · [[Deflect]] · [[Dependency]] · [[Domain]] · [[Effect Text]] · [[Enemy]] · [[Energy Cost]] · [[Equipment]] · [[Flavor Text]] · [[Friendly]] · [[Game Effect]] · [[Game Object]] · [[Ganking]] · [[Hold Effect]] · [[In Combat]] · [[Inactive]] · [[Keywords]] · [[Level]] · [[Might]] · [[Might Bonus]] · [[Mighty]] · [[Passive Ability]] · [[Permanent]] · [[Play]] · [[Power]] · [[Power Cost]] · [[Printed Might]] · [[Rules Text]] · [[Shield]] · [[Spell]] · [[Supertype]] · [[Swap]] · [[Tag]] · [[Targeting]] · [[Temporary]] · [[Token]] · [[Turn]] · [[Unit]] · [[Vision]]

## Other rules documents

[[Tournament Rules|Tournament Rules]]

<!-- tournament-links:start -->
## Tournament Rules

[[Sleeves]]

<!-- tournament-links:end -->
