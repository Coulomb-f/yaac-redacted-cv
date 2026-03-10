Awesome Source CV
=================

## About

**Awesome Source Latex CV** is a LaTeX template based on the [YAAC: Another Awesome CV](https://github.com/darwiin/yaac-another-awesome-cv) created by **Christophe Roger (Darwiin)**. 

This version is optimized for **LuaLaTeX** on Linux (specifically Fedora) and uses the **Source Sans Pro** font from Adobe, along with **Font Awesome** icons.

The original template and this derivative are published under the [CC BY-SA 4.0 License](https://creativecommons.org/licenses/by-sa/4.0/legalcode).

## Quick start

You can edit this CV by modifying the `.tex` files in this repository.

### Prerequisites

To compile this on Linux (Fedora), you will need TeX Live and the following packages:
- `texlive-luahbtex`
- `texlive-fontawesome`
- `texlive-tcolorbox`
- `texlive-sourcesanspro`
- `texlive-parskip`
- `texlive-preprint`
- `texlive-tools`
- `texlive-ulem`
- `texlive-grfext`
- `texlive-hyphen-german` (or your preferred language)

### Compilation

Use `lualatex` to compile:
```bash
lualatex cv.tex
```

## How to use **Awesome Source CV** latex class

### Construct the header

In the main `.tex` file, define your name and tagline:

```latex
\name{[FIRSTNAME]}{[LASTNAME]}
\tagline{[TAGLINE]}
```

Define your social and contact information in the `\socialinfo` block:

```latex
\socialinfo{
  \linkedin{[LINKEDIN]}
  \smartphone{[PHONE]}
  \email{[EMAIL]}
  \address{[ADDRESS]}
}
```

### Construct the _experiences_ section

Experiences are handled in the `experiences` environment using the `\experience` macro:

```latex
\begin{experiences}
  \experience
    {End date} {Experience title}{Company}{Location}
    {Begin date} {
                      \begin{itemize}
                        \item Item 1 description
                        \item Item 2 description
                      \end{itemize}
                    }
                    {Technology highlights}
\end{experiences}
```

## License

Latex class file `yaac-another-awesome-cv.cls` is published under the terms of the [LPPL Version 1.3c](https://www.latex-project.org/lppl.txt).

All content files are published under the terms of the [CC BY-SA 4.0 License](https://creativecommons.org/licenses/by-sa/4.0/legalcode).
