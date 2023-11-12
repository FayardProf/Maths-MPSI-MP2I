# Maths-Info-MPSI-Fayard

Cours de maths et d'informatique commune en MPSI

Les documents sont sous licence Creative Commons : CC BY-SA

- Pour compiler les fichiers, il est nécessaire d'installer:
  - Les packages magnolia-conf.tex, magnolia-maths.tex et magnolia.cls afin qu'ils soient accessibles par
    votre distrubution LaTeX. Vous pouvez pour cela les mettre dans le même dossier que le fichier .tex
    que vous compilez mais le mieux est le mettre dans un dossier à part accessible par votre distribution.
    Le fichier slashbox.sty est aussi disponible si votre distribution ne le possède pas.
  - Une distribution Python avec minted est nécessaire pour la coloration syntaxique du cours de Python.
  - Ensuite, les fichiers sont compilables uns à uns. Il est possible de générer des polys en allant
    dans le dossier correspondant (par exemple Info-Commun-Cours/09-Poly pour le poly d'informatique
    commune). Puis, si vous avec un système Unix:
    - make get
    - make

- Le cours compile correctement sous :
  - macOS avec MacTeX 2022 et Anaconda 2022-05
  - Debian 12 (Une Ubuntu récente devrait fonctionner de la même manière), avec les packages LaTeX suivants
    - apt-get install texlive texlive-lang-french texlive-latex-extra texlive-pstricks texlive-fonts-extra texlive-science

- Les auteurs de ces cours sont :
  - François Fayard: Tout le cours de maths et d'info.
  - Jean-Baptiste Bianquis: Son cours a servi de base pour les chapitres d'info sur la représentation des données, la complexité et la correction.
