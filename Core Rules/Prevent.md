---
title: "Prevent"
type: core-topic
rules_document: Core Rules
source_version: "2026-10-09"
cssclasses:
  - riftbound-rules
---

# Prevent

[[Start Here|Home]] · [[Concept Index|Find a concept]] · [[Core Rules Index|Core rules]]

<span title="Core rule 438"></span> ^cr-438

<details class="rule-ref"><summary title="Core rule 438 · PDF page 93" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438 · PDF page 93</div></details>

Preventing [[Damage|damage]] is the act of reducing the Damage a set of [[Game Object|game objects]] would take. ^cr-438-1

<details class="rule-ref"><summary title="Core rule 438.1 · PDF page 93" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.1 · PDF page 93</div></details>

Prevent is an action that interacts with [[Damage]]. ^cr-438-1-a

<details class="rule-ref"><summary title="Core rule 438.1.a · PDF page 93" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.1.a · PDF page 93</div></details>

Prevent includes any applied [[Bonus Damage]] when determining the total [[Damage|damage]] being prevented. ^cr-438-1-a-1

<details class="rule-ref"><summary title="Core rule 438.1.a.1 · PDF page 93" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.1.a.1 · PDF page 93</div></details>

Prevent appears in statements that define an amount of [[Damage|damage]] and the source of the damage it will affect, as well as the timespan it will be relevant for. ^cr-438-1-b

<details class="rule-ref"><summary title="Core rule 438.1.b · PDF page 93" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.1.b · PDF page 93</div></details>

Prevent actions are usually formatted as “Prevent the next X &#91;source&#93; [[Damage|damage]] that would be dealt to a &#91;[[Unit|unit]]&#93; this [[Turn|turn]].” ^cr-438-1-b-1

<details class="rule-ref"><summary title="Core rule 438.1.b.1 · PDF page 93" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.1.b.1 · PDF page 93</div></details>

The X is referred to as the Prevent Value. ^cr-438-1-b-1-a

<details class="rule-ref"><summary title="Core rule 438.1.b.1.a · PDF page 93" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.1.b.1.a · PDF page 93</div></details>

X can be “All,” which specifies an infinite amount of [[Damage|damage]]. ^cr-438-1-b-1-b

<details class="rule-ref"><summary title="Core rule 438.1.b.1.b · PDF page 93" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.1.b.1.b · PDF page 93</div></details>

Prevent will always apply to the next [[Damage|damage]] that would be dealt to a [[Unit|unit]] affected by the Prevent action. ^cr-438-1-b-2

<details class="rule-ref"><summary title="Core rule 438.1.b.2 · PDF page 93" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.1.b.2 · PDF page 93</div></details>

When [[Damage|damage]] is Prevented, it is replaced with an event where the source of the damage deals that much damage reduced by the Prevent Value tracked on the [[Unit]] specifically. ^cr-438-2

<details class="rule-ref"><summary title="Core rule 438.2 · PDF page 93" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.2 · PDF page 93</div></details>

The [[Damage|damage]] being dealt as a result of Preventing can never be less than 0, but can be 0. This is equivalent to not dealing damage. ^cr-438-2-a

<details class="rule-ref"><summary title="Core rule 438.2.a · PDF page 93" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.2.a · PDF page 93</div></details>

When [[Damage|damage]] is dealt this way, reduce the Prevent Value being tracked on the [[Unit]] affected by the Prevent action by the prevented amount. ^cr-438-3

<details class="rule-ref"><summary title="Core rule 438.3 · PDF page 94" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.3 · PDF page 94</div></details>

If the Prevent Value is 0 or less, then Prevent is no longer being tracked on the [[Unit]] in question, and the effect expires. ^cr-438-3-a

<details class="rule-ref"><summary title="Core rule 438.3.a · PDF page 94" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.3.a · PDF page 94</div></details>

The reduced value is the newly tracked Prevent Value. ^cr-438-3-b

<details class="rule-ref"><summary title="Core rule 438.3.b · PDF page 94" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.3.b · PDF page 94</div></details>

If the Prevent Value is “All” then it remains “All.” ^cr-438-3-c

<details class="rule-ref"><summary title="Core rule 438.3.c · PDF page 94" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.3.c · PDF page 94</div></details>

[[Damage]] dealt to a [[Unit]] that has that all of that damage Prevented is not considered to have been dealt to it at all. ^cr-438-4

<details class="rule-ref"><summary title="Core rule 438.4 · PDF page 94" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.4 · PDF page 94</div></details>

[[Damage]] can still be assigned to [[Unit|Units]] [[In Combat|in combat]] that are affected by Prevent. The damage dealt as a result of that assignment will be affected by the Prevent action. ^cr-438-5

<details class="rule-ref"><summary title="Core rule 438.5 · PDF page 94" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.5 · PDF page 94</div></details>

[[Damage]] can be assigned to a [[Unit]] up to a value that would be Lethal considering the Prevent Value of all Prevent Actions on a Unit, following the normal rules for damage assignment. ^cr-438-5-a

**Example:** A [[Unit|unit]] with 2 &#91;M&#93; is being assigned [[Damage|damage]] in the [[Combat|combat]] damage step. The unit has “prevent the first 3 damage I would take each combat.” The unit would need to be assigned 5 damage in order to have [[Lethal Damage|lethal damage]] assigned to it.

<details class="rule-ref"><summary title="Core rule 438.5.a · PDF page 94" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.5.a · PDF page 94</div></details>

No amount of [[Damage|damage]] is ever considered lethal if the Prevent Value is “All.” ^cr-438-5-b

<details class="rule-ref"><summary title="Core rule 438.5.b · PDF page 94" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.5.b · PDF page 94</div></details>

Prevent is a [[Limited Action]]. ^cr-438-6

<details class="rule-ref"><summary title="Core rule 438.6 · PDF page 94" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.6 · PDF page 94</div></details>

Players may only Prevent [[Damage]] when directed to by [[Game Effect|Game Effects]]. ^cr-438-6-a

<details class="rule-ref"><summary title="Core rule 438.6.a · PDF page 94" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.6.a · PDF page 94</div></details>

Prevent is a [[Delayed Replacement]] Effect. ^cr-438-7

See [[Replacement Effect#^cr-367|Replacement Effects]] for more information.

See [[Delayed Ability#^cr-390|Delayed Abilities]] for more information.

<details class="rule-ref"><summary title="Core rule 438.7 · PDF page 94" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 438.7 · PDF page 94</div></details>

## Related concepts

[[Bonus Damage]] · [[Combat]] · [[Damage]] · [[Delayed Ability]] · [[Delayed Replacement]] · [[Game Effect]] · [[Game Object]] · [[In Combat]] · [[Lethal Damage]] · [[Limited Action]] · [[Replacement Effect]] · [[Turn]] · [[Unit]]

## Other rules documents

[[Tournament Rules|Tournament Rules]]

<!-- tournament-links:start -->
## Tournament Rules

[[Angle Shooting]] · [[Competition Roles]] · [[Display]] · [[Floor Judge]] · [[Unsporting Conduct]]

<!-- tournament-links:end -->
