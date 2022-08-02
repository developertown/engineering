# Formatting

DeveloperTown projects **should** utilize code formatters to ensure consistent styling across a growing code base. There are a number of tools that can be used to achieve consistent code formatting and styling. At DeveloperTown projects should leverage [editorconfig](https://editorconfig.org/) and [prettier](https://prettier.io/) where appropriate.

## Why Format Code

## Language and Tools

* c#
* Kotlin
* Typescript / Javascript
* Terraform

### c#

### Kotlin

### Typescript / Javascript

[Prettier](https://prettier.io/) is an opinionated code formatter.  Prettier enforces a consistent code style (i.e. code formatting that won’t affect the AST) across your entire codebase because it disregards the original styling* by parsing it away and re-printing the parsed AST with its own rules that take the maximum line length into account, wrapping code when necessary.

### Terraform

```
terrform fmt
```

The `terraform fmt` command is used to rewrite Terraform configuration files to a canonical format and style. This command applies a subset of the Terraform language style conventions, along with other minor adjustments for readability.