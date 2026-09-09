# oakia-regles

Ce qui descend dans les postes OAKIA installés, sans attendre une nouvelle
version du logiciel.

Un poste va lire ces trois fichiers, en garde une copie, et continue de
tourner avec la sienne si le dépôt est injoignable. Rien ici n'est du
raisonnement : le raisonnement est dans le code, il ne descend jamais.

## `regles.json` — du vocabulaire

Un mot qui désigne un endroit, un intitulé qui range des actions. Une règle
ne peut qu'AJOUTER un mot à une liste que le logiciel connaît déjà. Elle ne
retire rien et ne remplace rien.

## `reparations.json` — un symptôme, et les gestes qui le soignent

Chaque fiche relie un symptôme et une suite de gestes, tous deux pris dans
les deux listes fermées écrites dans `reparations.py`. Une fiche qui nomme
un symptôme ou un geste inconnu est refusée. Aucun geste n'efface : un
fichier abîmé est mis de côté, horodaté, jamais supprimé.

## `cas_connus.json` — un document qui sortait faux

Ce qu'on attend maintenant d'un document qui s'est déjà trompé. Le logiciel
les rejoue avant chaque livraison. Un cas qui revient interdit de livrer.

## Ce qu'on ne met pas ici

Aucune donnée de chantier, aucun nom de client, aucun extrait de document
réel. Ce dépôt est public.
