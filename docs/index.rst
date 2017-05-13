.. Read the Docs Template documentation master file, created by
   sphinx-quickstart on Tue Aug 26 14:19:49 2014.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

WIPIMO - Recherche d'une solution pour l'aide en ligne
======================================================

J'ai cherché une solution pour réaliser la documentation de l'appli avec si possible la possibilité de générer aussi une version papier.

J'ai privilégié des solutions open source.

J'ai finalement sélectionné deux solutions : 

**Sphinx-doc** http://www.sphinx-doc.org et **MkDocs** http://www.mkdocs.org

Elles sont très similaires conceptuellement et techniquement.

Conceptuellement
****************
Les deux solutions utilisent un `Langage de balisage léger
<https://fr.wikipedia.org/wiki/Langage_de_balisage_l%C3%A9ger>`_ 
pour le contenu. `reStructuredText  <https://fr.wikipedia.org/wiki/ReStructuredText>`_ pour **Sphinx** et `Markdown <https://fr.wikipedia.org/wiki/Markdown>`_ pour **MkDocs**.

Le contenu est ensuite "compilé" aux formats souhaités, site web HTML, fichier PDF, fichier ePub,...

Un projet est constitué :

- d'un ensemble de fichiers ReStrucureText ou Markdown
- d'un thème d'export HTML contenant un fichier CSS pour la mise en forme.
- d'un fichier de configuration d'options de génération

Le contenu est structuré en Titres de différents niveaux ce qui permet la génération automatique de sommaires.

On peut enrichir le contenu de liens, images, tableaux, citations, notes de base de page.

.. note:: différents types de notes sont disponibles **"attention", "caution", "danger", "error", "hint", "important", "note", "tip"**, "warning", "admonition"
.. attention:: Un exemple de note ``attention``.
.. caution:: Un exemple de note ``caution``.
.. danger:: Un exemple de note ``danger``.
.. error:: Un exemple de note ``error``.
.. hint:: Un exemple de note ``hint``.
.. important:: Un exemple de note ``important``.
.. tip:: Un exemple de note ``tip``.

Techniquement
****************
Les deux solutions sont écrites en langage Python. Sphinx à d'ailleurs été conçu pour la documentation de Python.

Elles génèrent un site web statique comprenant un sommaire et une fonctionnalité de recherche.

Elles peuvent être versionnées dans un dépôt Git.

Elles peuvent être déployées et mises à jour automatiquement sur le site https://readthedocs.org comme c'est le cas de ce test utilisant le contenu d'exemple de ReadTheDoc.

Elles peuvent être déployées facilement dans un sous-dossier (réel ou virtuel) de notre application.

Exemples de sites utilisant ces solutions :
*********************************************
**Sphinx :**
""""""""""""""
Page de sites l'utilisant http://www.sphinx-doc.org/en/stable/examples.html

https://docs.readthedocs.io/en/latest/ (readthedoc theme)
http://libelemental.org/documentation/dev/index.html (readthedoc theme)
https://pip.pypa.io/en/latest/ (readthedoc theme)

http://pylangacq.org/ (alabaster theme)

http://pythonhosted.org/pymqi/

http://doc.jsfiddle.net/

https://docs.python.org/3/

http://mapserver.org/

http://docs.ceph.com/docs/master/

**MkDobs :**
"""""""""""""
http://www.mkdocs.org/

Autres liens :
*********************************************

https://www.ibm.com/developerworks/library/os-sphinx-documentation/

https://gist.githubusercontent.com/ukyo/3000457/raw/f1e0ddeb92b585be2c9078b925ea587ab0483b81/Generic%2520reStructuredText.rst

http://deusyss.developpez.com/tutoriels/Python/SphinxDoc/

https://thomas-cokelaer.info/tutorials/sphinx/rest_syntax.html

Welcome to Read the Docs Template's documentation!
==================================================

Contents:

.. toctree::
   :maxdepth: 2
   :glob:

   *



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

