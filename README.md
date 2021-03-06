# mkdocs-template

A template repository for a [MkDocs](https://mkdocs.org) site with best practices baked in.

## Theme

This site uses [Material for MkDocs](squidfunk.github.io/mkdocs-material) theme.

## Getting Started

1. Ensure that Python and PIP are installed on your system:

- [Python Download](https://www.python.org/downloads/)

2. Install MkDocs: https://www.mkdocs.org/user-guide/installation/

```bash
pip install mkdocs
```

3. Install Material for MkDocs: https://github.com/squidfunk/mkdocs-material#quick-start

```bash
pip install mkdocs-material
```

4. Preview the docs locally. From the location which contains mkdocs.yml:

```bash
mkdocs serve
```

## Documentation Sections

Documentation structure follows the [Divio System for Documentation](https://documentation.divio.com).

| Section        | Description                                                            |
| -------------- | ---------------------------------------------------------------------- |
| **Tutorials**  | Guides for getting a user started with the project                     |
| **How-To's**   | Guides for showing a user certain features or functions of the project |
| **References** | List of technologies with descriptors related to project               |
| **Concepts**   | Indepth discussions on topics related to the project                   |

Within the `docs` directory you'll find subdirectories for each of these types of documentation.
