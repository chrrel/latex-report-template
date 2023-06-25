# LaTeX Template for Reports and Theses 
This is a LaTeX template that can be used for reports and theses. An example PDF file can be found [here](report/report.pdf).

## Structure
The template depends on the following files.

- **acronyms.tex** - Define used acronyms here.
- **addons.tex** - Title page, quotation page, declaration and abstract. Usually there is no need to modify this file.
- **appendix.tex** - The appendix.
- **bilbiography.bib** - The bibliography.
- **content.tex** - The content file contains all chapters of your work.
- **report.tex** - The main file of this template. Nearly all settings can be changed here (including information displayed on the title page etc.). 
- **makefile** - The makefile for compiling the code.

## How to Use The Template
To compile the template to a PDF file, you can use the makefile in this repository.

`make` - Compile the project and create a PDF file.

`make clean` - Delete the output directory.

> **Note:**
> The package `latexmk` is required for compiling the project.

The option `isPrintVersion` can be changed in line 3 of *report.tex*. If it is set to true, all links in the generated PDF will be black, if it is set to false coloured links will be used.

## New Commands in this Template
This template comes with new, non-standard LaTeX commands which are explained in this section. You can also find an example of them in the [PDF example](report/report.pdf).

Add a source to a figure or listing with the `captionsource` command.

````LaTeX
\captionsource{\cite{abc:01}}

\captionsource[https://example.org]{J. Doe}
````

Format code inside paragraphs using the `code` command.
````LaTeX
 \code{UPDATE} 
````

Write definitions in a `define` environment.
````LaTeX
\begin{define}
	Let A be ...
\end{define}
````

## License
This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/).
