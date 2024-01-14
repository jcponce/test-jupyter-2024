# Markdown Files

Whether you write your book's content in Jupyter Notebooks (`.ipynb`) or
in regular markdown files (`.md`), you'll write in the same flavor of markdown
called **MyST Markdown**.
This is a simple file to help you get started and show off some syntax.

## What is MyST?

MyST stands for "Markedly Structured Text". It
is a slight variation on a flavor of markdown called "CommonMark" markdown,
with small syntax extensions to allow you to write **roles** and **directives**
in the Sphinx ecosystem.

For more about MyST, see [the MyST Markdown Overview](https://jupyterbook.org/content/myst.html).

## Sample Roles and Directives

Roles and directives are two of the most powerful tools in Jupyter Book. They
are kind of like functions, but written in a markup language. They both
serve a similar purpose, but **roles are written in one line**, whereas
**directives span many lines**. They both accept different kinds of inputs,
and what they do with those inputs depends on the specific role or directive
that is being called.

Here is a "note" directive:

```{note}
Here is a note
```

It will be rendered in a special box when you build your book.

Here is an inline directive to refer to a document: {doc}`markdown-notebooks`.

## Citations

You can also cite references that are stored in a `bibtex` file. For example,
the following syntax: `` {cite}`holdgraf_evidence_2014` `` will render like
this:

Moreover, you can insert a bibliography into your page with this syntax:
The `{bibliography}` directive must be used for all the `{cite}` roles to
render properly.
For example, if the references for your book are stored in `references.bib`,
then the bibliography is inserted with:

## We can use maths

Let's try to use some maths $\N$

$$
\bmat{cc} 1 & 1 \\ 2 & 2 \emat
$$

## We can use iframes

Let's use some iframes now.

### This is a MathBox applet

<iframe scrolling="no" style="border:0px;" src="https://topologia-general.github.io/sketches/hopf/" width="100%" height="380px"></iframe>

### This is a MathCell applet

<iframe scrolling="no" style="border:0px;" src="https://www.dynamicmath.xyz/sketches/mathcell/eversion/" width="500px" height="500px"></iframe>

### This a GeoGebra applet

<iframe scrolling="no" title="Slope field explorer" allowfullscreen=""
        src="https://www.geogebra.org/material/iframe/id/dabkhkqr/width/712/height/404/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/true/rc/false/ld/false/sdz/false/ctl/false"
        width="100%" height="404px" style="border:0px;"> </iframe>

### This is an example with p5js

<iframe style="border:0px;" src="https://www.dynamicmath.xyz/sketches/tesseract/" width="500px" height="500px"
scrolling="no"></iframe>

## These are images 

Try to add some images.

### This a PNG

<img src="https://www.geogebra.org/resource/fkwhfwez/uieZ2zy9C1R5i9IX/material-fkwhfwez.png" style="width:70%"
alt="fractal tree">

### This is a GIF

<img
src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgJDbwRHyvFdQLTSeFQGv8Fu7vh2m-ah4JCwoP9oNtLHwpPlOgww50HOu-DIAIryl-8357glsTyawl84kdHIs4p8WkiO3wyycbrGzH8NPtJND0RaoIwhp5p_XNL0F2IQvZjYW1yR2AEaK5indISRPWFkKJoMtAUnGApPxCH3HCkZC-zOrsG14dmZxrUXXfH/w1152/ggb-snow.gif"
style="width:70%" alt="Snow">

## Learn more

This is just a simple starter to get you started.
You can learn a lot more at [jupyterbook.org](https://jupyterbook.org).

```{tableofcontents}
```