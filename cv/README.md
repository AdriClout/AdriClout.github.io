# CV Directory Structure

This directory contains Adrien Cloutier's curriculum vitae in both French and English, organized for easy maintenance and bilingual website support.

## Directory Organization

```
cv/
├── Français/                           # French CV files
│   ├── CloutierAdrien_CV_3pages.pdf   # Current French CV (3 pages)
│   ├── CloutierAdrien_CV_3pages.tex   # LaTeX source for French CV
│   └── cv_fr.png                       # Preview image for website
│
├── Anglais/                            # English CV files
│   ├── CloutierAdrien_CV_english.pdf  # Current English CV (3 pages)
│   ├── CloutierAdrien_CV_english.tex  # LaTeX source for English CV
│   └── cv_en.png                       # Preview image for website
│
├── cv.pdf                              # Legacy file (kept for backward compatibility)
├── cv.png                              # Legacy file (kept for backward compatibility)
└── README.md                           # This file
```

## File Descriptions

### French CV (Français/)
- **CloutierAdrien_CV_3pages.pdf**: The current French CV, last updated November 2024
- **CloutierAdrien_CV_3pages.tex**: LaTeX source file using ModernCV template (classic style, blue color)
- **cv_fr.png**: Preview image (first page) used on the French version of the website

### English CV (Anglais/)
- **CloutierAdrien_CV_english.pdf**: The current English CV, translated from the French version
- **CloutierAdrien_CV_english.tex**: LaTeX source file (identical structure to French version)
- **cv_en.png**: Preview image (first page) used on the English version of the website

### Legacy Files
- **cv.pdf**: Older CV file kept for backward compatibility with external links
- **cv.png**: Older preview image kept for backward compatibility

## Usage on Website

### French Version (index.html)
```html
<a href="cv/Français/CloutierAdrien_CV_3pages.pdf">
  <img src="cv/Français/cv_fr.png" alt="Aperçu du CV" />
</a>
```

### English Version (index_en.html)
```html
<a href="cv/Anglais/CloutierAdrien_CV_english.pdf">
  <img src="cv/Anglais/cv_en.png" alt="CV Preview" />
</a>
```

## Updating CVs

### To update the French CV:
1. Edit `Français/CloutierAdrien_CV_3pages.tex`
2. Compile with pdflatex:
   ```bash
   cd cv/Français
   pdflatex CloutierAdrien_CV_3pages.tex
   pdflatex CloutierAdrien_CV_3pages.tex  # Run twice for references
   ```
3. Regenerate preview:
   ```bash
   qlmanage -t -s 1000 -o . CloutierAdrien_CV_3pages.pdf
   mv CloutierAdrien_CV_3pages.pdf.png cv_fr.png
   ```

### To update the English CV:
1. Edit `Anglais/CloutierAdrien_CV_english.tex`
2. Compile with pdflatex:
   ```bash
   cd cv/Anglais
   pdflatex CloutierAdrien_CV_english.tex
   pdflatex CloutierAdrien_CV_english.tex  # Run twice for references
   ```
3. Regenerate preview:
   ```bash
   qlmanage -t -s 1000 -o . CloutierAdrien_CV_english.pdf
   mv CloutierAdrien_CV_english.pdf.png cv_en.png
   ```

### Important Notes:
- **Keep both versions synchronized**: When updating content, make sure both French and English CVs contain the same information
- **Proper nouns**: Do not translate "Université Laval", EIOM, RFICS, CLESSN, and other organizational names
- **Publications**: Keep publication titles in their original language/format
- **Preview images**: Always regenerate preview images after updating PDFs

## LaTeX Template

Both CVs use the ModernCV LaTeX template:
- **Style**: classic
- **Color**: blue
- **Font size**: 11pt
- **Paper**: A4

### Required LaTeX packages:
- moderncv
- soul
- lmodern
- geometry
- lastpage
- fancyhdr

## Contact

For questions about CV updates or structure, contact:
- Email: adrien.cloutier.1@gmail.com
- Website: https://adriencloutier.com
