# LaTeX Documentation

Template from [HSLU Seiten 1-3 Bachelorarbeit LaTeX](https://www.overleaf.com/latex/templates/hslu-i-bachelor-thesis-template/cqgxdvbwydmt) on Overleaf.

[![latest release tag](https://img.shields.io/github/v/tag/nichtgian/latex?label=Download)](https://github.com/nichtgian/latex/releases/latest/download/Bericht.pdf)

## Documentation project setup

### Publish PDF (GitHub Actions)

Main inspiration was the [CV repository by cr2007](https://github.com/cr2007/CV/tree/main) on GitHub.

To build and deploy the document a new release tag has to be created on GitHub.

### Local development (VS Code + Docker)

Following the [guide](https://medium.com/@timju/latex-setup-with-vs-code-and-docker-612f998e1f23).

Setup Docker if not already done:

1. Run `wsl --install`  to install WSL on Windows and run `wsl --install -d Ubuntu-22.04` to download the Ubuntu distribution.
2. Install Docker Desktop. Virtualization needs to be enabled in the BIOS.

Then Setup LaTeX for VS Code

1. Install [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) extension.
2. The VS Code settings in this repo are defined in the `.vscode/settings.json` file. Else go to settings, search for `latex-workshop`. Enable Docker and put `ghcr.io/xu-cheng/texlive-full` as LaTeX image.
3. Preview document using `ctrl + alt + v`. The pdf is available in the `out` folder.
