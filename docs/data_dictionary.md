# Data dictionary

This dictionary describes only the files included in the public release.

## Source file

### `data/sources/legal_sources.csv`

- `source_id`: stable source identifier.
- `instrument_title`, `instrument_short_name`, `instrument_type`: source identity and type.
- `celex_or_eli`, `official_url`: authoritative identifier and official location.
- `jurisdiction`, `issuing_body`: legal system and issuer.
- `adoption_date`, `publication_date`, `entry_into_force_date`, `general_application_date`: distinct legal dates.
- `staged_application_notes`: provision-specific or phased timing.
- `amends_or_is_amended_by`, `corrigenda`, `consolidated_version_date`: amendment and version context.
- `status_at_legal_baseline`, `status_at_source_check`: recorded source status at the declared dates.
- `source_language`: language of the inspected source.
- `verification_status`, `verified_at`: authorial source check and its date.

## Legal-corpus files

### `data/legal_corpus/provisions.csv`

- `provision_id`: stable identifier for a provision or supporting unit.
- `source_id`: parent source.
- `article`, `paragraph`, `point`: source location.
- `heading`, `stable_pinpoint`: readable heading and precise reference.
- `cross_references`: related provisions required by the retained unit.
- `definitions_required`, `recitals_required`: definitions and recitals needed for interpretation.

### `data/legal_corpus/normative_statements.csv`

- `statement_id`, `provision_id`: statement identity and parent provision.
- `source_excerpt_max_25_words`: short source excerpt retained for traceability.
- `modality`, `modality_strength`: legal function and strength.
- `addressee_actor`, `addressee_legal_role`: addressed actor and instrument-specific role.
- `action`: legally material act, omission, decision, or procedure.
- `governed_object`, `object_granularity`: regulated object and its analytical level.
- `beneficiary_or_right_holder`, `purpose`: beneficiary and legal purpose.
- `trigger_conditions`, `cumulative_or_alternative_conditions`: application logic recorded from the source.
- `exceptions_derogations`: express exception, exclusion, or qualification.
- `required_information`, `required_form_or_format`: information and presentation requirements.
- `required_control`, `required_evidence`: control and evidence implications.
- `supervisory_or_decision_actor`: supervising or deciding authority.
- `consequence_or_remedy`: bounded consequence or remedy recorded by the analysis.
- `cross_instrument_dependency`: material legal dependencies outside the parent provision.

## Standards files

### `data/standards/standards.csv`

- `standard_id`, `title`, `version`: specification identity and exact version.
- `formal_status`, `issuing_body`: status declared by the responsible issuer and the issuer's identity.
- `canonical_url`, `publication_date`: official source and publication date.
- `normative_or_informative_scope`: normative and informative scope considered in the study.
- `conformance_mechanism`: available conformance or validation mechanism.
- `machine_readable_artifacts`: namespaces, vocabularies, contexts, or validation artefacts.
- `maintenance_status`: recorded maintenance or release status.
- `limitations`: principal limitation retained in the comparison.
- `admission_disposition`: whether the specification was admitted to or deferred from the bounded comparison.

### `data/standards/standard_elements.csv`

- `standard_element_id`, `standard_id`, `version`, `formal_status`: element identity and parent specification.
- `namespace`, `class_or_property`, `human_label`: technical identifier and label.
- `normative_definition`: definition used in the comparison.
- `domain`, `range`, `cardinality`, `controlled_vocabulary`: published structural constraints, where applicable.
- `normative_or_informative`, `validation_artifact`: formal role and available validation support.
- `intended_capability`: general representational function considered in the study.
- `known_limit`: limitation retained when using the element.
- `source_pinpoint`: specification section or authoritative source location.

## Result files

### `data/results/corpus_by_instrument.csv`

- `source_id`, `instrument`: source identity.
- `registered_units`: number of retained provision and supporting units.
- `normative_statements`: number of extracted normative statements.
