# Tournament Sources and Editorial Notes

[[Start Here|Home]] · [[Tournament Rules|Tournament rules]]

## Source

[[Sources/RiftboundTournamentRulesRUP5_en_EN.pdf|Riftbound Tournament Rules PDF]], last updated 9 October 2026, 53 pages. The vault reflects this supplied document, including its dated card-legality and release information. Its original link to the official rules hub is preserved.

## Completeness and structure

All **975 numbered entries** are retained across **56 tournament topic notes**, with **84 additional concept pages**. Definitions, examples, procedures, infractions, remedies, penalties, and the Disciplinary Code are included. Rule wording and capitalization are preserved; line wrapping, headings, and cross-reference presentation are adapted for reading. Related links are navigation aids.

Each passage has a ⓘ reference widget containing its Tournament rule number and source PDF page. Hover on desktop, or expand it by tapping on mobile. Core and Tournament references use distinct hidden anchor prefixes, so identical numbers from the two documents cannot collide.

One Shuffling subrule is printed with a missing separator in its source label. The original printed label is retained in its tooltip and manifest, with a distinct block anchor. One copied label before the Limited deck-construction text is omitted from readable prose and retained in the manifest.

## Cross-reference repairs

Several source references point to absent or mismatched passages. Navigation links are repaired for floor-judge responsibilities, General Error remedies, Final Point restrictions, team private information, and the Sealed registration step range. Original labels and repaired targets are recorded in `Maintenance/tournament-rules-manifest.json`. References without a precise documented target use the nearest existing parent passage and are also logged. These navigation repairs do not change the game-rule or policy wording.

## Integration with Core Rules

Existing notes now have clearly labelled Tournament Rules links. Their original core passages are preserved. Tournament-specific notes have `rules_document: Tournament Rules`, while core notes keep their original document metadata. Follow [[Tournament Introduction]] for the supplied document's precedence rules; the two sources are not silently merged.

## Maintenance and verification

`Maintenance/tournament-rules-manifest.json` stores every original extracted passage, destination note, unique hidden block identifier, PDF page, source hash, and reference repair. The combined validation report records coverage and link checks. The tooltip mechanism uses the existing CSS snippet and ordinary HTML; it requires no community plugin. Rendering in the user's mobile Obsidian installation has not been tested.
