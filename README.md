# Md Mustafizur Rahman - Academic CV

This CV reflects my academic journey.

## Download

![Workflow name](https://github.com/mustafizur-r/mustafizur_cv/actions/workflows/latex_build.yml/badge.svg?branch=main)

Changes are automatically updated with CI/CD, and the latest version is always accessible through the following link:

https://github.com/mustafizur-r/mustafizur_cv/releases/download/latest-release/mustafizur_cv.pdf

## How to Compile

This CV is compiled using `pdflatex`, ensuring wide compatibility and easy reproduction of the document.

To compile the CV from source with local LaTeX environment:
1. Install `texlive-full`
2. Run the following command in your terminal:

   ```bash
   pdflatex -output-directory=build mustafizur_cv.tex
   ```

To compile the CV from source with Docker:
1. The project uses `texlive/texlive` Docker container for compilation.
2. Run the following command in your terminal:

   ```bash
   docker run --rm -v $PWD:/workdir texlive/texlive pdflatex -output-directory=/workdir/build /workdir/mustafizur_cv.tex
   ```
