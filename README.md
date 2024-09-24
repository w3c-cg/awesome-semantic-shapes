# Awesome Semantic Shapes [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of Semantic Shapes resources. Contributions welcome!
> Please, read the [Contribution Guidelines](CONTRIBUTING.md) first.

Semantic shapes enable you to validate RDF graphs against a set of conditions.
Semantic shapes can also be viewed as a description of data graphs that satisfy these conditions.
Such descriptions may be used for a variety of purposes beside validation,
including user interface building, code generation and data integration.
Semantic shapes could be described in SHACL or ShEx languages.

## Contents

- [SHACL Validators](#shacl-validators)
- [ShEx Validators](#shex-validators)
- [Shapes Discovery Tools](#shapes-discovery-tools)
- [Shapes Collections](#shapes-collections)
- [Shape Conversion Tools](#shape-conversion-tools)
- [Shape Generators](#shape-generators)
- [Shape Editors, Visualizations](#shape-editors-visualizations)
- [Declarative UIs](#declarative-uis)
- [IDE support](#ide-support)
- [Book](#book)
- [Tutorials](#tutorials)
- [Presentations](#presentations)
- [Specifications](#specifications)
- [Legend](#legend)

## SHACL Validators

- [Jena SHACL](https://github.com/apache/jena/) ![GitHub last commit](https://img.shields.io/github/last-commit/apache/jena) `Apache-2.0` `Java` - Supports: SHACL Core, SHACL-SPARQL.
- [RDF4J SHACL Sail](https://github.com/eclipse-rdf4j/rdf4j) ![GitHub last commit](https://img.shields.io/github/last-commit/eclipse-rdf4j/rdf4j) `BSD-3-Clause` `Java`
- [TopBraid SHACL API](https://github.com/TopQuadrant/shacl) ![GitHub last commit](https://img.shields.io/github/last-commit/TopQuadrant/shacl) `BSD-3-Clause` `Java` - Based on Jena; supports: SHACL Core, SHACL-SPARQL, SHACL rules.
- [TopBraid SHACL API Extended](https://github.com/SHACL-X/shacl-x) ![GitHub last commit](https://img.shields.io/github/last-commit/SHACL-X/shacl-x) `BSD-3-Clause` `Java` - Fork of TopBraid SHACL API + added SHACL-JS based on GraalVM Polyglot.
- [SHACL for Ruby](https://github.com/ruby-rdf/shacl/) ![GitHub last commit](https://img.shields.io/github/last-commit/ruby-rdf/shacl) `BSD-3-Clause` `Ruby` - A pure-Ruby library for working with the Shape Constraint Language to validate the shape of RDF graphs.

## ShEx Validators

- [Apache Jena ShEx](https://jena.apache.org/documentation/shex/index.html) - Java.
- [shexSpec/shex.js](https://github.com/shexjs/shex.js) - [playground](http://rawgit.com/shexSpec/shex.js/master/doc/shex-simple.html) - JS.
- [ShEx-validator](https://github.com/HW-SWeL/ShEx-validator) - JS.
- [Validata](https://github.com/HW-SWeL/Validata) - [playground](http://hw-swel.github.io/Validata/) - [playground](https://www.w3.org/2015/03/ShExValidata/), JS.

## Shapes Discovery Tools

- [RDFminer](https://github.com/Wimmics/RDFminer) - Web application to automatically discover SHACL shapes representative of an RDF data graph, by Wimmics.
- [SHACL Discovery Service](https://github.com/AKSW/discover-shacl-shapes)
- [Shapes of You index](https://index.semanticscience.org/) - SPARQL queries, OWL/SKOS vocabularies, SHACL/ShEx shapes, indexed from public `git` repositories.

## Shapes Collections

- [schema.org Shapes](http://datashapes.org/schema) - Schema.org, converted to SHACL by TopQuadrant.

## Shape Conversion Tools

- [ShacShifter](https://github.com/AKSW/ShacShifter) - Python, ☠️, "shape shifter" from SHACL to other formats (currently RDForms).
- [SHACL To JSON Schema](https://github.com/comake/shacl-to-json-schema) - TS, SHACL-to-JSON-Schema translator.

## Shape Generators

- [owl2shacl](https://github.com/sparna-git/owl2shacl) - OWL-to-SHACL conversion rules.

## Shape Editors, Visualizations

- [Allotrope Shape Editor](https://gitlab.com/allotrope-open-source/shape-editor)

## Declarative UIs

Data viewers/Editors based on shapes.

- [shaperone](https://forms.hypermedia.app) - SHACL Shapes Form generator.

## IDE support

- [Linked Data Extension](https://github.com/elsevierlabs-os/linked-data) - VS Code Extension for editing RDF files with embedded SHACL validator and SPARQL engine.

## Book

- [Validating RDF Data (2018)](https://book.validatingrdf.com/)

## Tutorials

- [Shapes applications and tools - ISWC'20 Tutorial](https://www.validatingrdf.com/tutorial/iswc2020/)

## Presentations

## Specifications

- SHACL, W3C Recommendations & Notes
  - [Shapes Constraint Language (SHACL)](https://www.w3.org/TR/shacl/) - W3C Recommendation, 20 July 2017.
  - [SHACL Advanced Features](https://www.w3.org/TR/shacl-af/) - W3C Working Group Note, 08 June 2017.
  - [SHACL JavaScript Extensions](https://www.w3.org/TR/shacl-js/) - W3C Working Group Note, 08 June 2017.
  - [SHACL Test Suite and Implementation Report](https://w3c.github.io/data-shapes/data-shapes-test-suite/) - W3C Document 17 January 2024.
  - [SHACL Use Cases and Requirements](https://www.w3.org/TR/shacl-ucr/) - W3C Working Group Note 20 July 2017.

- SHACL, Community Group Latest Drafts & Notes
  - [SHACL 1.2 Core](https://w3c.github.io/shacl/shacl-core/)
  - [SHACL 1.2 SPARQL Extensions](https://w3c.github.io/shacl/shacl-sparql/)
  - [SHACL Advanced Features 1.1](https://w3c.github.io/shacl/shacl-af/)
  - [SHACL Compact Syntax](https://w3c.github.io/shacl/shacl-compact-syntax/)
  - [SHACL JavaScript Extensions](https://w3c.github.io/shacl/shacl-js/)

- ShEx
  - [Shape Expressions Language 2.1](https://shex.io/shex-semantics/index.html) - Final Community Group Report 8 October 2019.

- ShEx, Drafts
  - [P3330TM/D3 Draft Recommended Practice for Standard for Shape Expression Schemas](https://shexspec.github.io/spec/)

## Legend
☠️ — Each one denotes 5 years (e.g., ☠️☠️☠️ denotes 15 years) since last update.
💰 — Denotes closed source commercial software.
