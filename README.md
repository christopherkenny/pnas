
# PNAS Article Quarto Template

## Creating a New Article

To create a new article using this format:

```bash
quarto use template christopherkenny/pnas
```

This will create a new directory with an example document that uses this format.

## Using with an Existing Document

To add this format to an existing document:

```bash
quarto add christopherkenny/pnas
```

Then, add the format to your document options:

```yaml
format:
  pnas-pdf: default
```    

## Options

The default setting for class option generates a two column layout with:

```
classoption:
 - twocolumn
 - twoside
```
To set a corresponding author, ensure that the attribute "corresponding" is true and that they have an email listed.

For proper formatting, each affiliation should be given a letter id (like `a`, `b`, ..., `z`).

This template is designed for `template_type: pnasresearcharticle` (the default).
It can also take options `pnasmathematics` or `pnasinvited`, but these are not formally supported, as they have official alternative formats available on [Overleaf](https://www.overleaf.com/gallery/tagged/pnas).

## Example

Here is the source code for a minimal sample document: [template.qmd](template.qmd).

<!-- pdftools::pdf_convert('template.pdf', pages = 1)  -->
![[template.qmd](template.qmd)](template_1.png)

## License

This modifies the Overleaf PNAS Template, available at <https://www.overleaf.com/latex/templates/template-for-preparing-your-research-report-submission-to-pnas-using-overleaf-2023/whbdryzwztnd>. The original template is licensed under the [LaTeX Project Public License 1.3c](https://www.latex-project.org/lppl/lppl-1-3c/). The template within is derived from this and makes modifications to separate into the full document into Quarto "partials". All modifications can be seen in this repo. 

