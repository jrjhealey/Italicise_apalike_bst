# Italicise_apalike_bst
A modified `apalike.bst` LaTeX bibliography style file to include italicised 'et al.'s'


### 'Installing'

In order to use this alternative `.bst` file, download the file itself to the *same directory* as the `.tex` document which constructs your bibliography. This must be done so that your TeX application prioritises it over the default files located among the system files.
i.e.:

    ../                         <---- Document top level folder
     |
     |-- document.tex           <---- Document file that calls \bibliographystyle{}
     |
     |-- customapalike.bst      <---- Modified file from this repository
      
In your `.tex` file, you should then have something that resembles the following:

```tex
%% Preamble
\documentclass[]{} % Doc Setup

\begin{document}
...document body...

\bibliographystyle{customapalike}
\bibliography{/path/to/mybibfile.bib}
\end{document}
```

Set the `\bibliographystyle{customapalike}` using the name of the downloaded `.bst` file. If it is in the same directory as the main `.tex` file, you shouldnt need to specify the extension or the full filepath.

It should yeild the following (remember you will need to do a 'full TeX compilation cycle'; TeX -> BibTeX -> TeX -> TeX)

<a href="https://ibb.co/jeBfip"><img src="https://preview.ibb.co/njNmOp/Screen_Shot_2018_10_10_at_11_21_58.png" alt="Screen Shot 2018 10 10 at 11 21 58" border="0" /></a>
