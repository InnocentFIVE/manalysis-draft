# manalysis-draft

This is a draft version of the `manalysis` LaTeX package.

This package was originally designed to auto-resize parentheses in math mode, but later, additional modules were added.

## System requirements

The user is recommended to use TeX Live version 2024 or newer. All testing by the author was conducted on an Arch Linux distribution with the `texlive-basic` package version 2025.2-2. No testing has been performed on MacOS.

This package is highly experimental.

## Usage

Use `\usepackage{manalysis}` to load the package as usual in LaTeX. Then, introduce the desired *modules* of the package.

A *module* can be regarded as a sub-package of `manalysis`, which can be loaded using

```tex
\UseManalysisModule{<module>}
```

or

```tex
\UseManalysisModule{*}
```

The latter command will load all modules.

| File                        | Description                                                                             |
| --------------------------- | --------------------------------------------------------------------------------------- |
| `manalysis.sty`             | Core package                                                                            |
| `manalysis-accent.sty`      | Auxiliary module for automatically adjusting the width of accents in formulas           |
| `manalysis-bigop.sty`       | Auxiliary module for converting arbitrary mathematical expressions into large operators |
| `manalysis-paren.sty`       | Auxiliary module for automatically adjusting the height of parentheses in formulas      |
| `manalysis-pms.sty`         | Auxiliary module providing rough shapes using `l3draw` or TikZ                          |
| `manalysis-rfrac.sty`       | Auxiliary module providing a simple horizontal fraction command based on table syntax   |
| `manalysis-stackcenter.sty` | Auxiliary module for centering one symbol over another                                  |
| `manalysis-trifunc.sty`     | Auxiliary module for generating trigonometric functions like $\mathrm e^{\mathrm ix}$   |
