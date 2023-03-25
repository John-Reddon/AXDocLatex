# Comment utiliser le template AXDoc
C'est assezsimple, tout est déjà automatisé

 - téléchargez le dossier AXDoc
 - Créez un fichier `tex` à côté de ce dossier.
 - Commencez le document par :

```
\documentclass[a4paper, 12pt]{extarticle}

% Enter all fields in the following and run the compilation TWICE [!]
\newcommand{\docType}{AFF XXX}
\newcommand{\client}{CLIENT}
\newcommand{\projectName}{Contrôle avec des caméras}
\newcommand{\documentName}{Essais du template \LaTeX}
\newcommand{\redactor}{M. Dupont}
\newcommand{\titlePageLogo}{title_page_logo.png}

% You can remove that package, but add needed packages here, before using the \input command!
\usepackage{blindtext}
\input{AXDoc/AXPreamble}

% Your text here!

\end{document}
```

*attention, le title_page_logo doit être à côté du .tex pour fonctionner !*

Vous n'avez pas besoin de mettre la commande `\begin{document}` car elle se trouve dans le template.

Note importante : à la première compilation, il se peut que le module qui gère le fond fasse n'importe quoi... il faut alors compiler deux fois de suite (cet effet est doit être corrigé avec une version > 2)

# To Do :
 - création du template AXNote qui permet de créer des notes (rapport d'intervention, table d'échange, etc.)
 - mettre à jour le style des titres pour coller à la charte AX disponible dans le gabarit MS Word.

Remarque : un document rédigé avec la version actuelle sera tout à fait compatible avec les version futures. Il suffira de modifier le dossier AXDoc à côté de vos fichiers .tex.


# Changelog
**25/03/2023**, version 2.0
 - les headers et footers sont maintenant gérés par \LaTeX, ce qui limite les erreur de positionnement, de débordement de texte, etc.
 - ajout du package float pour mieux gérer les images flottantes.

**14/04/2023**, version 1.1
 - modification de la police

**12/03/2023**, version 1.0
 - dépôt initial

