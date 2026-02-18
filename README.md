# IMO Problems — LaTeX Source Collection

A complete collection of [International Mathematical Olympiad (IMO)](https://www.imo-official.org/) problem sets in LaTeX, covering every competition from **1959 to 2025** (66 contests; 1980 is omitted as no IMO was held that year).

## Repository Structure

```
imo_latex/        # LaTeX source files  (1959.tex – 2025.tex)
imo_pdfs/         # Compiled PDFs        (1959_eng.pdf – 2025_eng.pdf)
```

Each `.tex` file is a self-contained document that typesets the six problems of the corresponding year using standard AMS-LaTeX packages (`amsmath`, `amssymb`).

## Usage

### Compile a single year

```bash
pdflatex imo_latex/2024.tex
```

### Compile all years

```bash
for f in imo_latex/*.tex; do pdflatex "$f"; done
```

Pre-compiled PDFs are available in `imo_pdfs/` if you prefer not to compile locally.

## Coverage

| Range | Years included |
|-------|---------------|
| 1959 – 1979 | 21 contests |
| 1981 – 2025 | 45 contests |
| **Total** | **66 contests · 396 problems** |

## Notes

- Problem statements are in **English**.
- Each file contains exactly the official problem statements — no solutions or hints.
- LaTeX source is minimal and dependency-free beyond a standard TeX distribution (TeX Live / MiKTeX).

## License

Problem statements are the intellectual property of the IMO and its host countries. This repository redistributes them for educational and research purposes only.
