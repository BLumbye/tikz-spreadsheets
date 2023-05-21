# tikz-spreadsheets
A LaTeX package for easily drawing spreadsheets using TikZ

The documentation is WIP, but the package is usable. See the example below.

```latex
\begin{figure}[H]
    \begin{adjustbox}{max width=1\textwidth,center}
        \begin{tikzpicture}
            \spreadsheet[width=12,height=14,showheadings=false,mergedcells={A1-J2,C4-H4,C5-D5,E5-F5,G5-H5,I5-J5,A14-B14,C14-D14}]{table-annotation}
            
            \colorcells{table-annotation}{A1-J2}{blue!20}
            \colorcells{table-annotation}{C4-H4}{Goldenrod!75}
            \colorcells{table-annotation}{C5-J6}{Goldenrod!25}
            \colorcells{table-annotation}{A7-J7}{Red!20}
            \colorcells{table-annotation}{A10-J10}{Red!20}
            \colorcells{table-annotation}{B8-J9}{Green!20}
            \colorcells{table-annotation}{B11-J12}{Green!20}
            \colorcells{table-annotation}{A14-D14}{Blue!25}
            \colorcells{table-annotation}{L6-L9}{Gray!20}

            \celltext[c]{table-annotation}{A1-J2}{Title: Group Stage Comparison of UEFA European Championship Finalists\\(2008 and 2012)}
            \celltext[c]{table-annotation}{C4-H4}{Group Stage}
            \celltext[c]{table-annotation}{C5-D5}{Match 1}
            \celltext[c]{table-annotation}{E5-F5}{Match 2}
            \celltext[c]{table-annotation}{G5-H5}{Match 3}
            \celltext[c]{table-annotation}{I5-J5}{Total}
            \celltext[r]{table-annotation}{C6}{GF}
            \celltext[r]{table-annotation}{D6}{GA}
            \celltext[r]{table-annotation}{E6}{GF}
            \celltext[r]{table-annotation}{F6}{GA}
            \celltext[r]{table-annotation}{G6}{GF}
            \celltext[r]{table-annotation}{H6}{GA}
            \celltext[r]{table-annotation}{I6}{GF}
            \celltext[r]{table-annotation}{J6}{GA}
            \celltext[r]{table-annotation}{A7}{2008}
            \celltext[l]{table-annotation}{B8}{Germany}
            \celltext[r]{table-annotation}{C8}{2}
            \celltext[r]{table-annotation}{D8}{0}
            \celltext[r]{table-annotation}{E8}{1}
            \celltext[r]{table-annotation}{F8}{2}
            \celltext[r]{table-annotation}{G8}{1}
            \celltext[r]{table-annotation}{H8}{0}
            \celltext[r]{table-annotation}{I8}{4}
            \celltext[r]{table-annotation}{J8}{2}
            \celltext[l]{table-annotation}{B9}{Spain}
            \celltext[r]{table-annotation}{C9}{4}
            \celltext[r]{table-annotation}{D9}{1}
            \celltext[r]{table-annotation}{E9}{2}
            \celltext[r]{table-annotation}{F9}{1}
            \celltext[r]{table-annotation}{G9}{2}
            \celltext[r]{table-annotation}{H9}{1}
            \celltext[r]{table-annotation}{I9}{8}
            \celltext[r]{table-annotation}{J9}{3}
            \celltext[r]{table-annotation}{A10}{2012}
            \celltext[l]{table-annotation}{B11}{Italy}
            \celltext[r]{table-annotation}{C11}{1}
            \celltext[r]{table-annotation}{D11}{1}
            \celltext[r]{table-annotation}{E11}{1}
            \celltext[r]{table-annotation}{F11}{1}
            \celltext[r]{table-annotation}{G11}{2}
            \celltext[r]{table-annotation}{H11}{0}
            \celltext[r]{table-annotation}{I11}{4}
            \celltext[r]{table-annotation}{J11}{2}
            \celltext[l]{table-annotation}{B12}{Spain}
            \celltext[r]{table-annotation}{C12}{1}
            \celltext[r]{table-annotation}{D12}{1}
            \celltext[r]{table-annotation}{E12}{4}
            \celltext[r]{table-annotation}{F12}{0}
            \celltext[r]{table-annotation}{G12}{1}
            \celltext[r]{table-annotation}{H12}{0}
            \celltext[r]{table-annotation}{I12}{6}
            \celltext[r]{table-annotation}{J12}{1}
            \celltext[c]{table-annotation}{A14-B14}{GF = Goal For}
            \celltext[c]{table-annotation}{C14-D14}{GA = Goal Against}
            \celltext[l]{table-annotation}{L6}{\underline{Countries}}
            \celltext[l]{table-annotation}{L7}{Germany}
            \celltext[l]{table-annotation}{L8}{Spain}
            \celltext[l]{table-annotation}{L9}{Italy}
        \end{tikzpicture}
    \end{adjustbox}
    \caption{Table annotation labels}
    \label{fig:AnnotatedSpreadsheetExample}
\end{figure}
```