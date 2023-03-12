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
\newcommand{\redactor}{J. LEDIG}
\newcommand{\titlePageLogo}{title_page_logo.png}

% You can remove that package, but add needed packages here, before using the \input command!
\usepackage{blindtext}
\input{AXDoc/AXPreamble}

% Your text here!

\end{document}
```

*attention, le title_page_logo doit être à côté du .tex pour fonctionner !*

Vous n'avez pas besoin de mettre la commande `\begin{document}` car elle se trouve dans le template.

Note importante : à la première compilation, il se peut que le module qui gère le fond fasse n'importe quoi... il faut alors compiler deux fois de suite.

# Note de version

Actuellement, c'est la v1, du 12/03/2023 !

Enjoy

# Changelog
**12/03/2023**
 - dépôt initial

