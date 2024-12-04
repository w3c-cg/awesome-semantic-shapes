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
- [Talks and Presentations](#talks-and-presentations)
- [Specifications](#specifications)
- [Legend](#legend)

## SHACL Validators

Software tools or libraries, sorted by programming language.

- [Apache Jena SHACL](https://github.com/apache/jena/tree/main/jena-shacl) <img alt="Maven Central Version" src="https://img.shields.io/maven-central/v/org.apache.jena/jena-shacl" align="top"> <img alt="Maven Central Last Update" src="https://img.shields.io/maven-central/last-update/org.apache.jena/jena-shacl" align="top"> - Supports SHACL Core, SHACL-SPARQL; [docs](https://jena.apache.org/documentation/shacl/index.html); `Apache-2.0` license; `Java`.
- [RDF4J SHACL Engine](https://github.com/eclipse-rdf4j/rdf4j/tree/main/core/sail/shacl) <img alt="Maven Central Version" src="https://img.shields.io/maven-central/v/org.eclipse.rdf4j/rdf4j-shacl" align="top"> <img alt="Maven Central Last Update" src="https://img.shields.io/maven-central/last-update/org.eclipse.rdf4j/rdf4j-shacl" align="top"> - Supports SHACL Core (without some property paths, see [5.0.3 improvements](https://github.com/Sveino/Inst4CIM-KG/issues/95#issuecomment-2437819932)), SHACL-SPARQL, incremental validation; [docs](https://rdf4j.org/documentation/programming/shacl/); `BSD-3-Clause` license; `Java`.
- [TopBraid SHACL API](https://github.com/TopQuadrant/shacl) <img alt="Maven Central Version" src="https://img.shields.io/maven-central/v/org.topbraid/shacl" align="top"> <img alt="Maven Central Last Update" src="https://img.shields.io/maven-central/last-update/org.topbraid/shacl" align="top"> 💰 - Supports SHACL Core, SHACL-SPARQL, SHACL rules; based on Jena; `BSD-3-Clause` license; `Java`.
  - [RDF validator](https://www.itb.ec.europa.eu/shacl/any/upload) - The EU Interoperability Test Bed (ITB) playground based on TQ API; validate any RDF with SHACL Shapes.
  - [SHACL shapes validator](https://www.itb.ec.europa.eu/shacl/shacl/upload) - The EU Interoperability Test Bed (ITB) playgrounds based on TQ API; validate SHACL Shapes itself.
  - [Sparna SHACL validator](https://shacl-play.sparna.fr/play/validate) - Free online suite of tools from Sparna to work with SHACL; based on TQ API.
- [TopBraid SHACL API Extended](https://github.com/SHACL-X/shacl-x) <img alt="GitHub Release" src="https://img.shields.io/github/v/release/SHACL-X/shacl-x" align="top"> <img alt="GitHub Release Date" src="https://img.shields.io/github/release-date/SHACL-X/shacl-x" align="top"> - Fork of TopBraid SHACL API + added SHACL-JS based on GraalVM Polyglot; [docs](https://shacl-x.github.io/docs/); `BSD-3-Clause` license; `Java`.
- [shacl-js](https://github.com/TopQuadrant/shacl-js) <img alt="GitHub Release Date" src="https://img.shields.io/github/last-commit/TopQuadrant/shacl-js" align="top"> - SHACL API; `Apache` license; `JavaScript`. Recommends migration to `rdf-validate-shacl`. ☠️.
  - [playground](https://shacl.org/playground/) - Browser-based testbed.
- [rdf-validate-shacl](https://github.com/zazuko/rdf-validate-shacl) <img alt="NPM Version" src="https://img.shields.io/npm/v/rdf-validate-shacl" align="top"> <img alt="GitHub Release Date" src="https://img.shields.io/github/release-date/zazuko/rdf-validate-shacl" align="top"> - Supports SHACL Core; pure JavaScript validator on top of the [RDFJS](https://rdf.js.org/) stack; `MIT` license; `JavaScript`.
  - [playground](https://zazuko.github.io/shacl-playground) - Browser-based testbed.
- [shacl-engine](https://github.com/rdf-ext/shacl-engine) <img alt="NPM Version" src="https://img.shields.io/npm/v/shacl-engine" align="top"> <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/rdf-ext/shacl-engine" align="top"> - Supports SHACL Core, SHACL-SPARQL; A fast engine for data provided as [RDF/JS](http://rdf.js.org/data-model-spec/) objects; `MIT` license; `JavaScript`.
  - [playground](https://playground.rdf-ext.org/shacl/) - Browser-based testbed.
  - [rdf-ext-cli](https://github.com/rdf-ext/rdf-ext-cli) - Command line tool for validation. Data and shapes can be given as file, URL, or SPARQL endpoint + query.
- [SHACL for Ruby](https://github.com/ruby-rdf/shacl) <img alt="Gem Version" src="https://img.shields.io/gem/v/shacl" align="top"> <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/ruby-rdf/shacl" align="top"> - A pure-Ruby library for working with the Shape Constraint Language to validate the shape of RDF graphs; `BSD-3-Clause` license; `Ruby`.
- [maplib](https://github.com/DataTreehouse/maplib) <img src="https://img.shields.io/github/v/tag/DataTreehouse/maplib" align="top"> <img src="https://img.shields.io/github/last-commit/DataTreehouse/maplib" align="top"> - High-performance RDF knowledge graph construction, SHACL validation and SPARQL-based enrichment. `Apache-2.0` license. `Rust, Python`. But SHACL is not open source yet: [lib/shacl/src/lib.rs](https://github.com/DataTreehouse/maplib/blob/main/lib/shacl/src/lib.rs) says `unimplemented!("Contact Data Treehouse to try")`
- [rudof](https://rudof-project.github.io/rudof/) [![Latest Version](https://img.shields.io/crates/v/rudof-cli.svg)](https://crates.io/crates/rudof-cli) [![PyPI](https://img.shields.io/pypi/v/pyrudof)](https://pypi.org/project/pyrudof/) <img alt="GitHub Release Date" src="https://img.shields.io/github/release-date/rudof-project/rudof" align="top"> is a library that implements ShEx, SHACL, [DCTAP](https://www.dublincore.org/specifications/dctap/), and other technologies in the RDF ecosystem. The library is implemented in [Rust](https://www.rust-lang.org/) and also provides Python bindings.

## ShEx Validators

Software tools or libraries, sorted by programming language.

- [Apache Jena ShEx](https://github.com/apache/jena/tree/main/jena-shex) <img alt="Maven Central Version" src="https://img.shields.io/maven-central/v/org.apache.jena/jena-shex" align="top"> <img alt="Maven Central Last Update" src="https://img.shields.io/maven-central/last-update/org.apache.jena/jena-shex" align="top"> - Supports ShEx, ShExC; not supported semantic actions, EXTERNAL; [docs](https://jena.apache.org/documentation/shex/); `Apache-2.0` license; `Java`.
- [shexSpec/shex.js](https://github.com/shexjs/shex.js) <img alt="NPM Version" src="https://img.shields.io/npm/v/shex" align="top"> <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/shexjs/shex.js" align="top"> - JavaScript implementation of Shape Expressions; `MIT` license; `JavaScript`.
  - [playground](http://rawgit.com/shexSpec/shex.js/master/doc/shex-simple.html) - Browser-based testbed.
- [ShEx-validator](https://github.com/HW-SWeL/ShEx-validator) <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/HW-SWeL/ShEx-validator" align="top"> ☠️ - Standalone Node module with a command line interface; `MIT` license; `JavaScript`. Built on top of [ShExDemo](https://github.com/ericprud/ShExDemo)
  - [Validata](https://github.com/HW-SWeL/Validata) <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/HW-SWeL/Validata" align="top"> ☠️ - Web-based UI to validate RDF against ShEx schemas; `MIT` license; `JavaScript`.
  - [playground1](http://hw-swel.github.io/Validata/) (HW-SWeL)
  - [playground2](https://www.w3.org/2015/03/ShExValidata/) (W3C)
- [rudof](https://rudof-project.github.io/rudof/) [![Latest Version](https://img.shields.io/crates/v/rudof-cli.svg)](https://crates.io/crates/rudof-cli) [![PyPI](https://img.shields.io/pypi/v/pyrudof)](https://pypi.org/project/pyrudof/) <img alt="GitHub Release Date" src="https://img.shields.io/github/release-date/rudof-project/rudof" align="top"> is a library that implements ShEx, SHACL, [DCTAP](https://www.dublincore.org/specifications/dctap/), and other technologies in the RDF ecosystem. The library is implemented in [Rust](https://www.rust-lang.org/) and also provides Python bindings.

## Shapes Discovery Tools

- [RDFminer](https://github.com/Wimmics/RDFminer) - Web application to automatically discover SHACL shapes representative of an RDF data graph, by Wimmics; `CECILL-C` license; `Java`.
- [SHACL Discovery Service](https://github.com/AKSW/discover-shacl-shapes) - Example implementation of a discovery service for SHACL shapes/shape groups; `MIT` license; `PHP`.
- [Shapes of You index](https://index.semanticscience.org/) - SPARQL queries, OWL/SKOS vocabularies, SHACL/ShEx shapes, indexed from public `git` repositories; `MIT` license; `Typescript`, `Python`.
- [SHACL Play! Catalog](https://shacl-play.sparna.fr/play/shapes-catalog) - To see your shapes file listed here, add it to the [Shapes Catalog source file on Github](https://github.com/sparna-git/SHACL-Catalog/blob/master/shacl-catalog.ttl).

## Shapes Collections

- [schema.org Shapes](http://datashapes.org/schema) - Schema.org, converted to SHACL by TopQuadrant.
- [Europarl Shapes](https://data.europarl.europa.eu/en/developer-corner) - Application profiles for European Parliament & all related dataset-specific profiles.

## Shape Conversion Tools

- [ShacShifter](https://github.com/AKSW/ShacShifter) <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/AKSW/ShacShifter" align="top"> ☠️ - Shape shifter from SHACL to other formats (currently RDForms); `GPL-3.0` license; `Python`.
- [SHACL To JSON Schema](https://github.com/comake/shacl-to-json-schema) <img alt="NPM Version" src="https://img.shields.io/npm/v/@comake/shacl-to-json-schema" align="top"> <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/comake/shacl-to-json-schema" align="top"> - SHACL-to-JSON-Schema translator; `Typescript`.
- [rudof](https://rudof-project.github.io/rudof/cli_usage/convert.html) [![Latest Version](https://img.shields.io/crates/v/rudof-cli.svg)](https://crates.io/crates/rudof-cli) [![PyPI](https://img.shields.io/pypi/v/pyrudof)](https://pypi.org/project/pyrudof/) <img alt="GitHub Release Date" src="https://img.shields.io/github/release-date/rudof-project/rudof" align="top"> supports conversion between different RDF Data modeling technologies using the `convert` command.
- [SHACL Play! JSON-LD context](https://shacl-play.sparna.fr/play/context) <img alt="Version" src="https://img.shields.io/github/v/release/sparna-git/shacl-play" align="top"> <img alt="GitHub Release Date" src="https://img.shields.io/github/release-date/sparna-git/shacl-play" align="top"> - SHACL-to-JSON-LD context generator; `Java`.

## Shape Generators

 - [SHACL Play! Converter](https://shacl-play.sparna.fr/play/convert) - Converts between RDF schema formats. Has OWL-to-SHACL (open, semi-closed, closed). 
- [owl2shacl](https://github.com/sparna-git/owl2shacl) - OWL-to-SHACL conversion rules.
- [TopQuadrant: OWL Axioms to SHACL Constraints](https://www.topquadrant.com/doc/latest/reference/Transform_ConvertOWLAxiomsToSHACLConstraints.html) 💰 - Commercial closed-source solution by TopQuadrant
- [elevont/owl2shacl](https://github.com/elevont/owl2shacl) - A CLI tool that tries to convert simple OWL ontologies into SHACL shapes; `AGPL-3.0` license; `rust`.

## Shape-based Query Generators

- [shape-to-query](https://github.com/hypermedia-app/shape-to-query) <img alt="NPM Version" src="https://img.shields.io/npm/v/@hydrofoil/shape-to-query" align="top"> <img alt="GitHub Release Date" src="https://img.shields.io/github/release-date/hypermedia-app/shape-to-query" align="top"> - Generate SPARQL queries from SHACL Shapes; [docs](https://shape-to-query.hypermedia.app/docs); `MIT` license; `Typescript`.
  - [playground](https://shape-to-query.hypermedia.app)
- [SHACL Play! SPARQL](https://shacl-play.sparna.fr/play/sparql) - Generates SPARQL queries to extract RDF subset based on SHACL specification of the target dataset.

## Shape Editors, Visualizations

- [Allotrope Shape Editor](https://gitlab.com/allotrope-open-source/allotrope-devops/-/wikis/shacl-shape-editor) - The Shape Editor supports editing of shacl and shaclc files; `Apache-2.0` license; `Java`.
- [SHACL Play! Tools](https://shacl-play.sparna.fr/) - Edit & visualize SHACL; `LGPL-3.0 license` license; `Java`.
  - [SHACL in Excel](https://shacl-play.sparna.fr/play/shaclexcel) - A SHACL editor from Excel.
  - [SHACL documentation](https://shacl-play.sparna.fr/play/doc) - A documentation generator to print an application profile specified in SHACL.
  - [UML diagrams](https://shacl-play.sparna.fr/play/draw) - A diagram generator to display an application profile specified in SHACL.

## Declarative UIs

Data viewers/Editors based on shapes.

- [shaperone](https://github.com/hypermedia-app/shaperone) <img alt="NPM Version" src="https://img.shields.io/npm/v/@hydrofoil/shaperone-wc" align="top"> <img alt="GitHub Release Date" src="https://img.shields.io/github/release-date/hypermedia-app/shaperone" align="top"> - SHACL Shapes Form generator; [docs](https://forms.hypermedia.app); `MIT` license; `Typescript`.
  - [playground](https://forms.hypermedia.app/playground)
- [Sparnatural](https://github.com/sparna-git/Sparnatural) <img alt="Version" src="https://img.shields.io/github/v/release/sparna-git/Sparnatural" align="top"> <img alt="GitHub Release Date" src="https://img.shields.io/github/release-date/sparna-git/Sparnatural" align="top"> - Visual knowledge graph explorer with SPARQL, in the browser, configurable with SHACL; [docs](https://docs.sparnatural.eu/index.html#31-shacl-configuration); `LGPL-3.0 license` license; `Typescript`.

## IDE support

- [Linked Data Extension](https://marketplace.visualstudio.com/items?itemName=Elsevier.linked-data) - VS Code Extension for editing RDF files with embedded SHACL validator and SPARQL engine.
- [SHACL Language Server](https://marketplace.visualstudio.com/items?itemName=stardog-union.vscode-langserver-shacl) - A VS Code extension providing language intelligence (diagnostics, hover tooltips, auto-completion, etc.) for W3C standard SHACL via the Language Server Protocol.
- [Mentor RDF for VS Code](https://marketplace.visualstudio.com/items?itemName=faubulous.mentor) - Code editing support for RDF, RDFS, OWL, SKOS, SHACL and SPARQL.
- [SHACLC Language Server](https://marketplace.visualstudio.com/items?itemName=jeswr.shaclc-language-server) ([source](https://github.com/jeswr/shaclc-language-server)) - A VS Code extension providing language intelligence (diagnostics, hover tooltips, auto-completion, etc.) for CG standard SHACL Compact Syntax via the Language Server Protocol. MIT License.

## Books

- [Validating RDF Data (2018)](https://book.validatingrdf.com) - The SHACL and ShEx book.

## Tutorials

- [Shapes applications and tools: ISWC'20 Tutorial](https://www.validatingrdf.com/tutorial/iswc2020/) - Main tutorial.

## Talks and Presentations

- [The Many Shapes of SHACL by Holger Knublauch](https://www.youtube.com/watch?v=ccs-KhnWR1U) - LOTICO Talk, 18 Jun 2020.
- [One Ontology, One Data Set, Multiple Shapes with SHACL by Tara Raafat](https://www.youtube.com/watch?v=apG5K3zc4V0) - Connected Data London, 2019.
- [An Overview of SHACL Shapes Constraint Language: Part 2](https://www.youtube.com/watch?v=TSDplfqw8rM) - TopQuadrant, 2017.
- [An Overview of SHACL Shapes Constraint Language](https://www.youtube.com/watch?v=_i3zTeMyRzU) - TopQuadrant, 2017.

## Specifications

- SHACL W3C Recommendations & Notes
  - [Shapes Constraint Language (SHACL)](https://www.w3.org/TR/shacl/) - W3C Recommendation, 20 July 2017.
  - [SHACL Advanced Features](https://www.w3.org/TR/shacl-af/) - W3C Working Group Note, 08 June 2017.
  - [SHACL JavaScript Extensions](https://www.w3.org/TR/shacl-js/) - W3C Working Group Note, 08 June 2017.
  - [SHACL Test Suite and Implementation Report](https://w3c.github.io/data-shapes/data-shapes-test-suite/) - W3C Document 01 July 2019.
  - [SHACL Use Cases and Requirements](https://www.w3.org/TR/shacl-ucr/) - W3C Working Group Note 20 July 2017.

- SHACL Community Group Latest Drafts & Notes
  - [SHACL 1.2 Core](https://w3c.github.io/shacl/shacl-core/)
  - [SHACL 1.2 SPARQL Extensions](https://w3c.github.io/shacl/shacl-sparql/)
  - [SHACL Advanced Features 1.1](https://w3c.github.io/shacl/shacl-af/)
  - [SHACL Compact Syntax](https://w3c.github.io/shacl/shacl-compact-syntax/)
  - [SHACL JavaScript Extensions](https://w3c.github.io/shacl/shacl-js/)

- SHACL-related specifications
  - [The Shape Topologies algorithm](https://treecg.github.io/specification/shape-topologies)
  - [DASH Data Shapes](https://www.datashapes.org/) - Platform-independent extensions of SHACL for common tasks. Stuff that could become an official standard in the future.

- ShEx
  - [Shape Expressions Language 2.1](https://shex.io/shex-semantics/index.html) - Final Community Group Report, 8 October 2019.
  - [ShEx Primer](https://shexspec.github.io/primer/index.html) - Draft Community Group Report, 7 December 2022.
  - [ShEx Text Suite](https://github.com/shexSpec/shexTest) and [website](https://shexspec.github.io/shexTest/) - Version `next@1.0.2`, last release 5 October 2018.
  - [Recommended Practice for Standard for Shape Expression Schemas](https://shexspec.github.io/spec/) - IEEE Computer Society P3330/D3, Draft 9 October 2024. Next-version spec with `EXTENDS` keyword.
  - [ShEx Primer](https://shex.io/primer-next/) - Primer with `EXTENDS` keyword, Draft Community Group Report 25 May 2022.

## Legend
- ☠️ : Each one denotes 5 years since last update (e.g., ☠️☠️☠️ denotes 15 years).
- 💰 : Denotes closed source commercial software.