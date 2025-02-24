# Welcome!

## Don't know where to start?

- report a *bug* or suggest an *improvement* -- open an [issue] on *GitHub*
- write a *tutorial* -- have a new example for using END? create a new `.qmd` file and add it to the overall website structure in `_quarto.yml`
- improve the *documentation* -- all functions have a `docstring` where they are declared, and improving them is a great way to get started

[issue]: https://github.com/EcoJulia/SpatialBoundaries.jl/issues

## Setting up your environment

Have a look at the current [Julia documentation][pkgdoc].

[pkgdoc]: https://docs.julialang.org/en/stable/manual/packages/#Making-changes-to-an-existing-package-1

## EMOJIS!

Please use emojis, this helps visually sorting through the commits (and makes for a 
fun time). Inspiration taken from [sciencegitmojis](https://github.com/MichielStock/sciencegitmojis)

| If the commit is about...                               | ...then use                | Example                                        |
|:--------------------------------------------------------|:---------------------------|:-----------------------------------------------|
| Work in progress                                        | `:construction:`           | :construction: new output structure            |
| Bug fix                                                 | `:bug:`                    | :bug: mean fails if NA                         |
| Fixing typos                                            | `:pencil2:`                | :pencil2: README                               |
| Code maintenance                                        | `:wrench:`                 | :wrench: fix variable names                    |
| New test                                                | `:clapper:`                | :clapper: wget JSON resource                   |
| Plot figures                                            | `:bar_chart:`              | :bar_chart: example boundaries                 |
| New data                                                | `:cd:`                     | :cd: example pollination network               |
| New feature                                             | `:sparkles:`               | :sparkles: (insert achievement)                |
| Documentation                                           | `:books:`                  | :books: lattice function                       |
| Performance improvement                                 | `:racehorse:`              | :racehorse: parallelizes models by default     |
| Upcoming release                                        | `:package:`                | :package: v1.0.6                               |
| Ugly but working code                                   | `:dragon:`                 | :dragon: added lattice function                |
| Working on code that doesn't work but I want to go home | `:neutral_face:`           | :neutral_face: for triangulation               |
| I forgot to save everything before committing           | `:sandwich:`               | :sandwich: what is saving                      |
| Jettisoned something                                    | `:boom:`                   | :boom: manifest                                |

## Workflow

This section describes the general steps to make sure that your contribution is
integrated rapidly. The general workflow is as follows:

1. Fork the repository (see *Branches, etc.* below)
2. Create an *explicitly named branch* from `develop` (if present) or `master`
3. Create a pull request *as soon as you make the first commit*
4. Be as explicit as possible on your goals
5. Do not squash / rebase commits while you work -- we will do so when merging

### Pull requests

Creating a pull request *before* you push any code will signal that you are
interested in contributing to the project. Once this is done, push often, and be
explicit about what the commits do (see commits, below). This gives the
opportunity for feedback during your work, and allow for tweaks in what you are
doing.

A *good* pull request (in addition to satisfying to all of the criteria below)
is:

1. Single purpose - it should do one thing, and one thing only
2. Short - it should ideally involve less than 250 lines of code
3. Limited in scope - it should ideally not span more than a handful of files
4. Well tested and well documented
5. Written in a style similar to the rest of the codebase

This will ensure that your contribution is rapidly reviewed and evaluated.

### Branches, etc.

The *tagged* versions of anything on `master` are stable releases. The `master`
branch itself is the latest version, but it *must* always work (after the first
tagged release). For more intensive development, use the `develop` branch, or
feature-specific branches. All significant branches are under continuous
