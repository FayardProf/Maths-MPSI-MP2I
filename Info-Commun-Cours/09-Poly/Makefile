all:
	git log -1 --format="format:\
                \\gdef\\GITAbrHash{%h}\
                \\gdef\\GITAuthorDate{%ad}\
                \\gdef\\GITAuthorName{%an}" >> vc.tex
	pdflatex --shell-escape cours-python.tex
	pdflatex --shell-escape cours-python.tex
	pdflatex --shell-escape cours-python.tex
clean:
	rm -f vc.tex
	rm -f exos-*
	rm -f cours-complexite.tex
	rm -f cours-correction.tex
	rm -f cours-flot_execution.tex
	rm -f cours-fonction.tex
	rm -f cours-graphe.tex
	rm -f cours-representation_donnees.tex
	rm -f cours-structure_sequentielle.tex
	rm -f cours-valeur_type_variable.tex
	rm -f fiche.txt
	rm -f tmp.inputs
	rm -Rf _minted*
	rm -f cours-auto*
	rm -f cours.pdf
	rm -f cours.log
	rm -f cours.aux
	rm -f cours.maf
	rm -f cours.toc
	rm -f cours.mtc*
	rm -f tp-chaine_caractere.tex
	rm -f tp-fonction_flot_execution.tex
	rm -f tp-prog_imperative.tex
	rm -f tp-sudoku.tex
	rm -f tp-tableau_pile_file.tex
	rm -f tp-valeur_type_variable.tex
	rm -f tp-cryptage_cesar.tex
	rm -f tp-listes_gauss.tex
	rm -f tp-introduction_logo.tex
	rm -f tp-altimetre_syracuse.tex
	rm -f tp-cryptage_cesar.tex
	rm -f tp-bdd_mondial.tex
	rm -f tp-sudoku.tex
	rm -f tp-coupe_somme_minimale.tex
	rm -f tp-levenshtein_hamming.tex
	rm -f tp-recursif_horizon.tex
	rm -f cours-structure_donnees.tex
	rm -f cours-structures_donnees.tex
	rm -f cours*mtc*
	rm -f *.aux
	rm -f *.toc
	rm -f *.maf
	rm -f *.log
	rm -f tp-*.tex
get:
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-Cours/01-ValeurTypeVariable/cours-valeur_type_variable.tex > cours-valeur_type_variable.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-Cours/02-FlotExecution/cours-flot_execution.tex > cours-flot_execution.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-Cours/03-Fonction/cours-fonction.tex > cours-fonction.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-Cours/04-Liste/cours-structure_sequentielle.tex > cours-structure_sequentielle.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-Cours/05-RepresentationDonnees/cours-representation_donnees.tex > cours-representation_donnees.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-Cours/06-Complexite/cours-complexite.tex > cours-complexite.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-Cours/07-Correction/cours-correction.tex > cours-correction.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-Cours/08-Graphe/cours-graphe.tex > cours-graphe.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-Exos/01-ValeurTypeVariable/exos-valeur_type_variable.tex > exos-valeur_type_variable.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-Exos/02-FlotExecution/exos-flot_execution.tex > exos-flot_execution.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-Exos/03-Fonction/exos-fonction.tex > exos-fonction.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-Exos/04-Liste/exos-structure_sequentielle.tex > exos-liste.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-Exos/05-RepresentationDonnees/exos-representation_donnees.tex > exos-representation_donnees.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-Exos/06-Complexite/exos-complexite.tex > exos-complexite.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-Exos/07-Correction/exos-correction.tex > exos-correction.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-Exos/08-Graphe/exos-graphe.tex > exos-graphe.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-TPs/01-IntroductionLogo/tp-introduction_logo.tex > tp-introduction_logo.tex
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-TPs/02-AltimetreSyracuse/tp-altimetre_syracuse.tex > tp-altimetre_syracuse.tex 
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-TPs/03-CryptageCesar/tp-cryptage_cesar.tex > tp-cryptage_cesar.tex 
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-TPs/04-LevenshteinHamming/tp-levenshtein_hamming.tex > tp-levenshtein_hamming.tex 
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-TPs/05-RecursifHorizon/tp-recursif_horizon.tex > tp-recursif_horizon.tex 
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-TPs/06-Sudoku/tp-sudoku.tex > tp-sudoku.tex 
	sed -e '/BEGIN_BOOK/,/END_BOOK/!d' ../../Info-Commun-TPs/07-CoupeSommeMinimale/tp-coupe_somme_minimale.tex > tp-coupe_somme_minimale.tex 
diff:
	git latexdiff HEAD -- --main cours-sup.tex --latexopt "--shell-escape"
