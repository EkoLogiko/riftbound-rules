---
title: "Dependency"
type: concept
rules_document: Core Rules
source_version: "2026-10-09"
cssclasses:
  - riftbound-rules
aliases: ["Dependencies"]
---

# Dependency

[[Start Here|Home]] · [[Concept Index|Find a concept]]

## From Layers

![[Layers#^cr-480]]

<details class="rule-ref"><summary title="Core rule 480 · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 480 · PDF page 109</div></details>

![[Layers#^cr-480-1]]

<details class="rule-ref"><summary title="Core rule 480.1 · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 480.1 · PDF page 109</div></details>

![[Layers#^cr-480-1-a]]

<details class="rule-ref"><summary title="Core rule 480.1.a · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 480.1.a · PDF page 109</div></details>

![[Layers#^cr-480-1-b]]

<details class="rule-ref"><summary title="Core rule 480.1.b · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 480.1.b · PDF page 109</div></details>

![[Layers#^cr-480-1-c]]

<details class="rule-ref"><summary title="Core rule 480.1.c · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 480.1.c · PDF page 109</div></details>

## From Layers

![[Layers#^cr-481]]

Example: A [[Unit|unit]] with 4 &#91;M&#93; is under the effects of a [[Passive Ability|passive ability]] that reads “Units you [[Control|control]] here have their [[Might]] increased to 5 &#91;M&#93;.” Its controller plays Discipline on the unit, giving it +2 &#91;M&#93;. When applying Layer alterations, both effects are applied in the same layer. If we apply the passive ability first, the passive ability will give +1 &#91;M&#93; while the Discipline effect will give +2 &#91;M&#93;. If we apply them in the other order, the Discipline effect will give +2 &#91;M&#93;, and the passive ability will give +0 &#91;M&#93;. The passive ability is altered by the sequence of applications, so it depends on the Discipline effect.

<details class="rule-ref"><summary title="Core rule 481 · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 481 · PDF page 109</div></details>

![[Layers#^cr-481-1]]

Example: A [[Unit|unit]] with 4 &#91;M&#93; is under the effects of a [[Passive Ability|passive ability]] that reads “Units you [[Control|control]] here have their [[Might]] increased to 5 &#91;M&#93;.” Its controller plays a [[Spell|spell]] that reads “Give a unit +2 &#91;M&#93;, to a maximum of 5 &#91;M&#93;.” If we apply the passive ability first, the passive ability will apply +1 &#91;M&#93; and the spell effect will apply +0 &#91;M&#93;. If we apply the spell effect first, it will apply +1 &#91;M&#93; while the passive ability applies +0 &#91;M&#93;. Both effects are altered by the sequence of applications, so we can’t establish a dependency.

<details class="rule-ref"><summary title="Core rule 481.1 · PDF page 109" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 481.1 · PDF page 109</div></details>

![[Layers#^cr-481-2]]

Example: A [[Unit|unit]] with 4&#91;M&#93; is under the effects of a [[Passive Ability|passive ability]] that reads “Units you [[Control|control]] here have their [[Might]] increased to 5 &#91;M&#93;.” Its controller plays Discipline on the unit. As previously established, the passive ability depends on the Discipline effect. We apply the Discipline effect first, giving the unit +2 &#91;M&#93;, and then immediately apply the passive ability that depends on it. The unit’s final Might is 6 &#91;M&#93;.

<details class="rule-ref"><summary title="Core rule 481.2 · PDF page 110" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 481.2 · PDF page 110</div></details>

## From Layers

![[Layers#^cr-482]]

<details class="rule-ref"><summary title="Core rule 482 · PDF page 110" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 482 · PDF page 110</div></details>

![[Layers#^cr-482-1]]

<details class="rule-ref"><summary title="Core rule 482.1 · PDF page 110" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 482.1 · PDF page 110</div></details>

![[Layers#^cr-482-1-a]]

<details class="rule-ref"><summary title="Core rule 482.1.a · PDF page 110" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 482.1.a · PDF page 110</div></details>

![[Layers#^cr-482-1-b]]

<details class="rule-ref"><summary title="Core rule 482.1.b · PDF page 110" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 482.1.b · PDF page 110</div></details>

![[Layers#^cr-482-1-c]]

<details class="rule-ref"><summary title="Core rule 482.1.c · PDF page 110" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 482.1.c · PDF page 110</div></details>

![[Layers#^cr-482-2]]

<details class="rule-ref"><summary title="Core rule 482.2 · PDF page 110" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 482.2 · PDF page 110</div></details>

![[Layers#^cr-482-3]]

<details class="rule-ref"><summary title="Core rule 482.3 · PDF page 110" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 482.3 · PDF page 110</div></details>

## Related concepts

[[Control]] · [[Game Effect]] · [[Game Object]] · [[Inactive]] · [[Layers]] · [[Might]] · [[Passive Ability]] · [[Rules Text]] · [[Spell]] · [[Unit]]

## Other rules documents

[[Tournament Rules|Tournament Rules]]
