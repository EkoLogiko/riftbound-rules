---
title: "Triggered Ability"
type: core-topic
rules_document: Core Rules
source_version: "2026-10-09"
cssclasses:
  - riftbound-rules
aliases: ["Triggered Abilities"]
---

# Triggered Ability

[[Start Here|Home]] · [[Concept Index|Find a concept]] · [[Core Rules Index|Core rules]]

<!-- flowchart-links:start -->
**Flowchart:** [[Trigger Timing Flowchart#Trigger condition check|Trigger condition check]] · [[Playing or Activating Abilities Flowchart#Playing or activating abilities|Playing or activating abilities]] · [[Combat Flowchart#Combat sequence|Combat sequence]] · [[Showdown Flowchart#Showdown loop|Showdown loop]]
<!-- flowchart-links:end -->

<span title="Core rule 382"></span> ^cr-382

<details class="rule-ref"><summary title="Core rule 382 · PDF page 67" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 382 · PDF page 67</div></details>

Triggered Abilities are repeatable effects that happen when a Condition is met. ^cr-383

<details class="rule-ref"><summary title="Core rule 383 · PDF page 67" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383 · PDF page 67</div></details>

Triggered Abilities can usually be recognized by the word "when" followed by a [[Game Action|game action]] or event; the word "at" followed by a point in time during [[Turn|the turn]] sequence; or the phrase “the &#91;Nth&#93; time” followed by a game action or event. ^cr-383-1

Examples: "When you [[Conquer|conquer]] here, you may spend a [[Buffs|buff]] to [[Draw|draw]] 1." "At the end of your [[Turn|turn]], [[Ready|ready]] 2 [[Rune|runes]]." “The first time I [[Move|move]] each turn, you may ready something else that's [[Exhaust|exhausted]].”

<details class="rule-ref"><summary title="Core rule 383.1 · PDF page 67" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.1 · PDF page 67</div></details>

The phrases that identify triggered abilities do not always appear at the beginning of sentences or [[Ability|abilities]]. ^cr-383-1-a

<details class="rule-ref"><summary title="Core rule 383.1.a · PDF page 67" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.1.a · PDF page 67</div></details>

If an [[Ability|ability]] triggers “the &#91;Nth&#93; time” something happens and that trigger condition is met multiple times simultaneously, the ability’s controller picks one of those instances to serve as the trigger condition. The ability triggers only once, due to the chosen condition. ^cr-383-1-b

**Example:** Wraith of Echoes reads “The first time another [[Friendly|friendly]] [[Unit|unit]] dies each [[Turn|turn]], [[Draw|draw]] 1.” That [[Ability|ability]] hasn’t triggered yet this turn. Two other friendly units die simultaneously (say, due to [[Combat|combat]] [[Damage|damage]]). The Wraith’s controller chooses one of those deaths to trigger Wraith’s ability.

<details class="rule-ref"><summary title="Core rule 383.1.b · PDF page 67" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.1.b · PDF page 67</div></details>

Triggered Abilities have a Condition and an Effect. ^cr-383-2

<details class="rule-ref"><summary title="Core rule 383.2 · PDF page 67" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.2 · PDF page 67</div></details>

The Condition is the clause with When, At, or the Nth Time. ^cr-383-2-a

<details class="rule-ref"><summary title="Core rule 383.2.a · PDF page 67" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.2.a · PDF page 67</div></details>

Any additional conditional statement immediately after the Condition must be true in order for the Condition to be fulfilled. Such a conditional statement is part of the Trigger Condition and not the Effect. ^cr-383-2-a-1

**Example:** Sona, Harmonious reads “At the end of your [[Turn|turn]], if I'm at a [[Battlefield|battlefield]], [[Ready|ready]] up to 4 [[Friendly|friendly]] [[Rune|runes]].” Her Trigger [[Ability]]’s Condition will be fulfilled in the [[Ending Step]], but the Triggered Ability will only be placed on the [[Chain|chain]] if she is located at a battlefield when the Condition is fulfilled. If she is removed in reaction to the triggered ability, it will still resolve.

**Example:** Loose Cannon reads “At the start of your [[Beginning Phase]], [[Draw|draw]] 1 if you have one or fewer [[Card|cards]] in your [[Hand|hand]].” The “if you have one or fewer cards in your hand” conditional statement is not immediately after the trigger condition, so it is part of the effect and not the condition.

<details class="rule-ref"><summary title="Core rule 383.2.a.1 · PDF page 67" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.2.a.1 · PDF page 67</div></details>

The Effect is the [[Instructions]] that are not part of the Condition. ^cr-383-2-b

<details class="rule-ref"><summary title="Core rule 383.2.b · PDF page 67" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.2.b · PDF page 67</div></details>

The Condition of a Trigger is evaluated after a potentially inciting event has been processed, unless the event the Condition checks is the source of the triggered ability leaving [[Board|the board]]. ^cr-383-2-c

<details class="rule-ref"><summary title="Core rule 383.2.c · PDF page 67" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.2.c · PDF page 67</div></details>

If a [[Game Object]] has a Triggered Ability that is active in a specific [[Zone|zone]], it is evaluated and subsequently triggered if it enters that zone at the same time that its Trigger’s condition is met. ^cr-383-2-c-1

**Example:** Immortal Phoenix says “When you [[Kill|kill]] a [[Unit|unit]] with a [[Spell|spell]], you may pay &#91;1&#93;&#91;C&#93; to [[Play|play]] me from your [[Trash|trash]].” This [[Ability|ability]] triggers if Immortal Phoenix is in your trash immediately after you kill a unit with a spell, even if the unit you killed with a spell was that Immortal Phoenix.

<details class="rule-ref"><summary title="Core rule 383.2.c.1 · PDF page 68" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.2.c.1 · PDF page 68</div></details>

A [[Game Object]] will not be able to successfully evaluate its Trigger Condition, however, if it leaves the [[Zone|zone]] that its Trigger is active from at the same time that its Trigger is satisfied. ^cr-383-2-c-2

**Example:** Viktor, Leader says “When another non-Recruit [[Unit|unit]] you [[Control|control]] dies, [[Play|play]] a 1 &#91;M&#93; Recruit unit [[Token|token]] into your [[Base|base]].” This [[Ability|ability]] triggers if Viktor is on [[Board|the board]] immediately after another non-Recruit unit you control dies. It does not trigger if Viktor and another non-Recruit unit you control die during the same [[Game Action|game action]] (for instance, if they are both [[Kill|killed]] in the same [[Cleanups|Cleanup]] due to the [[Damage|damage]] dealt by Unchecked [[Power]]).

<details class="rule-ref"><summary title="Core rule 383.2.c.2 · PDF page 68" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.2.c.2 · PDF page 68</div></details>

If a [[Game Object]] has a Triggered Ability whose condition is the Game Object leaving [[Board|the board]], such a Triggered Ability is processed immediately before the Game Object changes [[Zone|zones]]. ^cr-383-2-c-3

**Example:** If a [[Game Object|game object]] has a [[Deathknell|deathknell]] [[Ability|ability]], which triggers on the game object dying, it will be processed and placed on the [[Chain|chain]] just prior to the game object being placed in the [[Trash|trash]], during the event of the game object dying.

**Example:** Treasure Trove has a triggered ability that triggers as it “leaves [[Board|the board]].” Such a triggered ability is processed and placed on the [[Chain|chain]] just before Treasure Trove completes the action of leaving the board by being moved to another [[Zone|zone]].

<details class="rule-ref"><summary title="Core rule 383.2.c.3 · PDF page 68" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.2.c.3 · PDF page 68</div></details>

Triggered Abilities that trigger from [[Game Object|Game Objects]] leaving [[Board|the board]] trigger and are placed on the [[Chain|chain]] after any [[Replacement Effect|Replacement Effects]] are processed. If a Replacement Effect causes the Game Object to not leave the board in the appropriate way, the relevant Triggered Abilities will not trigger. ^cr-383-2-c-3-a

**Example:** If a [[Unit|unit]]’s death is replaced by an event of that unit being healed, [[Exhaust|exhausted]], and recalled, that unit’s [[Deathknell]] [[Ability|abilities]] will not trigger, as the unit’s death event is replaced and does not occur.

**Example:** If Treasure Trove’s being [[Kill|killed]] is replaced with it being banished, it will still trigger just before the [[Banish|banish]] action is executed.

<details class="rule-ref"><summary title="Core rule 383.2.c.3.a · PDF page 68" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.2.c.3.a · PDF page 68</div></details>

When the Triggered Ability is being processed, note any information about the source of the Triggered Ability or the state of the game as needed in order to process the resulting Triggered Ability. ^cr-383-2-c-3-b

**Example:** A [[Unit|unit]] reads in part “When I leave [[Board|the board]], [[Deal|deal]] 2 to a unit where I was.” Its controller plays Retreat on the unit, returning it to [[Hand|hand]]. Before the unit is returned to hand, the triggered ability is placed on the [[Chain|chain]] and the necessary information about that unit is noted. When the triggered ability is being finalized, we can identify the former [[Location|location]] of the unit in question with the noted information.

<details class="rule-ref"><summary title="Core rule 383.2.c.3.b · PDF page 68" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.2.c.3.b · PDF page 68</div></details>

When a Condition is met, a Triggered Ability behaves like an [[Activated Ability]] and is placed on the [[Chain]]. ^cr-383-3

<details class="rule-ref"><summary title="Core rule 383.3 · PDF page 68" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.3 · PDF page 68</div></details>

If a Triggered Ability says “you may”or “they may” as the first part of its Effect, the controller of its source will choose whether or not to perform the Triggered Ability during finalization. ^cr-383-3-a

**Example:** Tideturner reads “When you [[Play|play]] me, you may choose a [[Unit|unit]] you [[Control|control]] at another [[Location|location]]. [[Move]] me to its location and it to my original location.” This “you may” appears as the first part of its effect, so the choice represents whether or not to perform the triggered ability.

<details class="rule-ref"><summary title="Core rule 383.3.a · PDF page 69" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.3.a · PDF page 69</div></details>

The decision of “may” when it appears in this way is solely whether or not to perform said triggered ability. ^cr-383-3-a-1

<details class="rule-ref"><summary title="Core rule 383.3.a.1 · PDF page 69" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.3.a.1 · PDF page 69</div></details>

If the controller of the Triggered Ability chooses not to perform that Triggered Ability during finalization, it is removed from the [[Chain|chain]] and considered to have not triggered. ^cr-383-3-a-2

<details class="rule-ref"><summary title="Core rule 383.3.a.2 · PDF page 69" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.3.a.2 · PDF page 69</div></details>

If “you may” or “they may” appears in any later part of the Effect of a triggered ability, it is decided on resolution. ^cr-383-3-a-3

**Example:** Ornn, Blacksmith reads “When you [[Play|play]] me or when I [[Hold|hold]], look at the top 4 [[Card|cards]] of your [[Main Deck]]. You may [[Reveal|reveal]] a [[Gear|gear]] from among them and [[Draw|draw]] it. Then [[Recycle|recycle]] the rest.” This “you may” does not appear as the first part of its effect, so the choice is made on resolution. The [[Ability|ability]] is always finalized to the [[Chain|chain]].

<details class="rule-ref"><summary title="Core rule 383.3.a.3 · PDF page 69" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.3.a.3 · PDF page 69</div></details>

If a Triggered Ability contains a [[Costs|cost]] within [[Instructions|instructions]] at the beginning of the effect or immediately following the “you may” or “they may” that appears as the first part of the effect, that cost is treated as the [[Base Cost|base cost]] of the Triggered Ability. ^cr-383-3-b

**Example:** Ekko, Recurrent reads “&#91;[[Deathknell]]&#93;&#91;>&#93; [[Recycle]] me to [[Ready|ready]] your [[Rune|runes]].” In this case, “recycle me to ready your runes” is a [[Costs|cost]] within [[Instructions|instructions]] that appears at the beginning of the effect of the [[Ability|ability]], and thus “recycle me” is taken as the [[Base Cost|base cost]] of the triggered ability.

**Example:** Insightful Investigator reads “When you [[Play|play]] me, choose an opponent. They [[Reveal|reveal]] their [[Hand|hand]]. You may pay 2 XP to choose a [[Card|card]] from their hand. If you do, they [[Discard|discard]] that card and [[Draw|draw]] 1.” The “pay 2 XP” is a [[Costs|cost]] within [[Instructions|instructions]], but because it does not appear in the first part of the effect, it is not taken as the [[Base Cost|base cost]] of the triggered ability. Paying 2 XP is performed on resolution.

<details class="rule-ref"><summary title="Core rule 383.3.b · PDF page 69" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.3.b · PDF page 69</div></details>

The [[Costs|cost]] must be paid in order to finalize the Triggered Ability to the [[Chain]]. ^cr-383-3-b-1

<details class="rule-ref"><summary title="Core rule 383.3.b.1 · PDF page 69" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.3.b.1 · PDF page 69</div></details>

Triggered Abilities can be put on the [[Chain]] during Closed States or Open States on any player's [[Turn|turn]]. ^cr-383-3-c

<details class="rule-ref"><summary title="Core rule 383.3.c · PDF page 69" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.3.c · PDF page 69</div></details>

If more than one Triggered Ability is Triggered simultaneously, then the player that controls the [[Ability|Abilities]] selects the order to place them on the [[Chain]]. ^cr-383-3-d

<details class="rule-ref"><summary title="Core rule 383.3.d · PDF page 69" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.3.d · PDF page 69</div></details>

If multiple players separately [[Control|control]] Triggered Abilities that are Triggered simultaneously, then starting with [[Turn|the Turn]] Player and proceeding in Turn Order, each player orders their Triggered Abilities on the [[Chain]]. ^cr-383-3-d-1

<details class="rule-ref"><summary title="Core rule 383.3.d.1 · PDF page 69" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.3.d.1 · PDF page 69</div></details>

Some Triggered Abilities will trigger “once each [[Turn|turn]],” or “N times each turn.” ^cr-383-3-e

<details class="rule-ref"><summary title="Core rule 383.3.e · PDF page 69" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.3.e · PDF page 69</div></details>

Such a Triggered Ability will only be performed the specified number of times each [[Turn|turn]]. If its trigger condition would be fulfilled and it has already been performed that many times, it does not trigger. ^cr-383-3-e-1

<details class="rule-ref"><summary title="Core rule 383.3.e.1 · PDF page 69" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.3.e.1 · PDF page 69</div></details>

If the Triggered Ability says “you may” or “they may” as the first part of its effect, its controller has the choice of whether or not it is performed. ^cr-383-3-e-2

<details class="rule-ref"><summary title="Core rule 383.3.e.2 · PDF page 69" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.3.e.2 · PDF page 69</div></details>

During finalization of the Triggered Ability, the player who controls the Triggered Ability may choose to perform it. ^cr-383-3-e-2-a

<details class="rule-ref"><summary title="Core rule 383.3.e.2.a · PDF page 69" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.3.e.2.a · PDF page 69</div></details>

If they do not, it is removed from the [[Chain|chain]]. ^cr-383-3-e-2-b

**Example:** A player controls a [[Unit|unit]] that reads in part “Once each [[Turn|turn]], when an [[Enemy|enemy]] unit dies, you may [[Banish|banish]] it.” When an enemy Recruit [[Token|token]] dies, the triggered ability goes on the [[Chain|chain]]. If they choose not to perform the [[Ability|ability]] on finalization, it is removed from the chain. When a Stalwart Poro dies later in the turn, they can choose to trigger it then.

<details class="rule-ref"><summary title="Core rule 383.3.e.2.b · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.3.e.2.b · PDF page 70</div></details>

Some Conditions are commonly used and structured in a way that explicitly defines their use and other properties of the Effect that is associated with it. ^cr-383-4

<details class="rule-ref"><summary title="Core rule 383.4 · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4 · PDF page 70</div></details>

[[Play Effect|Play Effects]] are Triggered Abilities whose Condition includes the [[Permanent]] that has the Play Effect being played to [[Board|the board]]. ^cr-383-4-a

<details class="rule-ref"><summary title="Core rule 383.4.a · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.a · PDF page 70</div></details>

These are commonly structured as “When you [[Play|play]] me…” for [[Unit|Units]] and “When you play this…” for [[Gear]]. ^cr-383-4-a-1

<details class="rule-ref"><summary title="Core rule 383.4.a.1 · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.a.1 · PDF page 70</div></details>

These Triggered Abilities are put on the [[Chain]] as [[Pending Chain Item|Pending Items]] after the [[Permanent]] these effects correspond to is finalized and enters [[Board|the board]]. ^cr-383-4-a-2

<details class="rule-ref"><summary title="Core rule 383.4.a.2 · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.a.2 · PDF page 70</div></details>

These Triggered Abilities can be referred to as [[Play Effect|Play Effects]]. ^cr-383-4-a-3

<details class="rule-ref"><summary title="Core rule 383.4.a.3 · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.a.3 · PDF page 70</div></details>

[[Ability|Abilities]] that trigger when another object is played are not considered [[Play Effect|Play Effects]]. ^cr-383-4-a-4

<details class="rule-ref"><summary title="Core rule 383.4.a.4 · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.a.4 · PDF page 70</div></details>

[[Targeting Effect|Targeting Effects]] are Triggered Abilities whose Condition includes a [[Game Object]] becoming targeted. ^cr-383-4-b

<details class="rule-ref"><summary title="Core rule 383.4.b · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.b · PDF page 70</div></details>

These are commonly structured as “When you choose me …” or “When you choose a &#91;[[Game Object]]&#93; …” ^cr-383-4-b-1

<details class="rule-ref"><summary title="Core rule 383.4.b.1 · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.b.1 · PDF page 70</div></details>

These Triggered Abilities are put on the [[Chain]] as [[Pending Chain Item|Pending Items]] after a [[Spell|spell]] or [[Ability|ability]] targets an appropriate [[Game Object]]. ^cr-383-4-b-2

<details class="rule-ref"><summary title="Core rule 383.4.b.2 · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.b.2 · PDF page 70</div></details>

Although these [[Ability|abilities]] say “choose” in their Condition, they trigger specifically when an appropriate [[Game Object]] is Targeted. ^cr-383-4-b-3

See [[Process of Playing a Card#^cr-355-6|Targeting]] for more information on what counts as [[Targeting]].

<details class="rule-ref"><summary title="Core rule 383.4.b.3 · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.b.3 · PDF page 70</div></details>

These Triggered Abilities can be referred to as [[Targeting Effect|Targeting Effects]]. ^cr-383-4-b-4

<details class="rule-ref"><summary title="Core rule 383.4.b.4 · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.b.4 · PDF page 70</div></details>

[[Conquer Effect|Conquer Effects]] are Triggered Abilities whose Condition includes a [[Unit]] participating in, and successfully [[Conquer|Conquering]] a [[Battlefield]]. ^cr-383-4-c

<details class="rule-ref"><summary title="Core rule 383.4.c · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.c · PDF page 70</div></details>

These are commonly structured as “When I [[Conquer|conquer]]…” and “When you conquer…” ^cr-383-4-c-1

<details class="rule-ref"><summary title="Core rule 383.4.c.1 · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.c.1 · PDF page 70</div></details>

This [[Card Category|category]] of Triggered Abilities encompasses only those that are triggered from [[Unit|Units]] that were present during the [[Conquer]] action, or [[Ability|Abilities]] that reference the player that performed the Conquer action. ^cr-383-4-c-2

<details class="rule-ref"><summary title="Core rule 383.4.c.2 · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.c.2 · PDF page 70</div></details>

The [[Conquer]] [[Ability|Abilities]] of [[Unit|Units]] are put on the [[Chain]] as [[Pending Chain Item|Pending Items]] after the Unit(s) these effects correspond to are present at a [[Battlefield]] when a player gains [[Control|control]] of it and gains 1 Victory Point from Conquering. ^cr-383-4-c-2-a

<details class="rule-ref"><summary title="Core rule 383.4.c.2.a · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.c.2.a · PDF page 70</div></details>

The [[Conquer]] [[Ability|Abilities]] of anything that references the player Conquering are put on the [[Chain]] as [[Pending Chain Item|Pending Items]] when the Condition that the player that controls the triggering source has performed a Conquer. ^cr-383-4-c-2-b

<details class="rule-ref"><summary title="Core rule 383.4.c.2.b · PDF page 70" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.c.2.b · PDF page 70</div></details>

If the act of gaining one point from [[Conquer|Conquering]] is negated or replaced in any way, the [[Conquer Effect]] will still trigger. ^cr-383-4-c-2-c

<details class="rule-ref"><summary title="Core rule 383.4.c.2.c · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.c.2.c · PDF page 71</div></details>

These Triggered Abilities can be referred to as [[Conquer Effect|Conquer Effects]]. ^cr-383-4-c-3

<details class="rule-ref"><summary title="Core rule 383.4.c.3 · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.c.3 · PDF page 71</div></details>

[[Hold Effect|Hold Effects]] are Triggered Abilities whose Condition includes a [[Unit]] being present at a [[Battlefield]] during the [[Beginning Phase|Beginning phase]] when a player scores Victory [[Points]] from [[Hold|Holding]]. ^cr-383-4-d

<details class="rule-ref"><summary title="Core rule 383.4.d · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.d · PDF page 71</div></details>

These are commonly structured as “When I [[Hold|hold]]…” or “When you hold…” ^cr-383-4-d-1

<details class="rule-ref"><summary title="Core rule 383.4.d.1 · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.d.1 · PDF page 71</div></details>

This [[Card Category|category]] of Triggered Abilities encompasses only those that are triggered from [[Unit|Units]] that were present during the [[Hold]] action, or [[Ability|Abilities]] that reference the player that performed the Hold action. ^cr-383-4-d-2

<details class="rule-ref"><summary title="Core rule 383.4.d.2 · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.d.2 · PDF page 71</div></details>

The [[Hold]] [[Ability|Abilities]] of [[Unit|Units]] are put on the [[Chain]] as [[Pending Chain Item|Pending Items]] after the Unit these effects correspond to are present at a [[Battlefield]] when a player maintains [[Control|control]] of it and Gains 1 Victory Point during their [[Beginning Phase]] from Holding. ^cr-383-4-d-2-a

<details class="rule-ref"><summary title="Core rule 383.4.d.2.a · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.d.2.a · PDF page 71</div></details>

The [[Hold]] [[Ability|Abilities]] of anything that references the player Holding are put on the [[Chain]] as [[Pending Chain Item|Pending Items]] when the Condition that the player that controls the triggering source has performed a Hold. ^cr-383-4-d-2-b

<details class="rule-ref"><summary title="Core rule 383.4.d.2.b · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.d.2.b · PDF page 71</div></details>

If the act of gaining one point from [[Hold|Holding]] is negated or replaced in any way, the [[Hold Effect]] will still trigger. ^cr-383-4-d-2-c

<details class="rule-ref"><summary title="Core rule 383.4.d.2.c · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.d.2.c · PDF page 71</div></details>

These Triggered Abilities can be referred to as [[Hold Effect|Hold Effects]]. ^cr-383-4-d-3

<details class="rule-ref"><summary title="Core rule 383.4.d.3 · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.d.3 · PDF page 71</div></details>

[[Attack Trigger|Attack Triggers]] are Triggered Abilities that trigger when a [[Unit]] or Player gains the [[Attacker]] designation for the first time during a [[Combat|combat]]. ^cr-383-4-e

<details class="rule-ref"><summary title="Core rule 383.4.e · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.e · PDF page 71</div></details>

These are commonly structured as “When I attack…” or “When you attack…” ^cr-383-4-e-1

<details class="rule-ref"><summary title="Core rule 383.4.e.1 · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.e.1 · PDF page 71</div></details>

These Triggered Abilities are put on the [[Chain]] as [[Pending Chain Item|Pending Items]] after the [[Unit]] these effects correspond to gains the [[Attacker]] designation during [[Combat]]. ^cr-383-4-e-2

<details class="rule-ref"><summary title="Core rule 383.4.e.2 · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.e.2 · PDF page 71</div></details>

These triggers will only have their condition checked once per [[Combat|combat]], despite a [[Unit]] being able to gain and lose the [[Attacker]] designation multiple times in the same combat. ^cr-383-4-e-2-a

<details class="rule-ref"><summary title="Core rule 383.4.e.2.a · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.e.2.a · PDF page 71</div></details>

If the trigger condition contains other requirements besides [[Attacker|attacking]] and if those requirements are not fulfilled when the [[Unit|unit]] gains the Attacker designation, it will not trigger in that [[Combat|combat]]. ^cr-383-4-e-2-b

<details class="rule-ref"><summary title="Core rule 383.4.e.2.b · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.e.2.b · PDF page 71</div></details>

These Triggered Abilities can be referred to as [[Attack Trigger|Attack Triggers]]. ^cr-383-4-e-3

<details class="rule-ref"><summary title="Core rule 383.4.e.3 · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.e.3 · PDF page 71</div></details>

[[Defend Trigger|Defend Triggers]] are Triggered Abilities that trigger when a [[Unit]] or Player gains the [[Defender]] designation for the first time during a [[Combat|combat]]. ^cr-383-4-f

<details class="rule-ref"><summary title="Core rule 383.4.f · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.f · PDF page 71</div></details>

These are commonly structured as “When I defend…” or “When you defend…” ^cr-383-4-f-1

<details class="rule-ref"><summary title="Core rule 383.4.f.1 · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.f.1 · PDF page 71</div></details>

These Triggered Abilities are put on the [[Chain]] as [[Pending Chain Item|Pending Items]] after the [[Unit]] these effects correspond to gains the [[Defender]] designation during [[Combat]]. ^cr-383-4-f-2

<details class="rule-ref"><summary title="Core rule 383.4.f.2 · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.f.2 · PDF page 71</div></details>

These triggers will only have their condition checked once per [[Combat|combat]], despite a [[Unit]] being able to gain and lose the [[Defender]] designation multiple times in the same combat. ^cr-383-4-f-2-a

<details class="rule-ref"><summary title="Core rule 383.4.f.2.a · PDF page 71" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.f.2.a · PDF page 71</div></details>

If the trigger condition contains other requirements besides [[Defender|defending]] and if those requirements are not fulfilled when the [[Unit|unit]] gains the Defender designation, it will not trigger in that [[Combat|combat]]. ^cr-383-4-f-2-b

<details class="rule-ref"><summary title="Core rule 383.4.f.2.b · PDF page 72" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.f.2.b · PDF page 72</div></details>

These Triggered Abilities can be referred to as [[Defend Trigger|Defend Triggers]]. ^cr-383-4-f-3

<details class="rule-ref"><summary title="Core rule 383.4.f.3 · PDF page 72" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.f.3 · PDF page 72</div></details>

Some effects may instruct a player to “activate” one of these named triggered abilities. ^cr-383-4-g

<details class="rule-ref"><summary title="Core rule 383.4.g · PDF page 72" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.g · PDF page 72</div></details>

To do so, that player checks the condition of all of the specified effects, as if they had fulfilled the named part of the condition. ^cr-383-4-g-1

**Example:** Reckoner’s Arena reads “When you [[Hold|hold]] here, activate the [[Conquer Effect|conquer effects]] of [[Unit|units]] here.” For each unit at the [[Battlefield|battlefield]], you will check the trigger condition of their conquer effects to see if the condition has been fulfilled, treating the [[Conquer|conquer]] portion of the condition as having been fulfilled. If all of the conditions are fulfilled for a conquer effect, it is placed on the [[Chain|chain]] as if it had just triggered. If any of the non-conquer parts of the condition are not fulfilled, it will not be placed on the chain.

**Example:** A [[Spell|spell]] reads “Activate the [[Play Effect|play effects]] of your [[Gear|gear]].” For each gear you [[Control|control]], you will treat it as if you had just played the gear and check the other conditions of that gear. If all of the conditions are fulfilled for a play effect, it is placed on the [[Chain|chain]] as if it had just triggered.

<details class="rule-ref"><summary title="Core rule 383.4.g.1 · PDF page 72" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.g.1 · PDF page 72</div></details>

The named part of the condition is fulfilled, but no actual such event occurs. ^cr-383-4-g-2

**Example:** Red Brambleback is a [[Unit|unit]] that reads in part “Your [[Conquer Effect|conquer effects]] for [[Conquer|conquering]] here trigger an additional time.” Reckoner’s Arena is a [[Battlefield|battlefield]] that reads “When you [[Hold|hold]] here, activate the conquer effects of units here.” The conquer effects that were activated in this way were not the result of a conquer occurring, so they will not trigger an additional time from Red Brambleback’s [[Passive Ability|passive ability]] if it is located there.

<details class="rule-ref"><summary title="Core rule 383.4.g.2 · PDF page 72" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 383.4.g.2 · PDF page 72</div></details>

### Presence on Permanents

^cr-384

<details class="rule-ref"><summary title="Core rule 384 · PDF page 72" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 384 · PDF page 72</div></details>

Typically active while on [[Board|the Board]]. ^cr-384-1

<details class="rule-ref"><summary title="Core rule 384.1 · PDF page 72" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 384.1 · PDF page 72</div></details>

Triggered Abilities of [[Permanent|Permanents]] are only able to have their Conditions evaluated while on [[Board|the Board]]. ^cr-384-2

<details class="rule-ref"><summary title="Core rule 384.2 · PDF page 72" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 384.2 · PDF page 72</div></details>

### Presence on Cards outside of the Board

^cr-385

<details class="rule-ref"><summary title="Core rule 385 · PDF page 72" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 385 · PDF page 72</div></details>

Triggered Abilities on [[Card|cards]] outside of [[Board|the Board]] rely on the Information [[Level]] of the [[Zone|zone]] they are in. ^cr-385-1

<details class="rule-ref"><summary title="Core rule 385.1 · PDF page 72" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 385.1 · PDF page 72</div></details>

Triggered Abilities outside of [[Board|the Board]] will self-describe their context. ^cr-385-2

**Example:** The triggered ability "When you [[Conquer|conquer]], you may [[Discard|discard]] 1 to return this from your [[Trash|trash]] to your [[Hand|hand]]." triggers while the [[Card|card]] it's on is in the trash, and not anywhere else.

<details class="rule-ref"><summary title="Core rule 385.2 · PDF page 72" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 385.2 · PDF page 72</div></details>

Some [[Replacement Effect|Replacement Effects]], [[Passive Ability|Passive Abilities]], and Triggered Abilities will begin with “once each [[Turn|turn]],” “N times each turn,” “once on each of your turns,” or “N times on each of your turns.” ^cr-386

<details class="rule-ref"><summary title="Core rule 386 · PDF page 72" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 386 · PDF page 72</div></details>

Such [[Replacement Effect|Replacement Effects]] and Triggered Abilities will only be applied to the specified number of events each [[Turn|turn]], or performed the specified number of times each turn. Once they have been performed that many times or been applied to that many events, they cannot trigger or be applied to a later event in the same turn. ^cr-386-1

<details class="rule-ref"><summary title="Core rule 386.1 · PDF page 72" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 386.1 · PDF page 72</div></details>

If such a Triggered Ability says “you may,” or “they may,” as the first part of its effect, or such a [[Replacement Effect]] says a player “may” replace the qualifying event, the controller of the [[Ability|ability]] has the choice of whether or not to perform or apply it. ^cr-386-2

<details class="rule-ref"><summary title="Core rule 386.2 · PDF page 73" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 386.2 · PDF page 73</div></details>

For [[Replacement Effect|Replacement Effects]], when an event the Replacement Effect could apply to occurs, the player who controls the Replacement Effect may choose not to apply it to the event. For Triggered Abilities, during Finalization of the Triggered Ability, the player who controls the Triggered Ability may choose not to perform it. ^cr-386-2-a

<details class="rule-ref"><summary title="Core rule 386.2.a · PDF page 73" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 386.2.a · PDF page 73</div></details>

If they do not apply the [[Replacement Effect]], it has not been applied this [[Turn|turn]]. If they do not perform the Triggered Ability, it is removed from the [[Chain|chain]]. ^cr-386-2-b

**Example:** Zilean, Time mage reads “Once each [[Turn|turn]], if you would [[Play|play]] a [[Token|token]] [[Unit|unit]] while I'm at a [[Battlefield|battlefield]], you may play that token and an additional [[Copy|copy]] of it instead.” When his controller plays a token, they can choose not to apply the [[Replacement Effect|replacement effect]] to that event. If they do, they can choose to apply it to a later event of a token being played.

**Example:** A player controls a [[Unit|unit]] that reads in part “Once each [[Turn|turn]], when an [[Enemy|enemy]] unit dies, you may [[Banish|banish]] it.” When an enemy Recruit [[Token|token]] dies, the triggered ability goes on the [[Chain|chain]]. If they choose not to perform the [[Ability|ability]] on finalization, it is removed from the chain. When a Stalwart Poro dies later in the turn, they can choose to perform it then.

<details class="rule-ref"><summary title="Core rule 386.2.b · PDF page 73" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 386.2.b · PDF page 73</div></details>

For such [[Passive Ability|Passive Abilities]], they will be active until they have been applied to the specified number of events, after which point they will become [[Inactive|inactive]]. ^cr-386-3

<details class="rule-ref"><summary title="Core rule 386.3 · PDF page 73" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 386.3 · PDF page 73</div></details>

If such a [[Passive Ability]] says “you may” or “they may” as the first part of the [[Ability|ability]] after the “once each [[Turn|turn]],” the controller of the source of the Passive Ability chooses whether or not to apply the ability to the event in question. If they do not, the Passive Ability is Ignored during that event. ^cr-386-3-a

See [[Ignoring Effects#^cr-764|Ignoring Effects]] for more information.

<details class="rule-ref"><summary title="Core rule 386.3.a · PDF page 73" aria-label="Show source rule">ⓘ</summary><div class="rule-tooltip">Core rule 386.3.a · PDF page 73</div></details>

## Related concepts

[[Ability]] · [[Activated Ability]] · [[Attack Trigger]] · [[Attacker]] · [[Banish]] · [[Base]] · [[Base Cost]] · [[Battlefield]] · [[Beginning Phase]] · [[Board]] · [[Buffs]] · [[Card]] · [[Card Category]] · [[Chain]] · [[Cleanups]] · [[Combat]] · [[Conquer]] · [[Conquer Effect]] · [[Control]] · [[Copy]] · [[Costs]] · [[Damage]] · [[Deal]] · [[Deathknell]] · [[Defend Trigger]] · [[Defender]] · [[Discard]] · [[Draw]] · [[Ending Step]] · [[Enemy]] · [[Exhaust]] · [[Friendly]] · [[Game Action]] · [[Game Object]] · [[Gear]] · [[Hand]] · [[Hold]] · [[Hold Effect]] · [[Ignoring Effects]] · [[Inactive]] · [[Instructions]] · [[Kill]] · [[Level]] · [[Location]] · [[Main Deck]] · [[Move]] · [[Passive Ability]] · [[Pending Chain Item]] · [[Permanent]] · [[Play]] · [[Play Effect]] · [[Points]] · [[Power]] · [[Process of Playing a Card]] · [[Ready]] · [[Recycle]] · [[Replacement Effect]] · [[Reveal]] · [[Rune]] · [[Spell]] · [[Targeting]] · [[Targeting Effect]] · [[Token]] · [[Trash]] · [[Turn]] · [[Unit]] · [[Zone]]

## Other rules documents

[[Tournament Rules|Tournament Rules]]

<!-- tournament-links:start -->
## Tournament Rules

[[Accountable Player]] · [[Game Play Errors]] · [[Missed Trigger]] · [[Observable Impact]] · [[Tournament Triggered Abilities]]

<!-- tournament-links:end -->
