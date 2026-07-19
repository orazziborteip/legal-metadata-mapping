# Legal metadata mapping for EU Data-Space and AI training governance

This repository contains the selected publication dataset supporting my thesis: *From lawful access to accountable training: Translating EU data regulation into machine-readable metadata for AI training data in Common European Data Spaces*.

The release documents a bounded legal corpus and the technical specifications assessed in the thesis. It is intended to make the principal source selection, extracted normative statements, and standards evidence inspectable without publishing the complete working research archive.

## Dataset at a glance

| Population | Records |
|---|---:|
| Registered legal sources | 7 |
| Provision and supporting units | 368 |
| Atomic normative statements | 145 |
| Assessed standards and specifications | 12 |
| Assessed standard components | 156 |

The 145 normative statements are the principal scientific population. Definitions, recitals, and related provisions are retained in `provisions.csv` where they are necessary for source traceability or interpretation; they are not counted as additional normative statements.

## Repository structure

```text
README.md
LICENSE

docs/
  methodology.md
  corpus_scope.md
  data_dictionary.md

data/
  sources/
    legal_sources.csv
  legal_corpus/
    provisions.csv
    normative_statements.csv
  standards/
    standards.csv
    standard_elements.csv
  results/
    corpus_by_instrument.csv
```

## Scope and interpretation

The dataset records an authorial research analysis of selected sources. Inclusion does not establish that every retained provision applies to a particular organisation, system, model, dataset, or operation. Likewise, the presence of a standard or metadata element does not establish legal applicability, factual accuracy, authority, fitness, compliance, or endorsement of the specification as a whole.

The study is complete within its declared corpus, but the corpus is purposive rather than exhaustive. The 145 normative statements constitute the bounded evidentiary basis for developing and applying the method; they are not a closed catalogue of all EU rules potentially relevant to data access and AI training, especially in an evolving regulatory landscape. The same method can be extended to additional provisions, instruments, standards, and use configurations, provided that each extension repeats the necessary source selection, legal analysis, extraction, and authorial validation. Such extensions may add to or qualify the resulting framework.

## Citation

## Licence

Except for the third-party material identified in the licence notice, the original dataset records and documentation are licensed under the [Creative Commons Attribution 4.0 International licence](LICENSE).

The licence does not relicense legislation, official documents, standards, specifications, trademarks, or other third-party material. Their identifiers, titles, short excerpts, and source links remain subject to the rights and reuse conditions of their respective issuers.
