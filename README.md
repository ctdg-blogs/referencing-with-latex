## Referencing with Latex
---
This repository is a collection of the referencing rules with latex
<br>
Some skills of paper make-ups are also included
<br>
`--` denotes `\begin{document}` in latex
<br>
`/` denotes alternative instructions

---
#### fonts and papers

   + improve font functions
   ```latex
   \usepackage[T1]{fontenc}
   \usepackage[utf8]{inputenc}
   --
   ```
   + line space
   ```latex
   \usepackage{setspace}
   --
   \begin{spacing}{2.0}   %double space
   \end{spacing}
   ```
   + paper settings & font size
   ```latex
   \documentclass[a0,landscape/portrait,11pt]{article}
   --
   ```

   | Instruction | settings |
   | ---- | ---- |
   | a0 | paper size |
   | landscape | 横向排版 |
   | portrait | 纵向排版 |
   + font style
      + Times New Roman
      ```latex
      \usepackage{times}
      --
      ```
   + inline font settings

   | Instructions | style |
   | ---- | ---- |
   | \textbf{word} | $\textbf{word}$
   
---
#### references

+ basic instructions
   ```latex
   \bibliography{reference}
   ---
   \cite{refer-name}
   \bibliographystyle{plain}
   \printbibliography
   ```
   where `reference` is the name of .bib file
+ .bib instructions
   ```bib
   @inbook{refer-name,
   author={A,B / A and B},
   editor={·},
   title={·},
   year={·},
   publisher={·},
   address={·},
   pages={·},
   isbn={·},
   doi={·},
   url={·}
   }
   ```
   ```bib
   @article{refer-name,
   author={·},
   title={·},
   journal={·},
   volume={·},
   number={·},
   year={·},
   abstract={·}
   }
   ```
   ```bib
   @msic{url-name,
   howpublished={\url{https://www.your-reference-web.com}},
   title={·},
   author={·},
   note={Accessed/Retrieved + date},
   }
   ```
   bibtex styles : article, book, booklet, conference, inbook, incollection, inproceedings, manual, misc, mastersthesis, phdthesis, proceedings, techreport, unpublished 
+ bibliographystyle

| instruction | list order / style |
| ---- | ---- |
| plain / alpha | alphabetical (author, year, title) |
| unsrt | same as bib file |
| abbrv | close-knit |
| ieeetr | 国际电气电子工程师协会期刊 |
| acm | 美国计算机学会期刊 |
| siam | 美国工业和应用数学学会期刊 |
| apalike | 美国心理学学会期刊 |


   ---
   #### useful websites list
   + templates 
      + [www.latextemplates.com](www.latextemplates.com)
      + [www.overleaf.com/latex/templates](https://www.overleaf.com/latex/templates)
   + reference 
      + [chicago style](https://www.overleaf.com/latex/examples/the-chicago-citation-style-with-biblatex/pdqqrmwtdqpc)
   + cooperation @ [www.overleaf.com](www.overleaf.com)