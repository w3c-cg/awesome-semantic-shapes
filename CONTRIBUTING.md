# Contribution Guidelines

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md).
By participating in this project you agree to abide by its terms.

This repository is governed by the [CC0 license](https://creativecommons.org/publicdomain/zero/1.0/).

To add, remove, or change things on the list: **Submit a pull request**.

## Quality standards

Please contribute links to packages/projects you have used or are familiar with. This will help ensure high-quality entries.

To be on the list, project repositories should adhere to the following quality standards.

- have at least 5 months of history since the first commit
- function as documented and expected
- be generally useful to the wider Semantic Web community
- be actively maintained or not maintained anymore but finished and extremely useful (should be marked with ☠️)
- be stable or progressing toward stable
- have at least one official version-numbered release
- be open source or commercial (marked with 💰) software

Categories must have at least 3 items.

## How to add an item to the list

Open a pull request against the README.md document that adds the repository to the list.

- One pull request can add more than one item to the list
- Each item should be added respecting sorting within its category
  - firstly, by programming language (if applicable)
  - secondly, in alphabetical order

## Item format

Non-software item must conform to the following format:
```
<link> - <Description>.
```

Software item must conform to the following format:
```
<link> <activity info> - <Description>.
```

In each case:
- The link:
  - Should be the name of the package or project.
  - Should point to a specific module related to the category (e.g., in the 'SHACL Validators' section, link to `https://github.com/apache/jena/tree/main/jena-shacl`, not `https://github.com/apache/jena`).
- Activity info
  - Should consist of two badges:
    - The latest known stable version badge (from any most common binary repository or GH Releases).
    - The recent repository activity badge (only one of these options): 
      - "latest release date" (recommended) from any repository binary or GitHub Releases.
      - if there is no published version, then "last commit date".
  - Should not contain URL links.
  - Use HTML `<img/>` badge format, not Markdown image (e.g., use `<img alt="Latest Version" src="https://img.shields.io/crates/v/rudof-cli" align="top">`, not `![Latest Version](https://img.shields.io/crates/v/rudof-cli.svg)`).
  - Use `<img align="top">` badge format for better inline alignment.
  - Do not use any other badges (build status, dependencies, etc.).
  - Additional emoji can be used to mark commercial 💰 or abandoned ☠️ software.
- Descriptions
  - Should be clear, concise, and non-promotional.
  - Should begin with a capital letter.
  - May consist of several sentences.
  - Should be separated from the activity info a hyphen preceded and followed by spaces, ` - `.
  - Should contain license info and programming language at the end, formatted as ``` `text in code quotes` ```.
  - Should follow the link on the same line and end with a punctuation mark. Remember to put a period `.` at the end of the project description.

### Examples

#### Non-software items

Without a description:

```markdown
- [SHACL 1.2 Core](https://w3c.github.io/shacl/shacl-core/)
```

With a description:
```markdown
- [Validating RDF Data (2018)](https://book.validatingrdf.com) - The SHACL and ShEx book.
```

#### Software module item with a description

```markdown
- [Apache Jena SHACL](https://github.com/apache/jena/tree/main/jena-shacl) <img alt="Maven Central Version" src="https://img.shields.io/maven-central/v/org.apache.jena/jena-shacl" align="top"> <img alt="Maven Central Last Update" src="https://img.shields.io/maven-central/last-update/org.apache.jena/jena-shacl" align="top"> - Supports SHACL Core, SHACL-SPARQL; [docs](https://jena.apache.org/documentation/shacl/index.html); `Apache-2.0` license; `Java`.
```

### Ignoring some linter's errors

Our list [awesome lint](https://github.com/sindresorhus/awesome-lint)

In general it is better to comply with linter's rules. But in some cases it is acceptable to bypass it:
- If you are adding reasonably the same URL link to several list's categories, you'll end up with duplication errors.
- If you reasonably need more freedom in a description formatting, this will lead to formatting errors.

In this cases it is possible to enable and/or disable some linter rules for the specific list item (line) with ```lint ignore``` (the recommended approach) or enable and/or disable the rules globally (not recommended) with ```lint disable``` and/or ```lint enable```.

Just put the rule IDs after `lint ignore` and separate them with spaces.

- double-link -- checks list item duplication
- awesome-list-item -- checks list item formatting

#### Examples

```
<!--lint ignore double-link-->
<!--lint ignore awesome-list-item-->
<!--lint ignore awesome-list-item double-link-->
```

## How to add a new category

If you are creating a new category, move any relevant projects to that new category, while ensuring
that every category in the resulting list has at least 3 projects, and that the categories are alphabetized.

## Updating your PR

It is often difficult to make a PR adhere to the standards above.
If the maintainers notice anything that we'd like changed, we'll ask you to
edit your PR before we merge it. There's no need to open a new PR; just edit
the existing one.

## Congratulations, your project got accepted — what now?

You are an outstanding project now! We encourage you to tell others about it 
by adding one of these badges to your project webpage(s):
- [![Mentioned in Awesome Semantic Shapes](https://awesome.re/mentioned-badge.svg)](https://github.com/w3c-cg/awesome-semantic-shapes)  
  - ```md
    [![Mentioned in Awesome Semantic Shapes](https://awesome.re/mentioned-badge.svg)](https://github.com/w3c-cg/awesome-semantic-shapes)  
    ```
  - ```html
    <a href="https://github.com/w3c-cg/awesome-semantic-shapes">
      <img src="https://awesome.re/mentioned-badge.svg" alt="Mentioned in Awesome Semantic Shapes" style="max-width: 100%;">
    </a>
    ```

- [![Mentioned in Awesome Semantic Shapes](https://awesome.re/mentioned-badge-flat.svg)](https://github.com/w3c-cg/awesome-semantic-shapes)
  - ```md
    [![Mentioned in Awesome Semantic Shapes](https://awesome.re/mentioned-badge-flat.svg)](https://github.com/w3c-cg/awesome-semantic-shapes)
    ```
  - ```html
    <a href="https://github.com/w3c-cg/awesome-semantic-shapes">
      <img src="https://awesome.re/mentioned-badge-flat.svg" alt="Mentioned in Awesome Semantic Shapes" style="max-width: 100%;">
    </a>
    ```
