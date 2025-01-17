# Land_Atmosphere_interactions_notes

Repository containing the practical material for the course of [Land-Atmosphere Interactions](https://studiekiezer.ugent.be/2025/studiefiche/en/I002451). This course materials is also hosted as a website at https://obonte.quarto.pub/land-atmosphere-interactions-practicals/.

The assignment (without solutions) can be found on a [public repository](https://github.com/olivierbonte/Land_Atmosphere_interactions_notes_public). The solutions are in a [private repository](https://github.com/olivierbonte/Land_Atmosphere_interactions_notes), access to which can be granted upon [contacting me](mailto:olivier.bonte@hotmail.com).

## Installation instructions

First, make a local copy of this repository using

```
git clone https://github.com/olivierbonte/Land_Atmosphere_interactions_notes.git
```

or download as zip file and unzip. In each case, make sure to navigate inside the `Land_Atmosphere_interactions_notes` practical before executing any of the command line interface (CLI) instructions below.

Go to the [Quarto download page](https://quarto.org/docs/download/) and download Quarto for your operating system (OS). This repository was built using Quarto 1.6.39.

Next, make sure you have (Mini)Conda installed (download links found [here](https://docs.anaconda.com/miniconda/)). Next open your CLI (or Anaconda prompt) and type:

```
conda env create -f environment.yml
conda activate la_interactions_quarto
```

In this repository, the final output is rendered to pdf. Therefore, [a LaTeX distribution is needed](https://quarto.org/docs/output-formats/pdf-basics.html#prerequisites). If you don't have a [Tex distribution](https://www.latex-project.org/get/#tex-distributions) installed on your machine, install the [TinyTex distribution](https://yihui.org/tinytex/), a lightweight version of [TeX Live](https://www.tug.org/texlive/), with following command in the CLI:

```
quarto install tinytex
```

To render the diagrams, made with [Mermaid](https://mermaid.js.org/intro/), [quarto needs the Chrome or Edge browser](https://quarto.org/docs/authoring/diagrams.html#chrome-install). If neither is present on your device, you can opt to download a lightweight version of chrome with following CLI command:

```
quarto install chromium
```

There are several ways to use Quarto, but here [VS Code](https://code.visualstudio.com/Download) is used as interface. With VS Code installed for you OS, perform the following:

1. Under extensions, install the [Quarto extension](https://marketplace.visualstudio.com/items?itemName=quarto.quarto).
2. Follow the instructions [here](https://code.visualstudio.com/docs/python/environments#_select-and-activate-an-environment) and select `la_interations_quarto` as your Python interpreter for VS Code.
3. To have a nice preview of your `.qmd` quarto document, use `Ctrl + Shift + k`. After modifying the `.qmd` document, use the same key combination to render the preview again. Alternatively, run `quarto preview` in the CLI (this should normally eliminate the need to use `Ctrl + Shift + k` repeatedly).
4. To render the entire set of documents as one `.pdf`, type `quarto render` in the command line. Under the `_book` folder, you can then find the render `.pdf`.
