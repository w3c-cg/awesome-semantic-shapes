# Contribution Guidelines

Please note that this project is released with a [Contributor Code of Conduct](code-of-conduct.md).
By participating in this project you agree to abide by its terms.

This repository is governed by the [CC0 license](https://creativecommons.org/publicdomain/zero/1.0/).

To add, remove, or change things on the list: **Submit a pull request**.

## Quality standards

Please contribute links to packages/projects you have used or are familiar with. This will help ensure high-quality entries.

To be on the list, project repositories should adhere to the following quality standards.

- have at least 5 months of history since the first commit.
- function as documented and expected;
- be generally useful to the wider Semantic Web community;
- be actively maintained or not maintained anymore but finished and extremely useful (should be marked with ☠️);
- be stable or progressing toward stable;
- have at least one official version-numbered release;
- be open source or commercial (marked with 💰) software.

Categories must have at least 3 items.

## How to add an item to the list

Open a pull request against the README.md document that adds the repository to the list.

- The pull request could add more than one item to the list.
- The added items should respect sorting within its category:
  - by programming language first (if it is applicable),
  - and then in alphabetical order.

## Item format

Non-software item must conform to the following format:

`<link> - <Description>.`

Software item must conform to the following format:

`<link> <activity info> - <Description>.`

Where:
- The link:
  - Should be the name of the package or project.
  - The hyperlink should point to a specific module related to the category (e.g. in case of 'SHACL Validators' section, use `https://github.com/apache/jena/tree/main/jena-shacl`, not `https://github.com/apache/jena`).
- Activity info:
  - Should consists of two badges:
    - Latest known stable version badge (from any most common binary repository or GH Releases).
    - Recent repository activity badge.
  - Use `<img align="top">` badge format to better inline alignment.
  - Do not use any other badges (build status, dependencies, etc.).
  - Additional icons could be used to mark commercial 💰 or abandoned ☠️ software.
- Description:
  - Should be clear, concise, and non-promotional.
  - Should begin with a capital letter.
  - May consist of several sentences.
  - Should be separated from the activity info with spaces and a dash ` - `.
  - Should contain license info and programming language at the end, formatted as `text in code quotes`.
  - Should follow the link on the same line and end with a punctuation mark. Remember to put a period `.` at the end of the project description.

### Examples

#### Non-software items

A simple item without a description:

```markdown
- [SHACL To JSON Schema](https://github.com/comake/shacl-to-json-schema)
```

Software example :
```markdown
- [Validating RDF Data (2018)](https://book.validatingrdf.com) - The SHACL and ShEx book.
```

#### Software module item with a description

```markdown
- [Apache Jena SHACL](https://github.com/apache/jena/tree/main/jena-shacl) <img alt="Maven Central Version" src="https://img.shields.io/maven-central/v/org.apache.jena/jena-shacl" align="top"> <img alt="Maven Central Last Update" src="https://img.shields.io/maven-central/last-update/org.apache.jena/jena-shacl" align="top"> - Supports SHACL Core, SHACL-SPARQL; [docs](https://jena.apache.org/documentation/shacl/index.html); `Apache-2.0` license; `Java`.
```

## How to add a new category

If you are creating a new category, move the projects that apply to the new category, ensuring
that the resulting list has at least 3 projects in every category, and that the categories are alphabetized.

## Updating your PR

A lot of times, making a PR adhere to the standards above can be difficult.
If the maintainers notice anything that we'd like changed, we'll ask you to
edit your PR before we merge it. There's no need to open a new PR, just edit
the existing one.

## Congrats, your project got accepted - what now?

You are an outstanding project now! Feel encouraged to tell others about it by adding one of these badges:  
[![Mentioned in Awesome Semantic Shapes](https://awesome.re/mentioned-badge.svg)](https://github.com/w3c-cg/awesome-semantic-shapes)  
[![Mentioned in Awesome Semantic Shapes](https://awesome.re/mentioned-badge-flat.svg)](https://github.com/w3c-cg/awesome-semantic-shapes)

```md
[![Mentioned in Awesome Semantic Shapes](https://awesome.re/mentioned-badge.svg)](https://github.com/w3c-cg/awesome-semantic-shapes)  
[![Mentioned in Awesome Semantic Shapes](https://awesome.re/mentioned-badge-flat.svg)](https://github.com/w3c-cg/awesome-semantic-shapes)
```
