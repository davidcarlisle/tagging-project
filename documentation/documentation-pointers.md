## Overview about documentation for tagging documents

In  general one can use the command `texdoc <package-name>` on the command line to get documentation about a specific package. Instead of using `texdoc` on your machine you can also use the online version at [https://texdoc.org](https://texdoc.org/index.html).


The following list gives an overview about different packages related to tagging and some details on the contents of each:

+ [`ltnews.pdf`](https://texdoc.org/serve/ltnews/0) (or `ltnews<number>.pdf`)
   LaTeX news (one for each LaTeX release) discusses relevant changes and enhancements in LaTeX in particular also updates and improvements for tagging of documents
   
+ [`documentmetadata-support-code.pdf`](https://texdoc.org/serve/documentmetadata-support-code.pdf/0)
  Contain details about `\DocumentMetadata` and the various supported settings, e.g. pdfstandard, lang, pdfversion
  
+ [`latex-lab-graphic.pdf`](https://texdoc.org/serve/latex-lab-graphic/0)
  Details on graphics tagging - including description for artifact, alt, actualtext, samples for tikz
  
+ [`latex-lab-math.pdf`](https://texdoc.org/serve/latex-lab-math/0)
  Details on math tagging and special treatment capturing math contents
  
+ [`latex-lab-table.pdf`](https://texdoc.org/serve/latex-lab-table/0)
  Details on table tagging - which table types are supported, which not; headers and rows, columns, etc.
  
+ [`blocks-doc.pdf`](https://texdoc.org/serve/blocks-doc/0) (or [`blocks-code.pdf`](https://texdoc.org/serve/blocks-code/0))
  How to declare and customize block-level environments, such as `center` or lists, etc.
  
+ [`l3pdfmeta.pdf`](https://texdoc.org/serve/l3pdfmetadata/0)
  Details on PDF-standards (from the perspective of LaTeX implementation)
  
+ [`tagpdf.pdf`](https://texdoc.org/serve/tagpdf/0)
  Documentation of low-level tagging commands and methods; description of `\tagpdfsetup` and the key/values it supports

For example, `texdoc ltnews41` opens the LaTeX news for release 2025-06-01. Without the number, a document with the release notes from all releases since 1994 is opened.  Similarly, `texdoc blocks-doc` will open the documentation on tagging of block-level environments for you.

To find a complete list of the currently available documents from the `latex-lab` please look at: [https://ctan.org/tex-archive/macros/latex-dev/required/latex-lab](https://ctan.org/tex-archive/macros/latex-dev/required/latex-lab).

Please also note that most of the documentation (as well as this page) is  "work in progress". Therefore, the list above might not completely reflect the current status of implementation.



## Testing Tagged PDF documents

If you have a tagged PDF document and want to check the of the tagging you can try

+    [`VeraPDF`](https://dev.verapdf-rest.duallab.com/) - online -  has a good validation mechanism
+    [`PAC`](https://pac.pdf-accessibility.org/) - Windows only; it only understands PDF1.7 and PDF/UA-1 documents but not PDF2-0 and PDF/UA-2
+    [`ngPDF`](https://ngpdf.com/) - online - deriving HTML from tagged PDF
+    [`showtags`](https://texlive.net/showtags) - Evaluating the PDF-structure  (This tool is produced by the LaTeX Project)
