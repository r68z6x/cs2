java cWeek 8 and 9 Literate programming
(Communicating Results)

1 Default setting of the Quarto Manuscript
1.1 Create the folder
(1) Create an empty folder for Quarto Manuscript and give it a proper name.
(2) Click File-New File-Quarto project-Manuscript project.
(3) Choose the folder we created in step 1.
1.2 Check the main YAML
(1) title:
(2) authors:
(3) bibliography: article citation
1.3 Check the structure of working folder
(1) _quarto.yml: format YAML. This is related to metadata and front matter of the
manuscript. Different formats of output are customized in this ffle.
(2) index.qmd: we write in this main document.
(3) references.bib: your references (which can be downloaded through Google Scholar or
through Zotero).
(4) Rename index.qmd as 0_main_ffle.qmd.
11.4 Generate two additional markdown ffles
Those additional markdown ffles conduct analysis that complement this main ffle.
1_generate_number: remember to put your aﬀﬀliation here.
2_generate_ffgure: remember to put your aﬀﬀliation here.
2 Edit YAML section and YAML ffle
2.1 Change the main ffle name in YAML
Please go to _quarto.yml to change the default ffle name to manuscript: article:
0_main_ffle.qmd.
2.2 Python engine
jupyter: python3
2.3 Aﬀﬀliation
title: Assignment 3
aﬀﬀliation: University of Auckland
email: xxxx
2.4 Date
date: last-modiffed
2.5 Abstract
abstract: Please put your absract of assignment 3 here. Example: This course will teach
you data science workffow. The course will focus on Python for Finance and reproducible
analytical pipeline.
22.6 keywords
Please put your keywords here
keywords: - Quarto - Manuscript
2.7 Add PDF as one of the output
Go to _quarto.yml
add pdf: default at the next level paramater of format:
comment out jats: default
3 Render the manuscript
3.1 First try
Click the preview button in Vscode.
Additional folders generated: .quarto, _manuscript, _freeze
_freeze: code is not re-evaluated unless their source changes. A corresponding _freeze folder
will be created.
3.2 Click on Word and PDF icon form your folder
Please go to the folder you created at step 1 of Section 1.1
This probably does not work.
Solution 1: Click on Word and PDF icon within Vscode.
Solution 2: manually edit the format parameter within YAML.
3.3 Add number for each section
number-sections: true
34 Python code cells
4.1 Article Notebook: wrong way
If you only run the following code, The 代 写data、python
代做程序编程语言article notebook will not appear..
Mylist = [1,2,3,4]
4.2 Article Notebook: correct way
We have to print something or return an object to make Article Notebook show up.
[1, 2, 3, 4]
4.3 Echo code or not
In the code, we can add the following parameter to control whether code will be echoed in the
main text (not Article Notebook):
#| echo: true
More about code cells on the following page: https://quarto.org/docs/reference/cells/cellsjupyter.html
4.4
 Output results or not
#| output: false
Mylist = [1,2,3,4]
Mylist
4.5 Other useful code cells parametrs
#| code-fold: true (Collapse code into an HTML tag)
#| code-line-numbers: true (Include line numbers in code block output)
45 Numbers, ffgures, and tables
5.1 Inline code for numbers
The average gap of eruption is 2.5.
5.2 External embeds: a ffgure
Let us import a ffgure created in another QMD ffle.
Figure 1: Timeline of recent earthquakes on La Palma
Embed: please refer to https://quarto.org/docs/authoring/notebook-embed.html for details
of how to use embeds in Quarto.
5.3 External embeds: speciffc folded line of code
Use the following code to import pandas:
import pandas as pd
import numpy as np
5.4 Display tables
An example adapted from Quarto documentation. Table 1 shows information related to different
 car models.
Table 1: Example
mpg cylinders displacement horsepower weight
18 8 307 130 3504
15 8 350 165 3693
5Table 1: Example
mpg cylinders displacement horsepower weight
18 8 318 150 3436
16 8 304 150 3433
17 8 302 140 3449
15 8 429 198 4341
14 8 454 220 4354
14 8 440 215 4312
14 8 455 225 4425
15 8 390 190 3850
5.5 Add existing figures from a folder
Figure 2: A logo for BUSFIN 711
5.6 Cross References
We can cross-reference figures, tables, equations, sections, etc.
5.7 External embeds: several line of code
This is mainly for the purpose of demonstration:
6 1_generate_number
A (University of Auckland)
import pandas as pd
import numpy as np
67 Reference
Indirect citation: This is a simple placeholder for the manuscript’s main document (Knuth
1984).
Direct citation: Knuth (1984) is am important paper.
Add more references to references.bib file.
Acknowledgement: some of materials are adapted from Quarto oﬀicial documentation.
Knuth, Donald E. 1984. “Literate Programming.” Comput. J. 27 (2): 97–111. https://doi.or
g/10.1093/comjnl/27.2.97.
7

         
加QQ：99515681  WX：codinghelp
