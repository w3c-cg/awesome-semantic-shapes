# Awesome Semantic Shapes [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of Semantic Shapes resources. Contributions welcome!
> Please, read the [Contribution Guidelines](CONTRIBUTING.md) first.

Semantic shapes enable you to validate RDF graphs against a set of conditions.
Semantic shapes can also be viewed as a description of data graphs that satisfy these conditions.
Such descriptions may be used for a variety of purposes besides validation,
including user interface building, code generation, and data integration.
Semantic shapes are frequently described using the SHACL or ShEx language.

## Contents

- [SHACL Validators](#shacl-validators)
- [ShEx Validators](#shex-validators)
- [Shapes Discovery Tools](#shapes-discovery-tools)
- [Shapes Collections](#shapes-collections)
- [Shape Conversion Tools](#shape-conversion-tools)
- [Shape Generators](#shape-generators)
- [Shape-based Query Generators](#shape-based-query-generators)
- [Shape Editors, Visualizations](#shape-editors-visualizations)
- [Declarative UIs](#declarative-uis)
- [IDE support](#ide-support)
- [Books](#books)
- [Tutorials](#tutorials)
- [Talks](#talks)
- [Presentations](#presentations)
- [Specifications](#specifications)
- [Legend](#legend)

## SHACL Validators

- [Apache Jena SHACL](https://jena.apache.org/documentation/shacl/index.html) <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/apache/jena" align="middle"> - Supports SHACL Core, SHACL-SPARQL; `Apache-2.0` `Java`.
- [RDF4J SHACL Engine](https://rdf4j.org/documentation/programming/shacl) <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/eclipse-rdf4j/rdf4j" align="middle"> - Supports SHACL Core (without some property paths), SHACL-SPARQL, incremental validation; `BSD-3-Clause` `Java`.
- [rdf-validate-shacl](https://github.com/zazuko/rdf-validate-shacl) <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/zazuko/rdf-validate-shacl" align="middle"> - Supports SHACL Core; pure JavaScript validator on top of the [RDFJS](https://rdf.js.org/) stack; [playground](https://zazuko.github.io/shacl-playground); `MIT` `JavaScript`.
- [SHACL for Ruby](https://github.com/ruby-rdf/shacl/) ![GitHub last commit](https://img.shields.io/github/last-commit/ruby-rdf/shacl) - A pure-Ruby library for working with the Shape Constraint Language to validate the shape of RDF graphs; `BSD-3-Clause` `Ruby`.
- [shacl-engine](https://github.com/rdf-ext/shacl-engine) <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/rdf-ext/shacl-engine" align="middle"> - Supports SHACL Core, SHACL-SPARQL; A fast engine for data provided as [RDF/JS](http://rdf.js.org/data-model-spec/) objects; [playground](https://playground.rdf-ext.org/shacl/); `MIT` `JavaScript`.
- [TopBraid SHACL API](https://github.com/TopQuadrant/shacl) <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/TopQuadrant/shacl" align="middle"> - Supports SHACL Core, SHACL-SPARQL, SHACL rules; based on Jena; `BSD-3-Clause` `Java`.
- [TopBraid SHACL API Extended](https://github.com/SHACL-X/shacl-x) <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/SHACL-X/shacl-x" align="middle"> - Fork of TopBraid SHACL API + added SHACL-JS based on GraalVM Polyglot; `BSD-3-Clause` `Java`.

## ShEx Validators

- [Apache Jena ShEx](https://jena.apache.org/documentation/shex/index.html) <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/apache/jena" align="middle"> - Supports ShEx, ShExC; not supported semantic actions, EXTERNAL; `Apache-2.0` `Java`.
- [shexSpec/shex.js](https://github.com/shexjs/shex.js) <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/shexjs/shex.js" align="middle"> - JavaScript implementation of Shape Expressions; [playground](http://rawgit.com/shexSpec/shex.js/master/doc/shex-simple.html); `MIT` `JavaScript`.
- [ShEx-validator](https://github.com/HW-SWeL/ShEx-validator) <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/HW-SWeL/ShEx-validator" align="middle"> :skull: - A standalone Node module with a command line interface; `MIT` `JavaScript`.
- [Validata](https://github.com/HW-SWeL/Validata) <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/HW-SWeL/Validata" align="middle"> - An intuitive, standalone web-based tool to help building RDF documents by validating against preset schemas written in the ShEx language; [playground](http://hw-swel.github.io/Validata/); [playground](https://www.w3.org/2015/03/ShExValidata/); `MIT` `JavaScript`.

## Shapes Discovery Tools

- [RDFminer](https://github.com/Wimmics/RDFminer) - Web application to automatically discover SHACL shapes representative of an RDF data graph, by Wimmics; `CECILL-C` `Java`.
- [SHACL Discovery Service](https://github.com/AKSW/discover-shacl-shapes) - Example implementation of a discovery service for SHACL shapes/shape groups; `MIT` `PHP`.
- [Shapes of You index](https://index.semanticscience.org/) - SPARQL queries, OWL/SKOS vocabularies, SHACL/ShEx shapes, indexed from public `git` repositories; `MIT` `Typescript, Python`.

## Shapes Collections

- [schema.org Shapes](http://datashapes.org/schema) - Schema.org, converted to SHACL by TopQuadrant.

## Shape Conversion Tools

- [ShacShifter](https://github.com/AKSW/ShacShifter) <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/AKSW/ShacShifter" align="middle"> :skull: - Shape shifter from SHACL to other formats (currently RDForms); `GPL-3.0` `Python`.
- [SHACL To JSON Schema](https://github.com/comake/shacl-to-json-schema) <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/comake/shacl-to-json-schema" align="middle"> - TS, SHACL-to-JSON-Schema translator; `Typescript`.

## Shape Generators

- [owl2shacl](https://github.com/sparna-git/owl2shacl) - OWL-to-SHACL conversion rules.

## Shape-based Query Generators

- [@hydrofoil/shape-to-query](https://shape-to-query.hypermedia.app/docs) - Generate SPARQL queries from SHACL Shapes; [playground](https://shape-to-query.hypermedia.app); `Typescript` `MIT`.

## Shape Editors, Visualizations

- [Allotrope Shape Editor](https://gitlab.com/allotrope-open-source/allotrope-devops/-/wikis/shacl-shape-editor) - The Shape Editor supports editing of shacl and shaclc files; `Apache-2.0` `Java`.

## Declarative UIs

Data viewers/Editors based on shapes.

- [shaperone](https://forms.hypermedia.app) <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/hypermedia-app/shaperone" align="middle"> - SHACL Shapes Form generator; [playground](https://forms.hypermedia.app/playground); `MIT` `Typescript`.

## IDE support

- [Linked Data Extension](https://marketplace.visualstudio.com/items?itemName=Elsevier.linked-data) - VS Code Extension for editing RDF files with embedded SHACL validator and SPARQL engine.
- [SHACL Language Server](https://marketplace.visualstudio.com/items?itemName=stardog-union.vscode-langserver-shacl) - A VS Code extension providing language intelligence (diagnostics, hover tooltips, auto-completion, etc.) for W3C standard SHACL via the Language Server Protocol.
- [Mentor RDF for VS Code](https://marketplace.visualstudio.com/items?itemName=faubulous.mentor) - Code editing support for RDF, RDFS, OWL, SKOS, SHACL and SPARQL.

## Books

- [Validating RDF Data (2018)](https://book.validatingrdf.com)

## Tutorials

- [Shapes applications and tools - ISWC'20 Tutorial](https://www.validatingrdf.com/tutorial/iswc2020/)

## Talks

- [The Many Shapes of SHACL by Holger Knublauch](https://www.youtube.com/watch?v=ccs-KhnWR1U) - LOTICO Talk, 18 Jun 2020.
- [One Ontology, One Data Set, Multiple Shapes with SHACL by Tara Raafat](https://www.youtube.com/watch?v=apG5K3zc4V0) - Connected Data London, 2019.
- [An Overview of SHACL Shapes Constraint Language](https://www.youtube.com/watch?v=_i3zTeMyRzU) - TopQuadrant, 2017.

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
:skull: — Each one denotes 5 years since last update (e.g., :skull: :skull: :skull: denotes 15 years).

:moneybag: — Denotes closed source commercial software.
