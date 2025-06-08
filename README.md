# Overleaf Optimizer
Created by Clemens Lode, https://www.lode.de, 2026

This template hooks into Overleaf's draft and compiler setting and configures your LaTeX project either for maximum speed or maximum quality. The template is an excerpt from the "LaTeX Book Publishing in 2026" template by LODE Publishing (https://www.lode.de).

The optimizer works with pdfLaTeX, XeLaTeX, and LuaLaTeX. pdfLaTeX supports protrusion, expansion, and tracking, while LuaLaTeX only supports protrusion and expansion, and XeLaTeX only supports protrusion.

That puts pdfLaTeX ahead, but LuaLaTeX and XeLaTeX support OpenType fonts. So, with LuaLaTeX, you get the best quality for OpenType fonts, with pdfLaTeX the best (and fastest) quality for Type 1 fonts.

For maximum efficiency:

- Use pdfLaTeX with a Type 1 font (e.g., libertinus) in draft mode throughout the development of your document or book.
- Switch to LuaLaTeX with maximum quality and OpenType font (e.g., libertinus-otf) when preparing the document or book for publication (i.e., looking line-by-line, fixing white space, fixing orphans/widows, etc.).


## Directory Structure

### Packages
- `lib/typography.tex` - Loads fontenc/fontspec depending on the draft/normal mode setting. Also loads xurl and microtype with draft/normal mode options.

### Configuration
- `settings/publisher.tex` - Select font 
- `style/polishing` - Draft vs normal mode settings

### Root
- `main.tex` - Entry point for compilation
- `preamble.tex` - Initializes PDF 2.0 and recognizes draft mode

Each directory contains specific components to keep the project organized. See individual sections below for details about each directory's contents and usage.


## Support & Contact
- Book: https://www.lode.de/book/lbp2026
- Support: mail@lode.de
- Website: https://www.lode.de
- Newsletter: https://www.lode.de/newsletter