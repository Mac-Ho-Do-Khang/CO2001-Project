### Structure

```
CO2001-Project
├── abstraction
│   └── main.tex
├── appendix
│   └── main.tex
├── components
│   ├── equipment
│   │   ├── ender3-v2.tex
│   │   ├── esp32-ttgo-tdisplay.tex
│   │   └── main.tex
│   ├── image
│   │   └── ...
│   ├── main.tex
│   ├── materials
│   │   ├── main.tex
│   │   └── pla.tex
│   └── software
│       ├── arduino.tex
│       ├── cura.tex
│       ├── fusion360.tex
│       └── main.tex
├── conclusion
│   ├── future-work.tex
│   ├── main.tex
│   └── summary.tex
├── development-testing
│   ├── development
│   │   ├── analysis.tex
│   │   ├── electrical.tex 
│   │   ├── image
│   │   │   └── ...
│   │   ├── main.tex
│   │   ├── mechanical.tex 
│   │   └── programming.tex
│   ├── main.tex
│   └── testing            
│       ├── image
│       └── main.tex
├── hcmut.png                   # HCMUT logo for title page
├── introduction
│   ├── main.tex
│   ├── objectives.tex
│   ├── overview.tex
│   └── structure.tex
├── main.pdf                    # Compiled PDF report
├── main.tex                    # Primary LaTeX entry point
├── README.md
├── refs.bib                    # Bibliography file
├── related-work
│   ├── byte90.tex
│   ├── image
│   │   └── ...
│   └── main.tex
└── theoretical-background
    ├── 3d-printing.tex
    ├── dfma.tex
    ├── image
    │   └── ...
    └── main.tex
```

### Owner's Setup

- LaTeX distribution: [MiKTeX](https://miktex.org/download/ctan/systems/win32/miktex/setup/windows-x64/basic-miktex-25.12-x64.exe)
- Editor: Visual Studio Code with LaTeX Workshop (_james-yu.latex-workshop_) extension
- Compilation: `Ctrl+Alt+B` to compile `./main.tex` → `./main.pdf`
  - Install any missing packages via MiKTeX when prompted

### To Write More

1. Open relevant chapter file → Write content → Save
2. If adding a new sub-section file, `\input{}` it from the chapter's `main.tex`
3. Add any references to `refs.bib` using BibTeX format and cite with `\cite{}`
    - Refer [here](https://www.bibtex.com/e/entry-types/) for entry types
    - Online sources shall be cited with `@misc` and include the URL and access date
4. Place images in the chapter's `image/` folder and reference them with `\includegraphics{}`
    - Cite the source of the image in the caption via `\cite{}` if not original
    - Add `\label{}` to the figure for referencing in `\listoffigures`