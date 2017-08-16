# opendyslexic_latex_example
A how-to showing install and use of open dyslexic fonts in latex documents.

Nathan Moore, Winona State University, nmoore@winona.edu

I've read [anecdotally](https://theestablishment.co/hating-comic-sans-is-ableist-bc4a4de87093#.jfq7z1s6a) that people who struggle with dyslexia can benefit from fonts which are intentionally designed to be asymmetric.  One font like this is "Open Dyslexic", http://opendyslexic.org/.  I write exams in the tex/latex typesetting language, and know tex at the dilletante level. So, the question I wanted to answer was, "How can I typeset a document and use Open Dyslexic fonts?"

Assumptions: I am working on a Windows 8 computer with MiKTeX 2.9 installed.

Procedure:

1. Download the fonts from http://opendyslexic.org/ or https://github.com/antijingoist/open-dyslexic/.
2. Unzip the fonts and drag them to c:\Windows\Fonts\ - this seems to complete the "installation."
3. Open a .tex file in a MiKTeX-linked editor (I'm using TeXworks 0.6.1, which seems pretty standard).
4. Add the following two lines to the document, in the "preamble" before the `\begin{document}` line:
  * `\usepackage{fontspec}`
  * `\setmainfont{Open Dyslexic}`
5. Finally, in the typeset window, use **LuaLaTeX** as the typesetting engine. ![alt_text](https://github.com/ntmoore/opendyslexic_latex_example/blob/master/LuaLaTeX.png "a screenshot showing the LuaLaTeX typesetting option")

A source file, with images, and pdf output are included in this repository.
